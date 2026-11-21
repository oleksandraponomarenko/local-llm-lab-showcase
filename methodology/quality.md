# How the lab investigates and corrects problems

Oleksandra sets the criteria for accepting a result. If a result falls short, the lab records the deviation, checks the original request and handover, and identifies who can correct it. The author can examine and respond to findings. The lab records the correction, any change intended to avoid recurrence, and the evidence available after the change.

## What the corrections journal covers

The corrections journal records deviations in the work, including failures in lab scripts or tools supplied by a model provider. A record describes what was observed, its effect on the work, and any action taken. The lab attributes the cause only when the evidence supports it.

## Project memory across sessions

Oleksandra designed the repository to hold task state, decisions, evidence, corrections and open questions. A receiving session can reconstruct its assignment from the task record and its handover. Before asking Oleksandra to decide, the receiving agent checks that the preparatory work and decision material exist.

See [two documented handovers](../cases/case-004.md) for examples of how agents pick up work from these records. The [synthetic task journal](../journal/synthetic-examples/README.md) shows a handover becoming actionable after its missing evidence is supplied. The [handover template](../templates/task-template.md) records the inputs needed to pick up the work.

## A check with a defined trigger

After a duplicate decision identifier was found, an agent proposed a checker. A second agent implemented it and the first independently tested it. Oleksandra specified that it runs before every commit that changes the journal and during end-of-session review. While this workflow was being prepared, the checker flagged a repeated decision identifier before a commit. The identifier was corrected and the check rerun.

The check covers journal structure and supported identifier references. Reviewers still check whether a valid reference is the intended one.

[Roadmap correction and independent review](../cases/case-001.md) · [Safety research and handover correction](../cases/case-002.md)
