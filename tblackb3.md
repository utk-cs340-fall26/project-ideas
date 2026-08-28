# Hunch: a calibration journal for people who like being right

## Project Summary

Hunch is a web app where you write down predictions about your own life, your work, and the world, attach a confidence percentage to each one, and find out later how good your gut actually is. "This PR gets merged by Friday, 85%." "My team wins the division, 60%." When the resolution date arrives, Hunch tells you what happened and scores you on it.

The part that makes it work: a daily job goes out and checks. Once a day, Convex wakes up, pulls every prediction that has come due, and for anything about the outside world it runs a web search and hands the results to an LLM that decides whether the thing happened, did not happen, or is still unclear. It comes back with a verdict and a source link, and you confirm with one tap. No money, no odds, no betting. You're wagering your own ego.

## Problem

Everybody thinks they have good judgment, and almost nobody has evidence. We make confident calls constantly and quietly forget the ones we got wrong. Forecasters fix this with spreadsheets and Brier scores; the rest of us don't, because resolving fifty old predictions by hand is miserable. Automating that is what turns this into something you'd keep.

## Major Features

- **Log a prediction:** a plain English statement, a confidence slider from 50 to 99 percent, a resolution date, tags, and a flag for whether it is personal or publicly checkable.
- **Daily auto-resolution:** a scheduled job searches for evidence on due public predictions, an LLM judges happened, didn't happen, or unclear, and returns a cited source. Low confidence verdicts get escalated to you instead of guessed.
- **Resolution queue:** the home screen is whatever needs your one-tap confirmation, plus your personal predictions to resolve by hand.
- **Scoring:** Brier score per prediction plus a rolling aggregate, so being confidently wrong costs more than being unsure and wrong.
- **Calibration curve:** bucket predictions by stated confidence, plot stated against actual hit rate. A perfect forecaster sits on the diagonal. Most of us sit above it.
- **Tag breakdowns:** "well calibrated about deadlines, wildly overconfident about sports."

## Technologies

- TypeScript end to end
- TanStack Start for the frontend
- Convex for the backend (queries, mutations, auth, and cron-style scheduled functions, with live client subscriptions so scores update as verdicts land)
- Convex scheduled action + search API + Claude API with a strict structured output schema for the daily resolver
- D3 for the calibration curve
- date-fns for scheduling

## Intended Users

Engineers who estimate for a living, students predicting their own grades, sports and politics arguers, and anyone who has said "I knew that would happen." They want it because it's the only real feedback loop for judgment, and because seeing your overconfidence on a chart is hard to look away from.
