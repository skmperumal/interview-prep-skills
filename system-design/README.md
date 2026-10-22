# System Design Interview Coach

This skill helps prepare for senior software engineering interviews focused
on system design and distributed systems. It can be used with any AI agent
that can read and follow the instructions in [`SKILL.md`](SKILL.md).

## What the skill does

The coach supports two interactive modes:

### Teaching Mode

Use this mode to learn or review a system-design or distributed-systems
concept. The skill starts from the problem the concept solves, then explains
the mechanism, gives real-world examples, discusses tradeoffs, and connects
the topic to related concepts.

Common topics include CAP and consistency, consistent hashing, sagas,
circuit breakers, rate limiting, database internals, event sourcing, flow
control, replication, and observability.

Example prompts:

- “Teach me CAP theorem for a senior system-design interview.”
- “Explain how the saga pattern works, including tradeoffs.”
- “Help me compare B-trees and LSM trees for interview preparation.”

### Interview Mode

Use this mode to practice a mock system-design interview. The agent acts as
the interviewer: it presents a prompt, listens to your approach, and probes
one question at a time. It avoids teaching or volunteering answers during the
interview, then gives structured feedback on strengths, gaps, and overall
signal when the practice concludes.

Example prompts:

- “Run a mock system-design interview for a URL shortener.”
- “Interview me on designing a ticketing system for a major concert.”
- “Give me a senior-level distributed-systems design challenge.”

You can ask to skip a drill-down or move on. When the interview ends, ask for
feedback or say that you are done.

## Using the skill with any AI agent

The skill is portable and does not require a particular AI product.

1. Make this folder available to your agent. Depending on the platform, copy
   or link `system-design/` into its skills/instructions location, attach
   `SKILL.md` to the conversation, or paste the file's contents into the
   agent's context.
2. Ask the agent to use the system-design interview coach. If the agent
   supports automatic skill discovery, it may activate from a relevant
   request; otherwise, explicitly tell it to follow `SKILL.md`.
3. Choose **Teaching Mode** or **Interview Mode**. The skill's instructions
   ask the agent to clarify the mode before beginning.
4. State your topic or interview scenario, and interact with the coach.

Skill discovery and installation conventions vary between agents. Use the
method supported by your agent; if it cannot load reusable skills, providing
the `SKILL.md` file directly still gives it the coaching instructions.

## Continue a session

During interview practice, ask to “continue” or “go again” to resume the
current mode. If you return after a break, the coach should briefly remind you
where you left off and ask whether you want to continue or switch topics.
