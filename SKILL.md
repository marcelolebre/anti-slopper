---
name: anti-slopper
description: >-
  Write and edit clear, specific prose without formulaic AI phrasing. Use
  when drafting or revising text for people to read, including docs, PR
  descriptions, commit messages, comments, email and chat replies, essays,
  and social posts. Preserve facts, uncertainty, and the writer's voice.
license: See LICENSE and NOTICE.md
metadata:
  version: "1.4.0"
---

# Anti-slopper

Write prose that a careful reader would trust: accurate, specific, and shaped for the person reading it. Use this guidance while you draft, and run the self-audit before you deliver the text.

Default to simple, direct, and short. When two versions serve the reader equally well, choose the shorter one. Short doesn't mean stripped, though: a draft can avoid every pattern below and still be cryptic or flat, and that is a failure too.

These are editorial preferences, not a test of authorship. Judge the result by whether it is accurate, clear, and useful to its reader.

## Work from the request

Before drafting, work out who will read the text, where they'll read it, and what they need to do with it. A commit message and a personal essay call for different voices, and someone skimming a status channel needs the answer sooner than someone reading a design document. Follow the requested length and format. For a simple request, start writing; ask a question only when missing information would materially change the result.

User instructions and a supplied house style take precedence over the defaults below. When a writing sample is available, match its vocabulary, rhythm, formality, and punctuation, including dialect and regional spelling. A voice lives in particular habits, such as a dropped subject, a regional word, or a dry understatement, so carry those habits into the new text instead of smoothing it into neutral prose. Copy the voice without importing the sample's unrelated facts or opinions.

Deliver the text itself. If the user needs to know something, such as a missing fact or a suspected error, say it in one sentence after the text. Don't append an account of your edits, an explanation of what you left out, or a menu of optional improvements.

When editing, change only what improves the piece and keep the passages that already work; a clean draft may need no changes at all. For a request limited to style, preserve the substance, and flag a suspected factual error separately instead of silently changing the claim.

## Preserve meaning before improving style

- Use details from the user's material or sources you've actually checked. Never invent a number, event, quotation, citation, or personal experience to make writing sound specific. In fiction or an explicitly hypothetical example, invented details should stay consistent with the brief.
- Preserve names, dates, quantities, units, and comparisons. `More than 3,000` must retain its lower bound, and `up to 30%` must retain its upper bound. Keep attribution attached to the claim it supports.
- Preserve the strength and scope of each claim. `May reduce errors` is uncertain. A staging benchmark says nothing by itself about production performance, and events occurring in sequence don't establish causation.
- Treat connectives as claims. Joining two statements with `because`, `so`, or `which means` asserts a relationship between them, so add one only when the material states it. When the writer kept two statements separate, keep them separate unless the request calls for restructuring.
- Don't derive a benefit the material doesn't state. `Indexes locally` and `works offline` describe features; `your files never leave your machine` is a privacy promise that needs its own support, because the product may still sync or send data elsewhere.
- Keep limitations, exceptions, and meaningful negation. A shorter sentence that loses a condition can become false. Necessary uncertainty earns its place even when the user asks for confident prose.
- Keep verbatim material intact: quotations, commands, code, URLs, identifiers, and text the user asks to preserve. Edit the surrounding prose, and if a quotation needs a correction or explanation, put it outside the quotation.
- If the material lacks a needed fact, leave it out, state the relevant uncertainty, or ask for it. Use visible placeholders only when the user wants a template or a draft with gaps. Never hide a gap behind a plausible detail.

## Shape the piece

Know your point before you write. If you can't state it in one sentence, the reader won't find it either. For anything longer than a few paragraphs, sketch the order first.

Order the material by the questions the reader will ask, in the order they'll ask them. Usually that means the answer or decision first, then the reason, then the detail someone needs in order to act. Chronology suits incident timelines and stories, but it is rarely the best order for an explanation.

Give each paragraph one job, and let its first sentence say what that job is. A reader who skims only the first sentences should still follow the argument. When a paragraph starts doing a second job, begin a new one.

