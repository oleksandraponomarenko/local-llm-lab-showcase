# Synthetic task journal: choosing a document-search configuration

This example is fictional. The lab wants to compare two document-search configurations on one benchmark before deciding which to pilot. The agreed evidence is recall and latency for both configurations.

## First handover

| ID | Owner | Status | Work needed |
|---|---|---|---|
| T-001 | Agent A, executor | In progress | Run both configurations and report recall and latency. Latency is available. Recall is missing. |
| T-002 | Agent B, independent reviewer | In progress | Check that the results use the same corpus and criteria. Return gaps to the executor. |
| T-003 | Research lead | Waiting | Choose a configuration after the comparison passes independent review. Depends on T-001 and T-002. |

## Records during review

| Record | What changed |
|---|---|
| **O-001 — Observation** | Before submitting latency results, Agent A checks the corpus indexes, finds a stale index and reruns both configurations with the correct corpus. |
| **C-001 — Correction** | Agent B finds that the submitted comparison omits recall. Agent A retains the valid latency results and completes the missing measurement under the same conditions. |

## After the correction

| ID | Owner | Status | Result |
|---|---|---|---|
| T-001 | Agent A, executor | Done | Delivered both measures for both configurations. |
| T-002 | Agent B, independent reviewer | Done | Confirmed comparable conditions and complete evidence. |
| T-003 | Research lead | Done | Chose configuration A for the pilot after reviewing the two measures. |

**D-001 — Decision.** The research lead selected A because it met the agreed recall threshold and had lower latency. The decision record is the handover to the pilot.

[Task and handover template](../../templates/task-template.md) · [Review template](../../templates/review-template.md)
