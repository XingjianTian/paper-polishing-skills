---
name: paper-evidence-check
description: Check whether claims, results, or citations support a specified statement, verify bibliographic details, or compare terminology and numbers across an abstract, body, figures, and tables. Use when the user asks whether a result or citation supports a sentence. For where a paper fails to answer its research questions, use paper-argument-check. Stay within the requested scope.
---

# Paper Evidence and Consistency Check

First identify the requested check: claims, citations, bibliography, or consistency across materials. Perform only the relevant part; do not require a full-paper audit every time. If only a bibliographic record is available, without supporting source text or results, mark specific effect-size claims as “insufficient material.” If the source explicitly measures a different construct or condition, mark the claim as “explicitly unsupported.” Before comparing numbers, check whether they describe the same participants and statistical definition. If that is unclear, report both values and the question to resolve. Report “conflict—value unresolved” only when the numbers are confirmed to be mutually exclusive under the same definition; do not choose a value for the user.

## Four types of checks

### Claims and results

Extract the main conclusions and locate the corresponding results, study design, and scope. Label each “supported,” “partially supported,” “explicitly unsupported,” or “insufficient material,” with a location and reason. Distinguish association from causation, intention from actual behavior, and sample findings from population generalizations. When evidence is insufficient, suggest narrower wording or explain what evidence is needed; do not invent additional analyses.

### Whether a citation supports the statement

Compare the cited sentence with original-source passages supplied by the author or actually read. Check the population, direction, conditions, and design. State the limitation when a title or abstract cannot establish the detail. Distinguish original research from secondhand reporting; several weak citations do not collectively become strong evidence.

### Publication identity

Verify the title, authors, year, and journal against DOI registration records, the publisher, or other reliable original records. Crossref and DataCite can help, but a missing record does not prove a publication does not exist. Use other reliable records for works without DOIs.

“A publication exists,” “the bibliographic details match,” and “it supports this claim” are different conclusions. If retraction status is requested, check publisher notices or authoritative records separately; a resolving DOI does not establish that a paper has not been retracted. Do not fill in bibliographic details from model memory.

### Consistency across materials

Compare construct names, abbreviations, sample sizes, groups, time points, units, and values across the abstract, body, figures, tables, and conclusions. First establish whether numbers should describe the same participants under the same statistical definition. If unclear, report both numbers and what needs checking; report the conflicting values and locations only after confirming they are mutually exclusive under the same definition. Resolve values using author-confirmed original data or analysis outputs. Without an authoritative basis, do not pick a value.

- For example, an “increase in actual usage rate” requires at least two time points using the same definition, which may include a comparable historical baseline. Two groups measured at the same time establish only a between-group difference, not a temporal increase by themselves.

## Output

Report by severity using “location | issue | evidence/source | recommendation | verification status.” Distinguish checked, pending verification, conflict—value unresolved, insufficient material, and explicitly unsupported. State the actual coverage and unavailable material; do not present a spot check as a complete pass. A single-item check can give the judgment, source or evidence, and minimum missing material in one sentence.

## Example requests

“Check whether the numbers in the abstract match the results table.”
“Check whether each of these five citations actually supports its corresponding sentence.”

## Sources

[Prompt library: Alignment, Integrity, Results](https://drshahizan.github.io/polishing-ai/prompts.html), [M08](https://drshahizan.github.io/polishing-ai/modules/m08-references.html), and [reference checker and its limitations](https://drshahizan.github.io/polishing-ai/doi-checker.html). The lookup methods and verification statuses are additional execution guidance.

[中文参考版](https://github.com/XingjianTian/paper-polishing-skills/blob/main/docs/zh-CN/paper-evidence-check.md)
