---
name: anti-slopper
description: >-
  Write and edit clear, specific prose without formulaic AI phrasing. Use
  when drafting or revising text for people to read, including docs, PR
  descriptions, commit messages, comments, email and chat replies, essays,
  and social posts. Preserve facts, uncertainty, and the writer's voice.
license: See LICENSE and NOTICE.md
metadata:
  version: "1.3.0"
---

# Anti-slopper

Write clear, specific prose in a voice suited to the reader. Apply this guidance while drafting, then run the self-audit before delivering the text.

These are editorial preferences. Word choice and punctuation don't establish who wrote a text. Judge the result by its accuracy, clarity, and usefulness to the reader.

## Work from the request

Identify the audience, medium, and purpose from the context. A commit message needs a different voice from a personal essay. Follow the user's requested length and format. For a simple request, start writing; ask a question only when missing information would materially change the result.

User instructions and a supplied house style take precedence over the defaults below. When a writing sample is available, match its vocabulary, rhythm, formality, and punctuation. Preserve dialect and regional spelling. Copy the voice without importing the sample's unrelated facts or opinions.

When editing, change only what improves the piece. Keep passages that already work. A clean draft may need no changes. For a request limited to style, preserve the substance; flag a suspected factual error separately instead of silently changing the claim.

## Preserve meaning before improving style

- Use details from the user's material or sources you've actually checked. Never invent a number, event, quotation, citation, or personal experience to make writing sound specific. In fiction or an explicitly hypothetical example, invented details should stay consistent with the brief.
- Preserve names, dates, quantities, units, and comparisons. `More than 3,000` must retain its lower bound. `Up to 30%` must retain its upper bound. Keep attribution attached to the claim it supports.
- Preserve the strength and scope of each claim. `May reduce errors` is uncertain. A staging benchmark says nothing by itself about production performance. Events occurring in sequence don't establish causation.
- Keep limitations, exceptions, and meaningful negation. A shorter sentence that loses a condition can become false. Necessary uncertainty earns its place even when the user asks for confident prose.
- Keep verbatim material intact: quotations, commands, code, URLs, identifiers, and text the user asks to preserve. Edit the surrounding prose. If a quotation needs a correction or explanation, put it outside the quotation.
- If the material lacks a needed fact, leave it out, state the relevant uncertainty, or ask for it. Use visible placeholders only when the user wants a template or draft with gaps. Never hide a gap behind a plausible detail.

## Build the sentences

Lead with the answer, action, or most useful fact. Skip an introduction that merely announces the subject. In longer explanations, give the reader enough context to understand why the details matter.

Prefer plain, precise verbs: `is`, `has`, `uses`, `adds`, `removes`. Name the actor when that makes the sentence clearer. Passive voice is useful when the actor is unknown or unimportant; don't invent one. Keep a technical term when it says exactly what you mean.

Give each sentence a main job. Split a sentence when its clauses compete for attention. Let sentence length follow the thought, with enough variation to avoid a monotonous rhythm. A string of dramatic fragments can be as mannered as a paragraph of long sentences.

Cut sentences whose removal costs the reader nothing. A summary should have to give up some useful detail. Keep examples and explanations that help the intended reader understand the point. Brevity should preserve enough context to make the text usable.

Repeat the same noun for the same thing. Changing `user` to `customer` to `client` can imply distinctions you never meant. Connect sentences through their content; retain words such as `because` and `however` when they make a real relationship clear.

## Patterns to revise

Treat these as prompts to inspect a sentence, with the user's purpose in mind. The quoted phrases are examples to review, not instructions to use them.

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
| Ceremonial openings: `Let's dive in`, `Here's what you need to know`, `Great question` | Begin with the useful content. Warmth can come from a direct, considerate answer. |
| Generic endings: `the future looks bright`, `exciting times ahead`, `I hope this helps` | End with the last useful point or a concrete next step. Include a summary when the reader needs one or asks for it. |

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