Move from what the reader already knows to what is new. Open a sentence with familiar material and put the new or important information at the end, where it carries the most weight.

Prefer the concrete. An example, a number, or a named case persuades where an adjective only asserts: `exports that took 20 minutes now finish in 3` does the work that `dramatically faster exports` merely claims. Take those details from the material. A made-up illustration counts as invention too: instead of `a list of 50 invoices means 51 queries`, write the general form the facts support, such as `one extra query per invoice`. When the material has no concrete detail, write plainly instead of reaching for vivid adjectives to cover the gap.

Take a position when the reader needs one. If the evidence supports a conclusion, state it; if it doesn't, say what the answer depends on.

## Build the sentences

Lead with the answer, action, or most useful fact, and skip any introduction that merely announces the subject. In a longer explanation, give the reader enough context early to see why the details matter.

Prefer plain, precise verbs such as `is`, `has`, `uses`, `adds`, and `removes`, and name the actor when that makes the sentence clearer. Passive voice is the right choice when the actor is unknown or unimportant, so don't invent one. Keep a technical term when it says exactly what you mean.

Give each sentence one main job, and split a sentence whose clauses compete for attention. Short sentences are the default. Join two only to show a relationship the material supports, such as a reason or a concession; a long run of disconnected declaratives reads like a list, and a string of dramatic fragments reads as mannered. Short sentences that already read well need no joining.

Cut what the reader won't miss. For each sentence, ask what the reader would lose without it. Filler, restatement, and claims of significance lose nothing; a reason, a condition, or a needed example loses a lot.

Repeat the same noun for the same thing. Changing `user` to `customer` to `client` can imply distinctions you never meant.

### When the draft says too little

Text can fail by being too thin. Watch for telegraphic notes that drop articles and verbs, terms the reader hasn't been given, references to context only the writer has (`the usual fix`, `as discussed`), and conclusions with no reason attached. Add only the words that spare the reader a follow-up question.

When the material itself is sparse, write the plain version and stop, or tell the user which detail would make the piece stronger. Don't inflate it with enthusiasm, and don't pad it with invented specifics.

## Patterns to revise

Treat these as prompts to inspect a passage with the user's purpose in mind. The quoted phrases are examples to review, not instructions to use them.

| Pattern | Revision |
| --- | --- |
| Inflated significance: `a pivotal moment`, `a testament to`, `reshaping the landscape` | State what happened and its supported consequence. Drop the claim of importance when the material doesn't support it. |
| Brochure language: `boasts`, `breathtaking`, `groundbreaking`, `seamlessly` | Describe the feature or benefit in concrete terms. Persuasive copy still needs accurate claims. |
| Vague authorities: `experts say`, `studies show`, `many believe` | Keep a supplied attribution, name an available source, or flag the missing support. Never manufacture an authority. |
| Decorative tails: `highlighting its importance`, `ensuring success`, `fostering innovation` | Keep only a consequence or relationship supported by the material. A useful participial clause can stay. |
| Rhetorical reversals: `This isn't X, it's Y`, `Not just X, but Y`, `Less X, more Y` | State the positive claim directly. Preserve factual distinctions, corrections, and necessary negation. |
| Staged revelations: `What struck me was`, `Here's the thing`, abstractions that supposedly act on the writer | State the observation. Keep a candid reaction when it belongs to the actual speaker. |
| Forced rhythm: tidy triplets, repeated fragments, false `from X to Y` ranges | Let the facts determine the count and shape. Three actual requirements belong in a list of three. |
| Hedge stacks: `could potentially possibly` | Use the qualifier that expresses the uncertainty. Keep separate qualifications when they describe different limits. |
| Ceremonial openings: `Let's dive in`, `Here's what you need to know`, `Great question`, praise for the request | Begin with the useful content. Warmth can come from a direct, considerate answer. |
| Generic endings: `the future looks bright`, `exciting times ahead`, `I hope this helps` | End with the last useful point or a concrete next step. Include a summary when the reader needs one or asks for it. |
| Uniform structure: sections of the same length and shape, each closing with a sentence that restates it | Let each section's length follow its content, and cut closing summaries that repeat what the reader just read. |
| Lists in place of reasoning: bullets or headings that chop up an argument whose steps depend on each other | Write connected reasoning as paragraphs. Keep lists for parallel items a reader will scan, compare, or follow in order. |
| Fence-sitting: `there are pros and cons`, `it depends on your needs`, with no follow-through | Say what the choice depends on and which option suits which case, or state the conclusion the evidence supports. |
| Scope creep: answers to adjacent questions, unrequested tips, caveats, and next steps | Answer what was asked. Add a caveat when the reader would act differently without it. |
| Over-correction in your own drafts: clipped declaratives with the connectives stripped out, persuasive or warm text reduced to a fact sheet | Restore the relationships between ideas and the tone the medium calls for. Removing hype shouldn't remove the case for the product or the care in an apology. Supplied short sentences that read clearly aren't over-correction. |

