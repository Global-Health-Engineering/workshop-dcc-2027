# DCC 2027 workshop submission

Workshop proposal by Lars Schöbitz (Global Health Engineering, ETH Zurich) for the Data Curation Conference 2027 of the Research Data Management Network at the University of Basel. The title is "From raw data to a website for humans: a live curation workflow with every AI step disclosed". Submitted by email on 21 October 2026 and accepted on 9 November 2026 for Thursday 14 January 2027, 10:45 to 12:00. The abstract in `submission/` is the version revised for the conference website after the acceptance, with an agenda, learning objectives and prerequisites; the submitted version is release v1.0.0.

## Conference

- Data Curation Conference 2027, "Don't ghost your data or it will haunt you", a cross-disciplinary conference on research data curation, reusability and AI
- Organiser: Research Data Management Network, University of Basel
- Date and place: Thursday 14 January 2027, University of Basel
- Format: workshop session, hands-on and interactive; the call said 30 to 50 minutes, the slot given at acceptance is 75 minutes with discussion (10:45 to 12:00), 10 to 20 participants who choose their workshop at registration
- Submission rules: title and abstract of at most 350 words, naming the discipline, the use case and the data curation aspects, by email to researchdata@unibas.ch with the subject "Submission DCC"
- Submission due 21 October 2026 (extended), accepted 9 November 2026; the revised abstract for the website due in the week of 16 November 2026
- Accepted presentations go on Zenodo under CC BY 4.0 or CC BY-SA 4.0
- Conference page: https://researchdata.unibas.ch/en/services/data-curation-conference-2027/

## AI disclosure

An AI coding agent (Claude Code with Claude Fable 5.1) drafted the abstract from a spoken draft and a prompt that I wrote without AI. I chose between the drafts, reviewed every version and approved the final text. Every commit in this repository names its author type in a trailer, and the prompts behind the AI assisted commits are archived in `prompts/`. The full statement, with what the agent did, what I did and how to verify it, is in [ai-disclosure.md](ai-disclosure.md).

## Pre-work website and the rawtoweb offer

Since the afternoon of 9 November 2026 the workshop is the first cohort of rawtoweb, a workshop offer of Global Health Engineering with one GitHub organisation for many workshops (after the gitklar model). Everything participants touch lives there: the pre-work website at https://rawtoweb.github.io/website/dcc-2027/ (repository rawtoweb/website, one site with a path per cohort), the cohort repository rawtoweb/dcc-2027 with the check-in issue and the dataset form, the pre-course survey (rawtoweb-dev/pre-course-survey) and one repository per data package. This repository stays the record of the conference submission: abstract, session plan, participant text, AI disclosure and later the slides. The website built here on 9 November moved to rawtoweb/website the same day.

## Folders and files

- `submission/` - The abstract: `abstract-workshop-dcc-2027.qmd` is the source, `abstract-workshop-dcc-2027.docx` the rendered file for the organisers, `abstract-workshop-dcc-2027.md` the same text for reading on GitHub; its own `_quarto.yml` keeps it out of the website render
- `ai-disclosure.md` - The full AI disclosure statement
- `drafts/` - What the abstract was built from: `spoken-draft.md` and `initial-prompt.md`, written without AI, and the two earlier versions with review notes
- `planning/` - `session-plan.md`, the plan for the 75 minutes with the decisions of 9 November 2026, `participant-information.md`, the text the organisers send to the registered participants (survey and check-in comment by 11 December 2026, optional R setup, datasets through the form by 11 December 2026); not part of the submission
- `prompts/` - Archived prompts behind the AI assisted commits, one file each
- `references/` - The call for proposals, kept local and out of git

## The four open questions

The revised abstract names four discussion themes. The questions in full, as submitted on 21 October 2026, are asked in the discussion block of the workshop:

- Oversight. Frontiers sells FAIR² data publication at CHF 5,500 per dataset, curated by an AI data steward on a closed platform. How much the author still checks is unclear. In our workflow every AI step is visible.
- Disclosure. We record how AI contributed to each output, in commit trailers and a prompt archive. I show that record for this proposal, the slides and the workshop material, in one public repository.
- Sensitive data. Ours comes from households in low income countries. What may enter a public repository, and when only aggregates may be released, is half-solved for us.
- Rewards. With AI, a paper is drafted in a day from well curated data. Scientific credit should shift towards the data. I invite the room to argue back.

## Repository

Moved from larnsce/dcc-2027 to Global-Health-Engineering/workshop-dcc-2027 on 9 November 2026, after the acceptance. GitHub redirects the old address. Release v1.0.0 (the submitted docx) moved with it.
