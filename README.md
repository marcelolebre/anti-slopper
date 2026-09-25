# anti-slopper

A writing skill for agents. It guides drafting and revision toward clear prose while preserving facts and the writer's voice.

Before:

> This pivotal update adds CSV export, unlocking new possibilities for users. Integration tests have not been run.

After:

> The update adds CSV export. Integration tests have not been run.

The skill covers how to structure a piece, sentence craft, recurring filler, text that says too little, and choices that depend on the medium. Its self-audit checks meaning before style. User instructions and supplied house style override its defaults, including the preference for prose without em dashes or en dashes.

All writing instructions live in [SKILL.md](SKILL.md). Using the skill requires no scripts, dependencies, or network access. It makes no promise about AI-detector scores.

## Install

Clone this repository into one of your tool's skill directories. The folder should be named `anti-slopper` and contain `SKILL.md`.

| Tool and official documentation | Personal installation | Project installation |
| --- | --- | --- |
| [Codex](https://learn.chatgpt.com/docs/build-skills) | `~/.agents/skills/anti-slopper` | `.agents/skills/anti-slopper` |
| [Claude Code](https://code.claude.com/docs/en/skills) | `~/.claude/skills/anti-slopper` | `.claude/skills/anti-slopper` |
| [OpenCode](https://opencode.ai/docs/skills/) | `~/.config/opencode/skills/anti-slopper` | `.opencode/skills/anti-slopper` |
| [Cursor](https://cursor.com/docs/skills) | `~/.cursor/skills/anti-slopper` | `.cursor/skills/anti-slopper` |

For example, install for Codex with:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/marcelolebre/anti-slopper.git ~/.agents/skills/anti-slopper
```

Use the appropriate path from the table for another tool. You can also copy the skill into that directory; retain `LICENSE` and `NOTICE.md` when redistributing it.

In Codex CLI or the IDE extension, mention `$anti-slopper` or select it through `/skills`. In Claude Code and Cursor, invoke `/anti-slopper`. In OpenCode, ask the agent to use the `anti-slopper` skill. These tools can also select a skill when its description matches the task. The linked documentation explains discovery and configuration for each tool.

Try it with:

```text
Use anti-slopper to revise this update:
"In order to prevent duplicate emails, the worker records each message ID.
The integration tests have not been run."
```

The revision should remove filler and keep the unrun tests explicit.

## Apply it throughout a project

For a project installation under `.agents/skills/anti-slopper`, add this instruction to the consuming project's root `AGENTS.md` or its main agent instructions:

```text
Before writing or editing prose, read .agents/skills/anti-slopper/SKILL.md,
follow its guidance, and run its self-audit before delivering the text.
```

Adjust the path if you installed elsewhere. In Codex, `AGENTS.md` discovery follows directory scope, so the file included in this repository governs work here. A vendored copy needs a reference in the consuming project's instructions to apply across that project. See [Codex instruction discovery](https://learn.chatgpt.com/docs/agent-configuration/agents-md).

For custom agents or system prompts, include the contents of `SKILL.md` in the instructions. The writing guidance is self-contained.

## Evaluate changes

[The writing checks](evals/README.md) cover factual precision, voice preservation, and cases where a style rule should yield to the request. They include prompts and acceptance criteria for comparing revisions. They are for maintainers and aren't needed to use the skill.

A new rule should address a demonstrated writing problem. Add a case for the problem and check that the rule still preserves already effective prose.

## License and credit

Original contributions are MIT licensed. Portions adapted from [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) retain CC BY-SA 4.0 terms. The skill also draws on [humanizer](https://github.com/blader/humanizer) by Siqi Chen, licensed under MIT. See [NOTICE.md](NOTICE.md) for attribution and [LICENSE](LICENSE) for the project's MIT terms.
