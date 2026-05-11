# Sanitized Promotion Packet Sample

This is a fictionalized artifact based on the structure of the private AETHER workflow. Candidate names, data sources, thresholds, paths, market identifiers, and operational details have been changed or generalized. The purpose is to show how the system thinks, not to disclose private strategy logic.

## Packet Summary

- Candidate: `context_continuation_v1`
- Packet date: 2026-05-10
- Decision state: `research_only`
- Requested movement: research hypothesis to paper candidate
- Decision: blocked pending stronger replay evidence
- Reviewer note: promising trace behavior, insufficient proof for promotion

## Candidate

`context_continuation_v1` is a research hypothesis about whether a structured session-context signal can improve follow-through quality after an initial directional move.

Plain-English thesis:

> When context, direction, and post-event acceptance align, continuation attempts may have better expectancy than the unfiltered baseline.

This packet does not claim the candidate is production-ready. It asks a narrower question: does the available evidence justify moving from research intake to controlled paper observation?

## Evidence Reviewed

Sanitized inputs:

- Local execution/export logs from a simulated operating environment.
- Historical bar and event-derived context features.
- Prior baseline candidate performance.
- Replay output with fixed cost assumptions.
- Scorecard summary generated from the current research pipeline.

Data coverage:

- Historical coverage: partial.
- Real-time observation: limited.
- Export quality: mixed but parseable.
- Known gap: not all required context fields are available across the full test window.

## Replay Summary

| Metric | Result | Gate |
| --- | ---: | --- |
| Candidate events | 184 | >= 100 preferred |
| Holdout events | 37 | >= 20 required |
| Base net | positive | positive required |
| Cost-stressed net | slightly positive | positive required |
| Profit factor | 1.31 | >= 1.25 required |
| Worst-day loss | acceptable | below invalidation line |
| Single-window concentration | high | must not dominate |
| Data completeness | partial | complete preferred |

Initial read:

- The candidate clears the minimum holdout count.
- Cost-stressed performance remains positive but thin.
- A small number of windows contribute too much of the positive result.
- Missing context fields make the replay less trustworthy than the headline score.

## Gate Review

### Paper Gate

Status: `blocked_needs_data`

Reasons:

- Holdout count is acceptable, but not robust.
- Cost-stressed results are positive, but the margin is thin.
- A concentrated time window contributes too much of the candidate's net result.
- The replay depends on derived context fields that are not consistently available across the full data window.

### Arming Gate

Status: `not_reviewed`

Reasons:

- The candidate has not passed the paper gate.
- No operational rehearsal has been requested.
- No execution-path approval is implied by this packet.

## Decision

Decision state: `research_only`

The candidate remains research-only. It should not be added to paper/shadow operation yet.

The correct next action is not parameter tuning. The correct next action is to improve data coverage, rerun replay with the same candidate definition, and verify whether positive performance survives the missing-context fix.

## Next Actions

1. Backfill the missing context fields for the affected historical window.
2. Rerun replay with identical candidate logic and fixed cost assumptions.
3. Add a concentration check to the scorecard so a single window cannot dominate the decision.
4. Promote to paper observation only if the rerun remains positive after cost stress and concentration checks.
5. Preserve this packet as the audit record for why the candidate did not move forward yet.

## Why This Artifact Exists

This packet is a control surface for an AI-assisted research system.

The important behavior is not that the system found a promising idea. The important behavior is that the system refused to promote a promising idea when the evidence was not strong enough.

That is the product lesson behind AETHER: useful AI workflows need a way to say "not yet" with reasons a human can inspect.

