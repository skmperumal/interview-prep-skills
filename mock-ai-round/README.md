# Mock AI Round

This skill creates a small, HackerRank-style coding exercise and supports the
candidate through debugging, implementation, test-gap analysis, and an
AI-assisted engineering discussion. A round starts with a realistic issue and
starter tests; it includes an intentional implementation defect and at least
one stated edge-case requirement for the candidate to investigate and cover.

## Install

Make the `mock-ai-round/` directory available in your AI coding assistant's
skills directory. The skill definition is in [`SKILL.md`](SKILL.md).

## Use

Ask your assistant to set up a round, optionally specifying a topic,
programming language, or existing project. For example:

- “Set up a mock AI coding round in Python about retrying a flaky API call.”
- “Create a small TypeScript exercise about pagination in this workspace.”
- “Run a mock AI round using this issue and the current project.”

The skill presents the exercise requirements and how to run the existing tests
without revealing the seeded defect or calling out the intended test gap. Work
through the code and tests with the assistant; compare the complete issue
requirements to the starter coverage, add regression tests, then verify the
implementation and discuss the result.

To solve an exercise you already have, provide its prompt and project instead
of asking the assistant to seed a new one. You can also ask to finish the round
or review the expected answers for structured coaching feedback.
