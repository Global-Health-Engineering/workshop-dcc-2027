# AI disclosure

This statement records how AI was used to produce the files in this repository. It follows the method the Global Health Engineering group at ETH Zurich uses for its outputs: every commit names its author type in a trailer, and the prompts behind AI assisted changes are archived in the repository. The same method is the subject of the "Disclosure" question in the submitted abstract and will be shown in the workshop.

## Summary

An AI coding agent drafted the workshop abstract from two documents I wrote myself, a spoken draft and a prompt with instructions. I chose between the drafts, added review notes, applied one wording change from a reviewer, and decided the final text. The agent ran the word counts, checked one factual claim on the web, rendered the submission documents, and drafted this statement.

## Tools

- Claude Code by Anthropic, running the model Claude Fable 5.1 (model id claude-fable-5-1), on 20 and 21 October 2026 and on 9 November 2026.
- Quarto 1.10 to render the docx. No AI is involved in rendering.

## What the agent did

- Read context from my personal knowledge base: the group's data publishing workflow, the washr and pkgreview tools, and my notes on publisher AI curation services and on AI disclosure.
- Read two public web pages on 20 October 2026: the Frontiers page on FAIR² data management, to check the price and the AI data steward named in the abstract, and the RDM Network page of the University of Basel, to understand the audience.
- Wrote two abstract versions from drafts/spoken-draft.md and drafts/initial-prompt.md, one in plain language and one in conventional academic language, each within the 350 word limit.
- Combined the two into the final version after I asked for the shape of the first and the terminology of the second, and worked my five review notes into it.
- Applied one wording change from a reviewer.
- Rendered the docx, wrote planning/session-plan.md, wrote README.md, drafted the submission email and drafted this statement.

## What I did

- Wrote drafts/spoken-draft.md and drafts/initial-prompt.md without AI and committed them myself.
- Decided to combine the two versions, wrote the review notes in drafts/2026-10-20-abstract-versions-a-b.md, and named the audience.
- Read and approved every version of the abstract. The final text is my responsibility.
- Chose which prompts to archive. The archive is selective: it holds the prompts I selected at each commit, not every message.

## How to verify

- Every commit the agent touched carries an `Assisted-by:` trailer. Every commit I touched carries a `Human-authored: true` trailer. A commit with both trailers is mixed.
- The commit "initial drafts" carries no trailer because I made it outside the commit tool. Its two files are mine.
- The `prompts/` folder holds the archived prompts, one file each, with the model and the files touched. The `Prompts:` trailer of a commit lists the archive ids of that commit.

```
git log --grep='^Assisted-by:'      # commits with AI assistance
git log --grep='^Human-authored:'   # commits with human authored changes
git log --all --grep='<prompt id>'  # the commit behind an archived prompt
```

## Revision of 9 November 2026

After the acceptance, the organisers asked for a revised abstract for the conference website (a sharper introduction, an agenda, learning objectives, prerequisites) and for the setup of the workshop.

What the agent did: read the organisers' email and their comments in the returned docx, checked both of my calendars for the conference day, put the open decisions to me as question boxes, rewrote the abstract in `submission/` to the structure asked for, rendered the docx and the markdown, revised `planning/session-plan.md` to 75 minutes, drafted `planning/participant-information.md` and the reply email to the organisers, built the pre-work website (first in this repository, then, after my decision to make the workshop the first cohort of the rawtoweb offer, as the cohort path of rawtoweb/website with the theme copied from the RDC 2026 Git for Scientists site), adapted the RDC pre-course survey and the gitklar admin scripts for rawtoweb, drafted the cohort repository with the check-in issue and the dataset form, transferred this repository to the Global-Health-Engineering organisation on my instruction, and extended this statement and the README. In the afternoon it put 23 open decisions to me as question boxes in a grilling round and wrote the plan I approved.

What I did: decided the seven points the revision rests on (the full 75 minutes, a laptop and a GitHub account for everyone with comments on an open issue as the channel for proposals and a check-in comment as the test step, running washr as an optional track, the four questions as themes in the abstract, my own addition that participants may send a dataset beforehand and get it published as a data package, the cutoff of 8 January 2027, publication with a DOI under CC BY 4.0 as the condition). The issue channel replaced a web form I had chosen earlier the same day.. I review every text before it goes to the organisers and send the email myself.

This statement was drafted by the agent and reviewed by me.