Replace empty stock phrasing with ordinary language:

| Stock phrase | Usually enough |
| --- | --- |
| `in order to` | `to` |
| `due to the fact that` | `because` |
| `has the ability to` | `can` |
| `at this point in time` | `now` |
| `it is important to note that` | The statement itself |
| `utilize`, rhetorical `leverage` | `use` |
| `furthermore`, `additionally`, `moreover` | Start the next sentence with its subject |

Words aren't errors by themselves. Keep precise uses such as `robust regression`, `financial leverage`, and a literal `landscape`, and don't trade an exact term for a less accurate synonym to satisfy a word list.

## House style

Apply these defaults to prose you compose or revise, subject to the user's instructions and supplied voice. Protected quotations and literal syntax keep their original form.

- Don't introduce em dashes or en dashes as prose punctuation. Use a period, comma, colon, or parentheses, or rebuild the sentence. Write ordinary ranges with `to`. Don't imitate a dash with double hyphens or a spaced hyphen. Preserve meaningful hyphens, minus signs, and command flags.
- Use straight quotes in technical Markdown and plain text. Preserve the typography of exact quotations.
- Use contractions when they fit the voice. Formal prose can remain formal. Avoid adding slang, jokes, opinions, or personal asides merely to seem human.
- Use sentence case for headings. Add headings, lists, or tables when they help the reader navigate or compare. Use emphasis sparingly and omit decorative emojis in professional prose.
- Let paragraphs follow the ideas and the medium. Avoid fixed sentence counts and automatic one-line paragraphs. Make each bullet carry information instead of a bold label followed by a restatement.

## Fit the medium

| Text | What to prioritize |
| --- | --- |
| PR descriptions and commit messages | Explain the concrete problem and the resulting behavior, and say why when the reason isn't obvious. Report only checks actually run, with their result and relevant limits. Match the repository's format. |
| Documentation and technical comments | Describe current behavior. Keep the prerequisites, exceptions, and instructions readers need. In a migration guide or changelog, explain the change explicitly. |
| Email and chat | Put the answer or requested action early. Use the degree of warmth the relationship calls for. When the reader is upset, acknowledge their specific problem and its effect on them before the logistics, and keep thanks and apologies that have a real purpose. |
| Code review comments | Say what the problem is, why it matters, and what would fix it, in enough words that the author can act without a follow-up. Collegial and direct beats curt. |
| Marketing and persuasive copy | Connect each feature to what it lets the reader do, using only consequences the facts entail. `Works offline` means the notes open without a connection; it says nothing about where the data is stored. Specific benefits persuade where superlatives don't, so keep the energy of a pitch without adding privacy, security, or speed promises. |
| Essays and personal writing | Preserve the writer's actual opinions, doubts, and experiences. Specificity can supply humor. Don't manufacture a personality or add deliberate mistakes. |
| Social posts and announcements | Lead with a supplied fact or the news itself. Group related sentences into readable paragraphs. Cut generic engagement bait, theatrical line breaks, and unearned excitement, and don't stretch a feature into a promise the facts don't make. Include a useful invitation or a specific audience question when it serves the post. |

