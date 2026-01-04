# AI Enterprise Diagnostic Guide

This repository contains a **system-level diagnostic framework** for evaluating,
designing, and scaling AI systems in enterprise environments.

It is intentionally:
- Model-agnostic
- Vendor-independent
- Domain-portable
- Risk-aware

The focus is not “how to build AI,” but **how to govern, scale, and trust AI systems**.

## Who this is for
- Enterprise AI leaders
- Architects and principal engineers
- Product and platform owners
- Risk, compliance, and audit stakeholders

## What this is NOT
- A model zoo
- A prompt library
- A tooling comparison

This is a **decision diagnostic**.

---

## Why This Repository Exists

Most AI failures in production are **not model failures**.

They are failures of:
- Decision framing
- Automation boundaries
- Human placement
- Policy design
- Economics
- Ownership
- Governance over time

These failures repeat across industries because teams rebuild AI systems **without reusable system-level abstractions**.

This repository exists to:
- Capture those abstractions
- Make them explicit
- Reuse them across domains, vendors, and generations of models

---

## Core Principle

> **Models generate intelligence.  
> AI systems fail at seams — not at models.
> Systems generate outcomes.
**

Sustainable AI advantage comes from **owning the system**, not optimizing the model.

---

## Repository Map (Start Here)

For a full overview, see [`PATTERN_INDEX.md`](./PATTERN_INDEX.md).

Below is a **guided entry point with direct links**.

---

## 00 — Foundations (Mental Models)

These patterns establish **how to think about AI systems**.

- **[P00 — Why Patterns, Not Models](./00-foundation/P00-why-patterns-not-models.md)**  
  Why durable AI value comes from systems, not model choice.

- **[P01 — AI Systems vs AI Models](./00-foundation/P01-ai-systems-vs-ai-models.md)**  
  Draws the boundary between intelligence and decision-making.

---

## 01 — Decision Core (Highest Leverage)

These patterns define **who decides what, and under what constraints**.

- **[P02 — Decision Support → Decision Automation Gradient](./01-decision-core/P02-decision-support-to-automation-gradient.md)**  
  Introduces phased automation instead of binary automation.

- **[P03 — Separation of Intelligence and Policy](./01-decision-core/P03-separation-of-intelligence-and-policy.md)**  
  Keeps business rules out of models.

- **[P04 — Cost–Quality–Risk Control Surface](./01-decision-core/P04-cost-quality-risk-control-surface.md)**  
  Makes AI economically governable.

---

## 02 — Human, Risk, and Trust

These patterns explain **how AI earns trust in real environments**.

- **[P05 — Human-in-the-Loop at Uncertainty Boundaries](./02-human-risk/P05-human-in-the-loop-at-uncertainty-boundaries.md)**  
  Places humans where judgment adds value.

- **[P06 — Failure-Mode–First AI Architecture](./02-human-risk/P06-failure-mode-first-ai-architecture.md)**  
  Designs systems around unacceptable outcomes.

- **[P07 — Audit-First AI Design](./02-human-risk/P07-audit-first-ai-design.md)**  
  Ensures every decision can be reconstructed and defended.

---

## 03 — System Dynamics & Agentic Behavior

These patterns govern **multi-step, adaptive AI systems**.

- **[P08 — Retrieval–Reasoning–Action Feedback Loop](./03-system-dynamics/P08-retrieval-reasoning-action-feedback-loop.md)**  
  Enables controlled agentic behavior.

- **[P09 — Confidence-Calibrated Routing](./03-system-dynamics/P09-confidence-calibrated-routing.md)**  
  Turns uncertainty into a routing primitive.

- **[P10 — Graceful Degradation and Safe Fallbacks](./03-system-dynamics/P10-graceful-degradation-and-safe-fallbacks.md)**  
  Preserves trust under stress and drift.

---

## 04 — Operating Model & Ownership

These patterns determine **whether AI compounds or stalls**.

- **[P11 — AI as a Platform, Not a Project](./04-operating-model/P11-ai-as-a-platform-not-a-project.md)**  
  Explains how AI scales across use cases.

- **[P12 — Model-Agnostic System Design](./04-operating-model/P12-model-agnostic-system-design.md)**  
  Future-proofs systems against model churn.

- **[P13 — AI Ownership and Seam Mapping](./04-operating-model/P13-ai-ownership-and-seam-mapping.md)**  
  Prevents failures at organizational boundaries.

---

## 05 — Economics & Scale

These patterns make AI **measurable, comparable, and scalable**.

- **[P14 — Unit Economics per Decision](./05-economics-scale/P14-unit-economics-per-decision.md)**  
  Measures AI value one decision at a time.

- **[P15 — Long-Tail and Edge-Case Handling](./05-economics-scale/P15-long-tail-and-edge-case-handling.md)**  
  Controls the rare cases that dominate cost and risk.

- **[P16 — Progressive Trust and Scope Expansion](./05-economics-scale/P16-progressive-trust-and-scope-expansion.md)**  
  Expands AI authority safely over time.

---

## 06 — Governance & Evolution

These patterns ensure AI systems **remain safe and relevant after deployment**.

- **[P17 — Policy Versioning with Stable Models](./06-governance-evolution/P17-policy-versioning-with-stable-models.md)**  
  Allows rules to evolve without destabilizing systems.

- **[P18 — Post-Deployment Learning Loops](./06-governance-evolution/P18-post-deployment-learning-loops.md)**  
  Enables controlled learning from real-world outcomes.

- **[P19 — Silent Failure Detection](./06-governance-evolution/P19-silent-failure-detection.md)**  
  Detects failures that look like success.

---

## How to Read This Repository

- **New to the framework:** Start at P00 → P04  
- **Designing a production system:** Focus on P02–P10  
- **Scaling across teams:** Focus on P11–P13  
- **Preparing for audit / regulation:** Focus on P06, P07, P17, P19  
- **Optimizing ROI:** Focus on P14–P16  

Skipping layers creates fragile systems.

---

## One-Sentence Summary

> **This repository defines a complete, navigable pattern language for building AI systems that scale safely, earn trust, and compound value over time.**
