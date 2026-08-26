# Hunch

You know that feeling when a computation spits out something like `1.6180339887...`, or a sequence like `2, 6, 12, 20, 30...`, and some part of your brain says "that looks like it should be something"? Right now, chasing that down means separately remembering that OEIS exists, knowing that libraries like mpmath ship integer-relation solvers, guessing which constants to test against, and then deciding for yourself whether the match you found is real or a coincidence. Hunch puts all of that in one place.

You paste in a sequence or a numeric value, and Hunch searches across several classical forms of mathematical structure — known sequences, polynomial fits, linear recurrences, integer relations among common constants — and returns a ranked list of candidate explanations. Each one comes with a plain-language evidence score based on how well it fits, how simple it is, and whether it holds up against data the tool deliberately held back to test it. You're not just told "the algorithm found something" — you get a sense of whether it's actually worth chasing.

## Major Features

- Instant lookup against the OEIS database of known sequences
- Automatic detection of closed-form (polynomial) fits and linear recurrences, validated against held-out terms
- Integer-relation search against a curated set of mathematical constants for numeric (non-sequence) input, with re-verification at higher precision wherever more digits are computable
- A plain-language evidence score for every candidate
- Side-by-side comparison when multiple explanations fit
- A lightweight web frontend for pasting in input and browsing ranked results

Stretch Goals:

- Automated generation and testing of more complex sequence hypotheses, including nonlinear recurrences, generating functions, and transformations of known sequences
- Experimental Ramanujan Machine-style searches for numerical identities or continued-fraction representations of constants
- Interactive tools for users to modify, combine, and re-test generated conjectures

## Technologies

- Python for backend
- mpmath for arbitrary-precision arithmetic and integer-relation search
- SymPy for polynomial fitting, symbolic work, and linear recurrence detection
- OEIS API for sequence matching
- React + TypeScript for frontend

Technologies for Stretch Goals: 

- SageMath
- Ramanujan Machine / ramanujantools

## Intended Users

Hunch is for math and physics students and researchers doing exploratory or computational work who want a fast, trustworthy first read on a mysterious number or sequence, instead of guessing or grinding through the process by hand. It's also a natural fit for instructors who want a hands-on way to show students how experimental mathematics actually works: spotting a pattern, testing it rigorously, and deciding what's actually worth the effort to prove.