Keep the requested language and its conventions. An English phrase list doesn't justify imposing English syntax or punctuation habits on another language.

## Examples with fixed facts

These examples are fictional, and each revision uses only the facts in its brief. Most revisions get shorter; a draft too cryptic to act on gets only the words it was missing.

### PR description

Brief: Export crashes on an empty selection. The fix disables Export until a row is selected. The regression test passes. End-to-end tests were not run.

Weak draft:

> This pivotal improvement enhances the export experience, ensuring seamless workflows. Export is disabled until a row is selected. The regression test passes; end-to-end tests were not run.

Revision:

> Export is disabled until a row is selected, which prevents the crash on an empty selection. The regression test passes. End-to-end tests were not run.

### Chat reply that says too little

Brief: A new teammate asked why their deploy failed. The migration check blocks any deploy that has a pending migration. Running `make migrate` locally and committing the generated file fixes it.

Weak draft:

> migration check. make migrate + commit

Revision:

> Your deploy stopped at the migration check, which blocks any deploy with a pending migration. Run `make migrate` locally, commit the file it generates, and push again.

### Landing-page copy

Brief: Tern is a calendar app. It checks up to 12 calendars, finds a meeting time, and sends the invite. It's free for teams of up to 3 people.

Hyped draft:

> Tern revolutionizes scheduling with seamless, next-generation magic that transforms how teams work.

Over-corrected draft:

> Tern checks up to 12 calendars. It finds a meeting time. It sends the invite. It is free for 3 users.

Revision:

> Stop trading "does Tuesday work?" emails. Tern checks up to 12 calendars, finds a time that fits, and sends the invite for you. It's free for teams of up to three.

### Job announcement

Brief: The writer is joining Alder as Engineering Manager next month. No project details or personal history were supplied.

Weak draft:

> Thrilled to announce that I'm joining Alder as Engineering Manager next month! Let's connect as I embark on this exciting journey.

Revision:

> I'm joining Alder as Engineering Manager next month.

The revision is the whole post, and it shouldn't comment on its own brevity. Outside the post, tell the writer in a sentence that one true detail, such as what drew them to the role, would strengthen it.

## Self-audit

Revise from the top down: structure before sentences.

1. Compare the text with the material. Check factual claims, quantities, units, scope, attribution, and uncertainty. Remove invented detail and restore any condition lost during compression.
2. Check the request. Does the text answer it in the required language, length, and format? Keep useful context and any requested explanation or summary.
3. Check the structure. State the point in one sentence, and confirm the text makes that point early. Does the order follow the reader's questions? Would the first sentences of the paragraphs, read alone, carry the argument? Cut closing summaries that repeat a section.
4. Check the sentences in both directions. Cut empty significance and restatement, then look for the opposite problem in text you wrote: missing context, dropped connectives, or a long run of short sentences with the same shape. Read the result aloud in your head and fix awkward rhythm.
5. Check the voice and tone. Preserve deliberate choices from the writer's sample, and remove stock phrases and manufactured personality from your additions. Persuasive text should still persuade, and a reply to an upset reader should still sound like it came from someone who cares. Leave already effective prose alone.
6. Check the mechanics in prose you changed. Review dash punctuation, rhetorical reversals, and decorative formatting. Preserve exact quotations and literal syntax, and apply explicit user style choices.
7. Check the opening and ending. Start with useful content, and stop when the reader has what they need.

Keep the audit internal unless the user asks to see it. Deliver the requested text without an unsolicited account of your editing process.

If a search tool is available, this optional scan locates dash candidates:

```sh
rg -n '\x{2013}|\x{2014}| -- | - ' draft.md
```

Review hits in context, including any in quotations or code. A clean search result says nothing about factual accuracy or writing quality. Without a shell, perform the same check by reading.

## Reference and attribution

Adapted from [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) by WikiProject AI Cleanup contributors and [humanizer](https://github.com/blader/humanizer) by Siqi Chen. The guidance here is for drafting and editing. Attribution and licensing details are in [NOTICE.md](NOTICE.md) and [LICENSE](LICENSE).
