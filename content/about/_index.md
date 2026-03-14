---
title: "About"
description: "Background, and what I’m exploring on this site."
weight: 100
show_in_menu: true
show_in_menu_when_section_chosen: []
show_in_footer_menu: false
footer_menu_position: 0
footer_menu_position_slot: 1
footer_menu_show_title: true
home_position: 200
home_hidden: true
show_series_index: false
show_tags_index: false
---

I’m Eyal. I have more than 15 years of experience in the field, starting in IT and DevOps, and spending the last 7 years deep in big data and databases.

Today I’m a tech lead on a team that owns the company’s database layer end-to-end. That means I spend a lot of time on the unglamorous details: data shape, access patterns, and what happens when the happy path breaks.

My default bias is “use the best tool for the job”. In practice that means I love learning, because the best tool changes with context, constraints, and the tradeoffs you’re willing to pay.

## What I’m doing here

I’m using this site to share and explore experiments, knowledge, and experience around databases and distributed systems. Sometimes that means distributed databases and replication. Sometimes it’s a boring single-node database and a performance problem that still matters.

Think of this as a writing lab. It’s “learning in public”, but with enough detail that I (or you) can rerun an experiment later.

This is written for engineers who already build and operate systems and want practical notes, and for future-me: a searchable memory with enough context to reproduce conclusions.

## What I’ll write about

I’m interested in the messy space between theory and production:

- Databases: relational and non-relational, storage engines, indexing, query planning.
- Distributed systems: replication, consistency, failure modes, backpressure, queues/streams.
- Performance engineering: benchmarking, profiling, capacity planning, latency vs throughput.
- Operations: observability, incident patterns, rollout strategies, “why did this melt?”

## What “experiments” means here

When I say “experiments”, I mean scoped exercises with a clear question:

- Small benchmarks with clear hypotheses (and the exact commands/config).
- Failure injection and “what breaks first” exercises.
- Tradeoff writeups after shipping: what we chose, what we regret, what we’d do next time.

The scope can range from quick notes to full repos:

- A small hypothesis in a post: a claim + quick test + result (even if the result is “inconclusive”).
- A repeatable lab: scripts/configs, pinned versions, and enough detail to rerun later.
- A full companion repo: code and/or infrastructure (Docker, Compose, Terraform, k8s manifests) to make the setup reproducible and shareable.

## Conventions I’ll try to keep

- Prefer minimal setups and publish artifacts (configs, scripts, datasets) when possible.
- Separate measurements from interpretation.
- Call out unknowns and follow-ups explicitly.

## Reproducibility (when it’s a benchmark)

- State the question and hypothesis up front.
- Pin versions and capture the full config.
- Record the exact commands used to run the test.
- Report workload shape and variance across runs.

## How I’ll write (and where AI fits)

Expect a mix of formats: a series when a topic needs multiple steps, a single long post when it’s best read end-to-end, and short notes when the value is a concrete observation.

I’ll also use AI (LLMs) in the process, mainly as a drafting and research assistant: sharpening an outline, generating alternative explanations, and stress-testing clarity. I won’t treat LLM output as a source of truth. When facts matter, I’ll prefer primary docs, code, and measurements, and I’ll call out when something is a hypothesis versus a result.

## What this is not

This is not a definitive guide, and it’s not vendor-neutral by default. I’ll be explicit about assumptions, environment, and what I didn’t test.

If you’re reading along and see a mistake or a better approach, I’d like to hear it. The best outcome is that a post gets sharper over time.

## What’s coming

Some concrete threads I plan to write up:

- Elasticsearch inverted index internals.
- MySQL: the server’s decision to use temp tables.
- When “distributed” is a tax: choosing a single-node database on purpose.
