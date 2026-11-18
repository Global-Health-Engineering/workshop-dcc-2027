# Session plan for the DCC 2027 workshop

Planning notes for the slot on Thursday 14 January 2027, 10:45 to 12:00 (75 minutes with discussion). Not part of the submission. Revised on 9 November 2026 after the acceptance and reworked on 18 November 2026; the version of 21 October planned 50 minutes.

| Time | Block | What happens |
|----|----|----|
| 0:00 to 0:15 | Introduction | Why we publish for humans, and the workflow in one picture |
| 0:15 to 0:50 | Building a dataset together | The room contributes through issues and comments on rawtoweb/dcc-2027, and the contributions arrive as different kinds of raw data. Live run with washr from these raw files to a data package and its website. A coding agent performs the steps, and the points where a person confirms are shown. Participants review the documentation and propose changes in comments. pkgreview and the release with a DOI are explained and not run |
| 0:50 to 1:10 | Discussion in four groups | One theme each: oversight, disclosure, sensitive data, credit. Each group answers the question of its theme, writes down two challenges and one recommendation, and one person reports back |
| 1:10 to 1:15 | Take home | Where the dataset and the guide are, how to try washr on your own data, who to ask |

This is the plan since 18 November 2026. The decisions that led to it are at the end of this file. The sections of 9 and 10 November are kept as the record of the earlier plans.

## Plan of 9 November 2026 (replaced)

| Time | Block | What happens |
|----|----|----|
| 0:00 to 0:10 | Why we publish for humans | The five year workflow in one picture, the three stages of data (raw, analysis ready, final), the sample dataset, the live issue everyone comments on, and the links to the participants' own data packages (built before the conference) for everyone to explore during the live run |
| 0:10 to 0:35 | Live run, part 1 | Raw dataset to a documented washr data package in a new repository of the rawtoweb organisation. The agent does the mechanical steps (folder structure, data dictionary, metadata, README). Participants post proposed documentation changes as comments on an issue of that repository, and the changes are merged live with the proposer's GitHub handle on the commit |
| 0:35 to 0:50 | Live run, part 2 | Review with pkgreview, release, DOI, website. The disclosure trail (commit trailers, prompt archive) on the repository. One or two of the participants' packages opened and compared |
| 0:50 to 1:10 | Discussion | The four open questions: oversight of AI curation, disclosure, sensitive data, credit for data. About five minutes per question |
| 1:10 to 1:15 | Take home | Where the repository lives, how to run washr on your own data, who to ask |

## Decisions of 9 November 2026

Later the same day the workshop became the first cohort of a new offer, rawtoweb (one GitHub organisation for many workshops, after the gitklar model); the records of those decisions are in `rawtoweb-dev/admin`, docs/decisions 0001 to 0008. The points below that they changed are marked.

- Duration: the full 75 minutes. The organisers called 60 minutes optimal and offered to release the group early; the full slot gives the discussion 20 minutes and makes room for the participants' packages.
- Hands-on: every participant brings a laptop and has a GitHub account. Proposals are comments on an open issue of this repository, the same method for every contribution at the conference. Running washr on the own laptop (R, washr) stays an optional track. An earlier choice the same day (phones and a web form) was dropped in favour of the issue, because the issue keeps every proposal and its merge public under the proposer's name.
- Preparation and test (changed in the afternoon): the public pre-work website is the cohort path dcc-2027 of the rawtoweb website, https://rawtoweb.github.io/website/dcc-2027/ (repository rawtoweb/website, one site with a path per cohort). Step 1 is a pre-course survey (email, GitHub username, about 12 questions, account created inside the survey), step 2 one comment on the pinned check-in issue of rawtoweb/dcc-2027. Both by Friday 11 December 2026. No organisation invitations. The participant information (participant-information.md) is the short text the organisers send with the link. `gh issue view <number> --comments` lists who has checked in. Whoever arrives without a working account pairs with a neighbour at the table.
- Room: group tables, Wi-Fi for everyone, projector with HDMI.
- Datasets (changed in the afternoon): participants submit their own data or a published CC BY 4.0 or CC0 dataset through the issue form "Submit a dataset" on rawtoweb/dcc-2027 (link or attached file, public from upload, three required tick boxes), by Friday 11 December 2026, no cap. One repository per package in the rawtoweb organisation, built in December with washr and pkgreview, reviewed on the issue, DOI on Zenodo before the conference. Roles: own data lists the owners and the people behind the data as aut and Lars as cre; a republished dataset lists the original authors as dtc, Lars as aut and cre, the participant as ctb, and the corresponding author gets the draft and three weeks (notices by 14 December, over by 4 January).
- Tools shown: washr runs live, pkgreview runs as the review step in part 2.
- The four open questions: named as themes in the abstract, asked in full in the discussion block and in the README of this repository.

