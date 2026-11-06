---
name: paper-faithful-edit
description: Polish, shorten, or translate existing paper passages or abstracts while preserving meaning. Correct facts only with explicit authorization and verifiable evidence; preserve terminology, numbers, negation, and claim strength. Do not expand the research content.
---

# Faithful Paper Editing

Address the requested issue: grammar, clarity, length, translation, or tone. Do not automatically add structural rewriting, simulated peer review, or submission checks.

## Approach

- Correct ordinary spelling, grammar, punctuation, and obvious formatting directly. Numbers, units, groups, negation, constructs, and claim strength carry facts or meaning: change them only when the user explicitly authorizes correction and supplies a clear basis. Otherwise, use the original text and user-supplied data as the basis, preserving construct names, technical terms, values, units, citations, and study scope. Follow the user or journal's English spelling convention; by default retain the original's predominant variant.
- Do not add claims, references, results, or methods while editing language. If notes are allowed, list ambiguities or conflicts separately for confirmation. If the user wants only the edited text and its meaning can be faithfully retained, preserve the original facts without inserting markers. If translation requires choosing between opposite meanings, ask only about that passage rather than guessing a correction.
- When both checking and editing are requested, retain the original language and claims in the edited text. Put evidence judgments, unresolved claims, and required source material separately. Do not turn an unresolved claim into a new statement about a work “being cited” or “reporting” something.
- English author names, titles, or DOIs in a citation do not authorize translation. Keep Chinese source text in Chinese unless translation is explicitly requested. For example, editing “Example（2025）有力地证明……” still calls for a Chinese sentence. The language of these instructions does not override the source language or the user's request.
- Check sentence by sentence: is negation retained? Has “no significant difference” become “a small difference”? Has “intention” become “behavior”? Has association become causation? Has the sample scope expanded? Have percentages been inaccurately summarized?
- Distinguish statistical significance, effect size, and practical importance. Do not turn a nonsignificant result into “no effect,” or claim importance from significance alone.
- Remove empty embellishment, stock phrases, and mechanical repetition without weakening or strengthening the original claim. Do not apply a blanket banned-word list. Preserve established disciplinary terms and meaningful authorial phrasing.
- For an abstract, first check the necessary background, question, methods, main results, and conclusion; then shorten to the actual word limit. Ask the author to supply missing results rather than inventing them.
- If only polishing is requested, do not extensively rearrange the text because of potential structural issues. Add a short note only when necessary.

## Output

Provide the edited text, with a few notes on consequential changes to meaning, terminology, or evidence strength. Honor text-only requests. When the original meaning can be retained, do not insert ambiguity markers into a text-only answer; ask about a passage first if faithful translation cannot choose between opposite meanings. If checking is also requested, list the findings and minimum missing material separately rather than inserting unresolved concerns into the edited text. State whether the word limit is met; do not claim an exact count without actually counting.

## Example requests

“Polish this English paragraph without changing technical terms, citations, or numbers.”
“Shorten the abstract to 250 words without losing the main results.”

## Sources

[Prompt library: W-01–W-03, Abstract, Discussion](https://drshahizan.github.io/polishing-ai/prompts.html), [abstract editing example](https://drshahizan.github.io/polishing-ai/example.html), and [common pitfalls](https://drshahizan.github.io/polishing-ai/pitfalls.html). The website's examples are fictional teaching material; do not adopt their numbers or citations as research facts.

[中文参考版](https://github.com/XingjianTian/paper-polishing-skills/blob/main/docs/zh-CN/paper-faithful-edit.md)
