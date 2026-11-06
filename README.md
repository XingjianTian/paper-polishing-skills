# Paper Polishing Skills

**English (primary)** · [简体中文](README.zh-CN.md)

Four focused AI skills for academic writing: check arguments, edit faithfully, verify evidence, and prepare submission or revision materials.

**Use one skill for the task at hand. Combine skills only when you explicitly need multiple deliverables.** A paragraph edit does not need a full manuscript audit or an end-to-end research workflow.

## The four skills

| Skill | Use it to | Example request |
| --- | --- | --- |
| [paper-argument-check](paper-argument-check/SKILL.md) | Check argument structure and alignment between questions, methods, results, and contributions | “Identify where the introduction fails to address the research question. Do not rewrite it yet.” |
| [paper-faithful-edit](paper-faithful-edit/SKILL.md) | Polish, translate, or shorten text while preserving meaning; correct facts only with authorization and evidence | “Shorten this abstract to 250 words. Preserve numbers, terminology, and claim strength.” |
| [paper-evidence-check](paper-evidence-check/SKILL.md) | Check whether results or citations support a claim, and reconcile bibliographic or numerical discrepancies | “Does this citation support the claimed 17% reduction, or does the DOI only identify the paper?” |
| [paper-submission-revision](paper-submission-revision/SKILL.md) | Prepare submission documents and reviewer responses grounded in actual materials | “Draft responses from these comments and revisions. List undecided items separately.” |

## Install and use

Each folder is a standalone skill with a `SKILL.md` entry point. Ask a file-capable assistant to follow that file, or copy the skill you want into your Codex skills directory:

```sh
git clone https://github.com/XingjianTian/paper-polishing-skills.git
cd paper-polishing-skills
mkdir -p ~/.codex/skills
cp -R paper-faithful-edit ~/.codex/skills/
```

Refresh skill discovery or start a new chat as appropriate for your client, then invoke the skill with your text:

```text
Use $paper-faithful-edit to polish the abstract below.
Return only the revised text. Preserve numbers, negation, terminology,
British spelling, and the strength of the conclusions.
[paste abstract]
```

If you need both evidence checking and editing, request both deliverables and keep their outputs separate. If you have already confirmed the correct value and only need the text corrected and polished, `paper-faithful-edit` is enough.

The installed instructions are in English. They do **not** require English output: follow the user's requested language, and preserve the manuscript's language unless translation is requested. [Chinese reference translations](docs/zh-CN) are secondary reading copies, not additional installable skills. See the [Chinese usage guide](使用说明.md) for further routing examples.

## Working boundaries

- Faithful editing preserves the original language, attribution, numbers, and claim strength. Keep evidence concerns separate; change facts only with explicit authorization and a clear basis.
- Matching a bibliographic record identifies a work. Establishing support for a claim requires the relevant source text, results, or study design.
- Before calling different numbers a contradiction, check whether they describe the same sample and statistical definition. Report missing information rather than guessing a correct value.
- Reviewer responses distinguish verified changes, explicitly planned changes, and supported disagreements. Keep internal tasks and undecided items outside the response draft; do not invent completed work or commitments.
- External searches, full-text access, and policy checks depend on the assistant's available tools. These instruction files do not provide database access themselves.

## Sources and adaptation

Adapted from Mohd Shahizan Othman's [Polishing Your Draft Article Using AI Tools](https://drshahizan.github.io/polishing-ai/) workshop materials. The project reorganizes the material into focused tasks and adds practical execution boundaries. Each skill links to its specific sources.

This is an independent adaptation, not an official skill collection, a site mirror, or a verbatim translation. Rights to third-party materials remain with their respective owners; publishing this repository does not relicense those materials.

## Validation

The original Chinese instructions received web Pro review, targeted corrections, and behavioral spot checks covering skill selection, authorized corrections, missing evidence, and revision responses. The English edition translates those instructions and is checked separately for format and translation consistency. That prior review does not constitute a separate Pro review of the English wording.

These checks do not guarantee publication quality, acceptance, client-side automatic discovery, or access to real bibliographic databases.