## Decisions of 10 November 2026

After the review of the pre-work website. They replace the matching points of 9 November.

- The dataset is step 3 of the pre-work and expected from everyone. Whoever has no data to share says so in the survey of step 1. Participants see the workflow on data they know before the day.
- Steps 1 and 2 are required. The sentence about pairing with a neighbour is gone everywhere.
- No live merging of proposals from the room on one shared dataset. Documentation input comes before the day, through the dataset form and the review on each dataset's issue. In the room everyone posts one comment on the issue of a published package, on what a human reader still misses. One or two are applied live, the rest afterwards, and the commits name the proposer.
- Agenda, subject to change: introduction 15, live run with washr 20 (changed from 10 and 25 the same afternoon), review, release and DOI 10 (pkgreview introduced and not run, the steps shown on a participant's package that has its DOI, the comment), discussion in four groups 25 (one theme each, sticky notes, one person per group reports back), take home 5.
- washr is shown as work a person or an agent can do. pkgreview is introduced as the AI driven layer.
- Running washr on the own laptop is for after the workshop, together with a guide that is being rewritten for use outside openwashdata. It is not part of the session and no date is promised for the guide.
- Roles on a participant package: the participant is an author, for own data and for a published dataset they picked. The original authors of a published dataset are data contributors and are asked by email whether they want to be authors as well. Lars is maintainer only.
- Material to ask of the organisers: group tables, sticky notes and pens.

## Decisions of 17 and 18 November 2026

After a call with the organisers on 16 November 2026. They replace the matching points of 9 and 10 November.

- No dataset from participants before the conference. The organisers saw too much work on my side if 20 people send one, and too little for the workshop if almost nobody does. The dataset form and step 3 are gone.
- The room builds one dataset together. Contributions come through GitHub, a little before the conference and the rest in the room, and they arrive as different kinds of raw data.
- Issues and comments only. Nobody edits files, makes a copy of the repository or joins an organisation. The workshop does not teach GitHub; participants learn how to contribute with issues and comments.
- Pre-work in two steps, due on Friday 8 January 2027: the survey, and one comment on the check-in issue with one line on the kind of data, without name and institution. A reminder goes out that evening to anyone who has not finished, with Tuesday 12 January 2027 as the last day. No time estimates are given for the pre-work.
- The survey has two parts. Part 1 is for planning only. Part 2 (data curation and the four themes) can enter the public workshop dataset, one row per person without name, email address, username or any answer of part 1, and only with a second consent.
- No DOI in the workshop. pkgreview and the release are explained and not run.
- Publishing an own dataset this way is offered after the workshop, on request.
- Agenda: introduction 15, building a dataset together 35, discussion in four groups 20, take home 5.
- The fourth theme is named Credit everywhere.

## Open

- The content of the shared dataset and the routes the contributions take in the room (proposal: a dataset about the room from part 2 of the survey, an issue form, a free text comment and a table filled in the room).
- Whether the public State of Open Data survey responses (https://doi.org/10.6084/m9.figshare.31095940) serve as a second raw source or as the comparison for the Credit theme.

- The name of the repository of the workshop dataset (decided in December).
- The guide for running washr on the own laptop after the workshop, rewritten for use outside openwashdata. No date promised.
- How a comment on an issue becomes a commit that names the proposer (handle in the message, or a Co-authored-by trailer with the GitHub noreply address).
