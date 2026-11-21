# Local LLM Lab Showcase

Oleksandra started Local LLM Lab to build and evaluate a local language model system that adapts to one person and fits her language, way of thinking, and everyday work.

The lab also documents a practical challenge Oleksandra set herself. How far can one researcher take a technical project by drawing on her own research and quality oversight skills and directing two agents from different model families? The showcase traces what she designed, decided, and reviewed, what the agents contributed, and what the team has produced so far.

**Current stage:** research and planning. The lab has produced requirements, reconciled independent safety studies, and a branching roadmap draft with an independent review. The local model, system integrations and adaptation experiments are planned.

[Competencies and evidence](competencies/README.md) · [Lab progress, 13–20 November 2026](evidence/2026-11-20-lab-progress.md) · [Roadmap](roadmap/README.md)

## Why a local language model?

Oleksandra wants a system that can carry useful context and feedback from one task to the next, so she can pick up work without explaining her preferences from scratch. A local core gives her control over what the system remembers, what it shares, and when it changes. The lab will test whether adaptation improves the system’s usefulness across her tasks and whether those gains carry over when she changes models.

The [roadmap](roadmap/README.md#branches-by-resources-and-capabilities) shows how the system could develop along several paths, from a small local model on available hardware to a local core that can call selected cloud services or support additional integrations as resources allow.

## Workstreams

```mermaid
flowchart TB
    Lab["Local LLM Lab"]
    Lab --> Management["Management"]
    Lab --> Design["System design"]
    Lab --> Learning["Learning and behaviour"]
    Lab --> Delivery["Build and evaluation"]
    Management --> Journal["Journal, decisions and quality checks"]
    Design --> Requirements["Requirements and safety"]
    Design --> Platform["Platform and resource choices"]
    Learning --> Behaviour["Reasoning and interaction"]
    Learning --> Materials["Feedback and case-based materials"]
    Delivery --> Capabilities["Capabilities by configuration"]
    Delivery --> Evaluation["Baseline, adaptation and regression checks"]
```

Oleksandra defined four research streams for the plan:

| Stream | Question |
|---|---|
| Safety framework | How should the system protect the owner and constrain what the model can do across roles and devices? |
| Reasoning and behaviour | How can the system keep plausible interpretations open and respond proportionately to a correction? |
| Learning architecture | Which feedback should carry forward, and through what mechanism? |
| Case-based learning materials | How can examples teach reasoning about a situation and support staged evaluation? |

The [roadmap](roadmap/README.md) shows how the work branches with available resources and what must be in place before a capability can be added. [How we rebuilt the roadmap](cases/case-001.md) explains why the tree changed.

## How the lab works

Oleksandra sets the research goal and acceptance criteria, directs the work, reviews evidence and takes decisions. Agents research, draft, implement and document assigned work. An agent can review another agent's result independently, with each contribution credited to its author.

When work falls short, the lab records what happened, investigates contributing causes and checks what changed after a correction. In one case this produced [a branching roadmap with explicit assumptions and dependencies](cases/case-001.md). In another it led to [two independent safety studies and a recorded correction to a research claim](cases/case-002.md).

- [Methodology and quality checks](methodology/README.md)
- [Synthetic example of a working task journal](journal/synthetic-examples/README.md)
- [Cases](cases/README.md)
- [Evaluation evidence and planned checks](evidence/README.md)
- [Reusable templates](templates/README.md)

See the [licensing proposal](LICENSING.md) for the current status of reuse terms.
