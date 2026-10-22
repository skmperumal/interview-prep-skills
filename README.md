# Interview Prep Skills

A collection of portable, agent-agnostic skills for interview preparation and
coaching. Each skill is organized in its own folder and includes a `SKILL.md`
file with reusable instructions. Skills can be used with any AI agent that can
read and follow supplied instructions; no single product or platform is
required.

## Skills in this repository

### `system-design/`

A distributed-systems and system-design interview coach for senior software
engineering preparation. It supports:

- **Teaching Mode:** Learn a distributed-systems concept with explanations,
  examples, diagrams, tradeoffs, and related concepts.
- **Interview Mode:** Practice a system-design interview through one-at-a-time
  questions, follow-up probes, and structured feedback.

See [`system-design/README.md`](system-design/README.md) for detailed usage.

## Using these skills with an AI agent

1. Choose the skill folder relevant to your preparation.
2. Make its `SKILL.md` available to your agent. Depending on the agent, you can
   install/copy the folder into its skill or instruction directory, attach the
   file to the conversation, or paste its contents into the agent's context.
3. Ask the agent to use the skill and describe the preparation you want—for
   example, learning a topic, practicing a mock interview, or getting feedback
   on an answer.
4. Follow the skill's interaction guidance. If it offers different modes, name
   your preferred mode or answer the agent's clarification.

Agent platforms differ in how they discover, install, and activate reusable
instructions. Follow the conventions of your chosen agent, or provide the
`SKILL.md` instructions directly. The content is designed to be portable and
does not depend on a specific vendor.

## Download and configure a local agent to use a skill

Clone the repository to download all of its skills, or download the folder for
the skill you want if you only need one:

```sh
git clone https://github.com/perumalmani58/interview-prep-skills.git
cd interview-prep-skills
```

Choose a skill folder in this repository; each skill's instructions are in
that folder's `SKILL.md`. Make the folder or file available to your local AI
agent in whichever way it supports:

- If the agent supports reusable local skills or instructions, follow its
  documentation to add or link the chosen skill folder.
- If it accepts project context or attached files, provide that skill's
  `SKILL.md`.
- Otherwise, paste the contents of `SKILL.md` into the conversation.

Agent conventions for installation, discovery, and activation vary. Do not
assume an agent automatically finds a downloaded skill; explicitly ask it to
follow the instructions. For example, after replacing `<skill-folder>` with
the folder you chose:

> Read and follow `<skill-folder>/SKILL.md` as the instructions for this
> conversation. Use this skill to help me prepare for **[your interview goal
> or topic]**. Follow its guidance, including any mode selection or
> interaction rules it defines.

## Adding more skills

Place each additional skill in a clearly named directory with a `SKILL.md`
file and a folder-level `README.md` describing its purpose and usage. Add a
short entry for it to this top-level README so readers can discover it.
