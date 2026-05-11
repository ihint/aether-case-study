# AETHER

Sanitized operating artifacts from a private AI-assisted research-to-operations system.

This repo exists for one reason: to show the work without exposing the private implementation. The core repositories stay closed because they contain operational details, local data paths, and domain-specific strategy logic. What is public here is the transferable engineering: evaluation loops, replay artifacts, scorecards, promotion packets, audit trails, and human approval gates.

[Live control surface](https://ihint.github.io/aether-case-study/control-surface.html)

![AETHER control surface](./assets/aether_control_surface_desktop.png)

```text
SYSTEM STATE    REVIEW ACTIVE
LIVE ACTION     LOCKED
FLOW            TELEMETRY -> REPLAY -> SCORECARD -> PACKET -> HUMAN GATE
BOUNDARY        RESEARCH CAN CONTINUE; LIVE ACTION REQUIRES APPROVAL
```

## Start Here

| Artifact | What It Shows |
| --- | --- |
| [Control surface](./control-surface.html) | The operating cockpit: state, risk, thesis, event context, gates, and audit trail. |
| [Founder-facing case study](./founder-facing-case-study.md) | The narrative version for a skeptical builder reviewing whether the work is real. |
| [Promotion packet sample](./sanitized-promotion-packet.md) | How a candidate moves from idea to replayable, reviewable decision artifact. |

## Operating Model

| Layer | Job | Boundary |
| --- | --- | --- |
| Hypothesis intake | Turn an ambiguous idea into a replayable candidate. | No operational action. |
| Replay | Reconstruct behavior from artifacts, not vibes. | Missing data blocks confidence. |
| Scorecard | Apply costs, stress checks, and holdout logic. | Positive does not mean approved. |
| Promotion packet | Package evidence for human review. | Claims must point back to artifacts. |
| Approval gate | Separate recommendation from authorization. | Live-capable state requires human approval. |
| Audit trail | Preserve what changed, when, and why. | Decisions stay inspectable after the fact. |

## Why It Matters

The interesting part is not that an AI system can generate ideas. Ideas are cheap.

The interesting part is whether the system can prove which ideas deserve to move forward, show what evidence is missing, and refuse to act when the context is unsafe.

AETHER was built around that line:

- Research outputs are separate from operational actions.
- Candidate states are explicit, not implied.
- AI-assisted discovery is bounded by schemas, replay, scoring, and review.
- A promising candidate can still be blocked.
- The surface emphasizes state, risk, event context, gates, and auditability instead of a simple performance scoreboard.

## Privacy Boundary

This repo intentionally excludes source strategy code, private data files, local paths, repository names, credentials, account details, operational routing details, and proprietary strategy parameters.

The public artifacts are enough to review the engineering shape without leaking the system.
