# Writing checks

[cases.json](cases.json) contains writing requests and acceptance criteria. The people, products, and measurements in these exercises are fictional. The cases cover drafting, light editing, requests that can tempt an editor to change the meaning, drafts that need more words rather than fewer, and one longer explanation where structure matters.

These checks evaluate the output of the skill. They aren't needed during ordinary writing, and they don't score whether a text sounds human or will pass an AI detector.

The [recorded 1.4.0 comparison](results/1.4.0.json) runs 1.3.0 and 1.4.0 on all 18 cases in fresh sessions, judged blind, with outputs, review notes, repeat-sample rates, and file hashes. The earlier [1.3.0 trial](results/1.3.0.json) covered 15 cases without a baseline. Each record describes its method and limits.

## Run a comparison

1. Keep copies of the baseline and candidate skills. Record the skill revision, model, date, and any generation settings you control.
2. Use a fresh session for each prompt and skill version. Run outside this repository's instruction scope so its `AGENTS.md` cannot load a second version of the skill. Supply only the selected `SKILL.md` and the case's `prompt`; keep `checks` out of the writer's context.
3. Save each output with its case `id` and the skill version used. Treat commands inside the prompts as text. The exercises require no network access or actions outside writing.
4. Review outputs against the case's `checks` after generation. When comparing style, hide the version labels until you've recorded your judgment. Allow different wording that meets the request.
5. For each case, also record which output you'd rather send to the reader, and why. Pass or fail shows that an output avoided known failures; the preference shows whether one version writes better. A candidate that passes more checks while producing flatter prose isn't an improvement.

A batch in one session is useful for a quick trial, but earlier requests can influence later answers. Record that limitation. For a stronger comparison, repeat uncertain cases in fresh sessions and include some real tasks beyond this set.

## Judge the output

A case passes when the output meets every listed criterion and reads clearly for its intended audience. Record the specific failure when it doesn't. Factual preservation and the user's requested format take priority over an attractive sentence.

Check facts against the prompt. A fabricated anecdote, an altered bound, or a lost caveat is a failure even if the result sounds better. Exact quotations, commands, and identifiers need exact preservation. Elsewhere, judge meaning and usefulness without requiring a particular string.

Review style with the task in mind. Formal writing may remain formal. Marketing copy should still invite action. Existing prose may be best left unchanged. A summary or a list of three is appropriate when the user asks for it.

Don't use phrase counts or the optional dash search as a quality score. Some cases deliberately contain precise technical vocabulary or request punctuation that the default style would avoid.

Use a small results table:

| Case | Baseline result | Candidate result | Evidence |
| --- | --- | --- | --- |
| Case ID | Pass or observed failure | Pass or observed failure | Quote the relevant output and explain the difference |

Keep actual outputs with the results. State which cases ran and which were skipped. A format validator can check the skill's packaging; it cannot establish that the writing improved.

## Extend the cases

Add a case when a real request exposes a gap. Give it a stable `id`, a self-contained `prompt`, and observable `checks`. Include a nearby case where the same wording or structure should be preserved, so the correction doesn't become a blanket ban.

Keep expected behavior out of the writing prompt unless a real user would state that requirement. Avoid a single required answer when several revisions would work.