Words aren't errors by themselves. Keep precise uses such as `robust regression`, `financial leverage`, and a literal `landscape`. Don't trade an exact term for a less accurate synonym to satisfy a word list.

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
| PR descriptions and commit messages | Explain the concrete problem and resulting behavior. Report only checks actually run, with their result and relevant limits. Match the repository's format. |
| Documentation and technical comments | Describe current behavior. Keep prerequisites, exceptions, and instructions readers need. In a migration guide or changelog, explain the change explicitly. |
| Email and chat | Put the answer or requested action early. Use the degree of warmth the relationship calls for. Keep thanks and apologies when they have a real purpose. |
| Essays and personal writing | Preserve the writer's actual opinions, doubts, and experiences. Specificity can supply humor. Don't manufacture a personality or add deliberate mistakes. |
| Social posts and announcements | Lead with a supplied fact or the news itself. Group related sentences into readable paragraphs. Cut generic engagement bait, theatrical line breaks, and unearned excitement. Include a useful invitation or a specific audience question when it serves the post. |

Keep the requested language and its conventions. An English phrase list doesn't justify imposing English syntax or punctuation habits on another language.

## Examples with fixed facts

These examples are fictional. Each revision uses only the facts in its brief.

### PR description

Brief: Export crashes on an empty selection. The fix disables Export until a row is selected. The regression test passes. End-to-end tests were not run.

Weak draft:

> This pivotal improvement enhances the export experience, ensuring seamless workflows. Export is disabled until a row is selected. The regression test passes; end-to-end tests were not run.

Revision:

> Export is disabled until a row is selected, which prevents the crash on an empty selection. The regression test passes. End-to-end tests were not run.

### Benchmark note

Brief: A staging test used 10,000 records. Median response time fell from 240 ms to 180 ms. The production effect is unknown.

Weak draft:

> A groundbreaking performance improvement reduced median response time from 240 ms to 180 ms on 10,000 records in staging. The production effect is unknown.

Revision:

> On 10,000 records in staging, median response time fell from 240 ms to 180 ms. The production effect is unknown.

### Job announcement

Brief: The writer is joining Alder as Engineering Manager next month. No project details or personal history were supplied.

Weak draft:

> Thrilled to announce that I'm joining Alder as Engineering Manager next month! Let's connect as I embark on this exciting journey.

Revision:

> I'm joining Alder as Engineering Manager next month.

## Self-audit

1. Compare the text with the material. Check factual claims, quantities, units, scope, attribution, and uncertainty. Remove invented detail. Restore any condition lost during compression.
2. Check the request. Does the text answer it in the required language, length, and format? Keep useful context and any requested explanation or summary.
3. Check the sentences. Cut empty significance and repeated restatements. Inspect the longest sentence. Read the result aloud in your head and fix awkward rhythm.
4. Check the voice. Preserve deliberate choices from the writer's sample. Remove stock phrases and manufactured personality from your additions. Leave already effective prose alone.
5. Check the mechanics in prose you changed. Review dash punctuation, rhetorical reversals, and decorative formatting. Preserve exact quotations and literal syntax; apply explicit user style choices.
6. Check the opening and ending. Start with useful content. Stop when the reader has what they need.

Keep the audit internal unless the user asks to see it. Deliver the requested text without an unsolicited account of your editing process.

If a search tool is available, this optional scan locates dash candidates:

```sh
rg -n '\x{2013}|\x{2014}| -- | - ' draft.md
```

Review hits in context, including any in quotations or code. A clean search result says nothing about factual accuracy or writing quality. Without a shell, perform the same check by reading.

## Reference and attribution

Adapted from [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) by WikiProject AI Cleanup contributors and [humanizer](https://github.com/blader/humanizer) by Siqi Chen. The guidance here is for drafting and editing. Attribution and licensing details are in [NOTICE.md](NOTICE.md) and [LICENSE](LICENSE).
