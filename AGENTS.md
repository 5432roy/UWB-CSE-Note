# UWB Class Notes

This repository stores lecture notes for classes at the University of Washington Bothell. Notes arrive as fragments: incomplete sentences, grammar errors, and unordered points are expected. Turn each batch into a clear, complete markdown note without adding material the lecture did not cover.

## Layout

- One folder per class, named with the course code exactly as given (for example `CSS534/`, `CSS581/`).
- One markdown file per lecture date inside that folder.
- Name files `YYYY-MM-DD.md` so they sort chronologically. If two lectures for the same class share a date, append a short kebab-case topic: `YYYY-MM-DD-topic.md`.
- Do not create a file until there is note content for that date. Do not invent empty class folders.

```
CSS534/
  2026-10-06.md
CSS581/
  2026-10-07.md
```

## Distinguishing notes from conversation

When the user clearly asks a question or addresses the agent instead of providing lecture content, respond in chat without adding the question, instruction, or response to the lecture notes. Add the answer to the notes only if the user explicitly asks to include it.

If a message contains both lecture fragments and a question or instruction for the agent, add only the lecture content to the notes. Apply requested corrections to that content without recording the conversation about the correction.

When the user says they forgot or are unsure about a detail in the lecture notes, help complete or verify that detail and update the notes with the result. This is an exception to the rules against adding outside material and including answers without an explicit request. Keep the completion limited to the missing detail, use reliable sources when needed, and mark an inferred completion as tentative when the context does not establish it with certainty. Do not record the user's question or the conversation about the completion.

## Adding or updating a note

1. Put the note in the matching course folder. Create the folder if it does not exist.
2. If a file for that date already exists, merge the new fragments into it. Do not start a second file for the same lecture.
3. Keep the speaker’s technical terms, names, numbers, formulas, and code exactly as given. Fix spelling of ordinary words; do not “correct” jargon, identifiers, or notation.
4. Complete fragments into full sentences and group related points. The wording may be clearer than the raw note. The claims, scope, and order of ideas must still come from the fragments.
5. Leave a gap when a fragment is too incomplete to finish honestly. Use a short italic note such as *unclear in lecture* rather than guessing a definition, proof, or example.
6. Do not add outside explanations, textbook filler, or related topics that were not in the notes. A one-line clarification is fine only when it restates something already implied by the fragments.

## Markdown

Decide the grouping from the content. Prefer a small number of meaningful sections over a flat dump or over-nested headings.

- Start with a level-1 heading: course code, then the lecture date (`# CSS534 — 2026-10-06`). Add a lecture title on that line when the notes include one.
- Use level-2 headings for topics. Use level-3 headings only when a topic has distinct subparts.
- Use paragraphs for explanations and bullet lists for enumerations, steps, and properties. Number steps only when order matters.
- Use a fenced code block with a language tag for code, commands, and pseudocode.
- Use inline code for identifiers, file names, and short syntax.
- Use `$...$` for inline math and `$$...$$` for display math when the notes contain formulas.
- Format mathematical notation with LaTeX inside math delimiters rather than inline code. Use `\mathbb{R}` for the set of real numbers and powers for vector spaces, such as `$\mathbb{R}^2$` and `$\mathbb{R}^{784}$`. Put multi-character exponents in braces and use `\times` for multiplication, such as `$28 \times 28 = 784$`. Preserve the meaning of the supplied notation when formatting it.
- Bold a term the first time it is defined, and selectively bold key takeaways, important constraints, or central results so they are easy to scan.
- Use italics selectively for terms being introduced or discussed and for uncertainty notes. Keep emphasis sparse: highlight short phrases rather than whole paragraphs, and avoid combining bold and italics on the same text.
- Use a markdown table when the notes compare items along the same fields. Do not use a table for a simple list.
- Keep horizontal rules and blockquotes out unless the lecture is quoting a source.

Example shape:

```markdown
# CSS534 — 2026-10-06

## Consensus

A **consensus** protocol lets a set of processes agree on a single value.

- Every correct process eventually decides.
- No two correct processes decide different values.

## Failure model

Processes may crash and then stay silent. The lecture did not cover Byzantine faults.
```

## Tone

Write in plain, direct sentences. Preserve uncertainty that was in the lecture. Do not smooth a tentative claim into a definite one.

Avoid attribution phrases such as "according to the lecture," "the lecture describes," or similar wording used to distance the notes from a claim. If you disagree with a statement or think it is only partially correct, explain the concern in chat and confirm with the user how to record it before changing or qualifying that statement in the notes. Do not silently correct it or add a caveat; decide the wording with the user.
