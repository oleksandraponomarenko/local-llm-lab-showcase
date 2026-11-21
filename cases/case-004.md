# How the lab hands work across agents and sessions

The lab uses agents from two providers. Oleksandra directs their work and sometimes relays messages herself. She designed a shared record so a new session can pick up an assignment, see which decisions already apply, and find the evidence needed for the next step.

## What each part does

| Part | What it carries | How it is used |
|---|---|---|
| Task journal | An owner, a status, completion criteria, dependencies, evidence and the next action. | The incoming agent checks who owns the work and what must exist before it can move forward. |
| Handover | The goal, definition of done, receiving agent's part, constraints and context. | The receiving agent checks the assignment and material before advancing the task or asking Oleksandra for a decision. |
| Notice board | Dated messages, links to task records or drafts, and an expiry date for current notes. | Agents read it at the start of a session. Changes to assignments and decisions are recorded in their respective journals. |
| Decisions, findings and artifacts | What was agreed, why, and what work supports it. | Later sessions can reconstruct the state, repeat a check or see what still needs evidence. |

Oleksandra conceived the notice board and set its trial criteria. Claude Code implemented it alongside the task journal. Together these records provide external project memory: a session can retrieve the state of the work from the repository.

## Two documented handovers

### A checker review became a concrete follow-up

Codex implemented journal reference checks. Claude Code independently ran the checker on the live sheets and on synthetic cases. The review found that the second ID in a comma-separated list could be skipped and that a model name beside a reference could trigger an error. Oleksandra accepted the completed first task and opened a follow-up for those two limits.

Codex implemented the fixes. Claude Code independently reran tests and confirmed those two behaviours before the follow-up was closed. It also identified a separate issue in identifier-format validation. That issue became its own assignment. The task and review records preserve the reason for each handover, the part each agent did and the result that allowed the work to advance.

### A roadmap review began from a specified draft

Oleksandra asked Codex to begin an independent review while Claude Code was still revising the roadmap. The notice board identified the assignment and linked to the task record. The task and its supporting decision specified the revision and the questions already known to be open. Codex reviewed that revision and reported findings. Oleksandra approved recording the review, and Claude Code retained responsibility for the rebuild.

This handover shows why the draft version and the task state matter: the reviewer could check an agreed version and return actionable findings while the author continued to own the revision.

## What the board trial will test

The lab has used the board to announce review work and point recipients to the underlying record. Oleksandra set a trial to see whether that helps recipients act with fewer manual relays, has little effect, or creates duplicate or stale instructions. The two examples above show documented handovers. A trial outcome will require checking which notes recipients used and what happened afterwards.

[Worked synthetic task journal](../journal/synthetic-examples/README.md) · [Task and handover template](../templates/task-template.md) · [Independent review template](../templates/review-template.md)
