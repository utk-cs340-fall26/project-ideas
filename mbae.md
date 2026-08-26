### The Idea

The idea is to develop a lightweight, Git-backed developer tool that provides function-level code lineage tracking ("block blame") by walking existing Git history and parsing concrete syntax trees via Tree-sitter. It survives complex cross-file refactors, renames, and formatting shifts, pairing structural history with offline LLM-generated intent summaries derived from commit messages and PR diffs, and exposes this deep history to coding agents via a Model Context Protocol (MCP) server.

### The Problem it solves

Standard git blame and line-tracking tools break the moment a function is renamed, reformatted, or moved across files, leaving engineers blind to how code evolved (e.g. legacy/deprecated code). 

Furthermore, AI coding tools see only a snapshot of the code. They can't see what a function used to be or why it changed, so agents routinely delete guards they don't understand and re-introduce bugs that were already fixed once (leading to user frustration). This tool solves both by building a persistent function lineage index that tracks code semantically across time, exposing history to developers via custom UI and to AI agents via MCP.

### Major Features

* Git-Backed Tree-Sitter Backfill: Walks local Git commit history offline, using Tree-sitter byte offsets to index function-level blocks without duplicating source text or altering native Git workflows.
* Semantic Lineage Matcher: Infers function survival across renames and file moves using multi-signal heuristics (signature normalization, body similarity, call-graph position, and co-movement) complete with confidence score metadata.
* Honest Hover-Blame UI: A clean interface that displays block lineage history, warning developers with confidence ratings (e.g., "probable move, XX% confidence") rather than silently failing or guessing.
* Offline Intent Summarizer: Uses a local background model to read historical commit messages and diffs per function lineage, generating a readable chronological log of why the code was changed.
* Lineage MCP Server: Exposes lineage_of(file, line) and intent_history(lineage_id) to coding agents, letting a model retrieve a function's full cross-refactor history and the reasoning behind each change before modifying it.

### Stack

Language & Parsing: Python, with Tree-sitter

Storage: SQLite (for a lightweight, zero-config block and confidence-score key-value store)

UI/Visualization: FastAPI + React + TypeScript (side-by-side block-blame comparison view)

### Intended Users

Software engineers, student groups, and maintainers working on complex or long-lived codebases. They would want this tool because it makes refactoring and understanding legacy code history dramatically faster and more reliable than raw Git diffs.