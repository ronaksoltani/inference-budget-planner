# Project plan: Inference Budget Planner

## Brief

**Type:** Local-first developer tool

**Audience:** Teams planning AI feature costs.

**Problem:** Estimate monthly inference spend from editable token rates, call volume and average context size. Compare quieter, expected and growth scenarios.

## Experience flow

1. Read the scope and privacy boundary before entering data.
2. Load the fictional sample or paste authorized input.
3. Run the local analysis and inspect each rule or calculation.
4. Copy or download a draft only when the user chooses.

## Core capabilities

- Enter your own provider rates per million tokens
- Model input and output tokens separately
- Compare low, expected and growth traffic
- See formulas and assumptions beside every estimate

## Key design decision

Keep the application self-contained and explain what is heuristic, human-reviewed or user-configured. Never imply that a demo replaces a production control.

## Boundaries

All prices are user-entered assumptions. The planner contains no current provider price list, does not call model APIs and is not a billing quote.

## Learning goals

- Keep input handling, analysis and rendering in clear small functions.
- Make empty, invalid and successful states visible and accessible.
- Use semantic HTML, labelled fields, keyboard focus and responsive CSS.
- Document assumptions, local data handling and limitations.

## Next iteration

Add user research and domain-specific validation rules, then document those rules with examples before expanding scope.
