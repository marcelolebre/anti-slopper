# anti-slopper

An agent skill that makes AI assistants **write like a human**. It works while drafting, before the slop exists, then runs a self-audit before anything ships.

What that looks like:

> **Slop:** This isn't a tool. This is a revolution.
> **Human:** The tool changes how teams ship code.

> **Slop:** Gallery 825 serves as the exhibition space and boasts over 3,000 sq ft.
> **Human:** Gallery 825 is the exhibition space and has about 3,000 sq ft.

> **Slop:** 🚀 Thrilled to announce I'm joining Acme as VP of Engineering! Let's connect!
> **Human:** New job: VP of Engineering at Acme. First project is fixing the deploy pipeline I complained about here in March.

The skill catalogs 37 patterns like these, each with its human alternative: significance inflation, promotional tone, `-ing` padding, em dashes, hedge stacks, "what got me is…" reveals, buried ledes and engagement bait in social posts, and the fatal "this isn't X, it's Y" construction.

Underneath the catalog is a "Sentences first" craft section: the sentence is the unit, default to short, let juxtaposition connect, trust the reader. Most AI tells dissolve once the sentence is right.

Use it for any prose a person will read: PR descriptions, commit messages, docs, comments, design notes, chat and email replies, social posts, and essays.

## Install

The whole skill is one self-contained markdown file, `SKILL.md`. No scripts, no tools, no platform APIs. Any agent that can read a file can use it.

**Claude Code**

```bash
git clone https://github.com/marcelolebre/anti-slopper ~/.claude/skills/anti-slopper
```

Invoke with `/anti-slopper`, or let the agent trigger it automatically when it's about to write prose (the `description` in `SKILL.md` drives auto-selection).

**OpenCode**

```bash
git clone https://github.com/marcelolebre/anti-slopper ~/.config/opencode/skills/anti-slopper
```

(OpenCode also scans the Claude Code skills directory, so either location works.)

**Codex CLI, Amp, Copilot, and other AGENTS.md-aware agents**

Vendor this repo into your project (clone, submodule, or copy) and the included `AGENTS.md` points the agent at `SKILL.md` whenever it writes prose. Or add one line to your existing `AGENTS.md`:

```
Before writing prose for a person to read, follow path/to/anti-slopper/SKILL.md and run its self-audit.
```

**Cursor**

Copy `SKILL.md` into `.cursor/rules/anti-slopper.mdc`, or reference it from your rules file.

**Anything else (custom agents, system prompts, GPTs)**

Paste the contents of `SKILL.md` into the system prompt or instructions. It's plain markdown and self-contained.

## What's inside

- `SKILL.md` — the skill: core habits, 37 patterns with human alternatives, social media registers (hooks, broetry, CTAs), a "personality and soul" section for opinion registers, voice matching, false-positive guidance, and a pre-ship self-audit.
- `AGENTS.md` — a pointer file so AGENTS.md-aware agents pick the skill up automatically when the repo is vendored into a project.

## License and credit

Built on [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) (WikiProject AI Cleanup, CC BY-SA 4.0) and the [humanizer](https://github.com/blader/humanizer) skill by Siqi Chen (MIT).

MIT licensed, except the portions adapted from Wikipedia, which remain available under CC BY-SA 4.0. Details in [NOTICE.md](NOTICE.md).
