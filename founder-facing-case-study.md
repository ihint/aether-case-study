# Founder-Facing Case Study: AETHER

I am not applying because I need permission to be useful, and I am not trying to escape my own work.

I am applying because this role matches work I have already been doing: turning messy, high-stakes workflows into evaluated systems that earn trust. AETHER is the proof point. It forced me to build in ambiguity, search hard for leverage, and use AI as an accelerator without letting it replace judgment.

## What I Built

AETHER is a private AI-assisted futures research-to-operations platform.

It takes messy local market data, live futures context, options-regime refreshes, macro/credit/rates context, and ambiguous hypotheses, then turns them into reproducible workflows, compiler blueprints, replay/event artifacts, scorecards, candidate registries, promotion gates, and operator-readable state. The system was designed around one principle: generated research should never silently become operational action.

The strongest proof is not that it produced attractive ideas. The strongest proof is that it killed them. In the latest remote run, plausible post-news MNQ candidates produced thousands of events and were blocked for negative expectancy after costs. That is the discipline I bring: move fast, but make the machine honest.

## Proof

- Built across two generations: legacy runtime/research system to cleaner AI-first research platform.
- Built automated coverage around the risky parts: ingestion, replay, persistence, schemas, compiler behavior, risk gates, registry behavior, operator APIs, and execution-boundary logic.
- Designed explicit states: research-only, review-only, paper-permission, and live approval only by human authority.
- Built a live-context layer that refreshes market context, fuses multiple signals, and exposes when data is stale or contradictory.
- Wrote an aggressive risk-on doctrine with wise drawdown control: more assertive research and paper/shadow testing are allowed only when context and evidence agree, while stale-data, event, execution, drawdown, and human-approval gates remain binding.
- Built local and cloud workflows for messy data, incomplete coverage, scorecards, runbooks, operator state, and audit artifacts.
- Created review artifacts that can block or kill a promising candidate when the evidence fails.
- Deployed an operator surface on a DigitalOcean worker with Postgres-backed state and a profitability endpoint.

Representative artifacts:

- [AETHER control surface](./control-surface.html)
- [Sanitized promotion packet sample](./sanitized-promotion-packet.md)

## Why It Matters

The hard part was not generating ideas. Ideas are cheap, especially with agents.

The hard part was building a system that could answer: what data do we actually have, what is missing, can this be replayed, does it survive costs and holdout checks, is the system allowed to act, what should the next agent do, and can a human understand why a candidate moved forward or got blocked?

That is the part of AI engineering I have been building toward: turning uncertain model-assisted work into useful, reviewable, operationally safe decisions.

## What I Bring

I am useful in the messy middle between idea and production. I can take a vague problem, build the domain language, create the first useful workflow, write the tests, document the boundary conditions, and keep shipping while the system is still taking shape.

I use AI heavily, but I do not treat model output as authority. In AETHER, AI-assisted discovery is bounded by schemas, replay, scorecards, promotion packets, and human approval. That discipline transfers directly to product work where user trust matters.

The repositories are private because they contain operational details and domain-specific logic, but I can walk through the architecture, safety model, testing strategy, and sanitized artifacts.

> I built a system for proving which AI-assisted trading ideas deserve to move forward, and for killing the ones that do not. That is the intensity I bring.
