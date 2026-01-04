
# AI System Pattern P03: Separation of Intelligence and Policy

## Problem

Many AI systems embed **business rules inside models**:
- Thresholds hidden in prompts
- Compliance logic learned implicitly from data
- Policy changes requiring retraining or prompt rewrites

This creates systems that are:
- Fragile to change
- Hard to audit
- Difficult to govern
- Impossible to explain when things go wrong

When intelligence and policy are entangled, **no one knows where decisions truly come from**.

---

## Context

This failure mode appears in:
- LLM-based decision systems
- Credit, pricing, moderation, and compliance workflows
- “Smart” automation built too quickly
- Teams optimizing prompts instead of systems

It becomes visible when:
- Business rules change frequently
- Regulators ask “why was this decision made?”
- A model upgrade unexpectedly changes outcomes

---

## Core Insight

**Intelligence should inform decisions.  
Policy should constrain decisions.**

Models answer: *“What is likely?”*  
Policies decide: *“What is allowed?”*

When policy lives inside models, control is lost.

---


## AI System Diagnostic Diagram 

<div style="padding-top: 25px;">
<img src="p03.png" alt="AI System Diagnostic Diagram" width="600" height="500"/>
</div>

**Key annotation:**
The **boundary between Intelligence and Policy must be explicit and enforced**.

---

## How the Pattern Works

### Intelligence Layer

* Produces:

  * Scores
  * Predictions
  * Rankings
  * Reasoning traces
* Characteristics:

  * Probabilistic
  * Replaceable
  * Optimized for signal quality

### Policy Layer

* Encodes:

  * Thresholds
  * Risk rules
  * Legal constraints
  * Business priorities
* Characteristics:

  * Deterministic
  * Versioned
  * Auditable
  * Changeable without retraining

The system works because **each layer has a single responsibility**.

---

## Control Points (Where Leverage Lives)

This separation enables:

* Policy changes without model retraining
* Multiple policies on the same model
* Explicit decision traceability
* Safe experimentation

Concrete control points include:

* Confidence thresholds
* Risk segmentation rules
* Escalation criteria
* Override permissions
* Policy versioning

If you cannot point to these explicitly, policy is leaking into the model.

---

## Failure Modes if Ignored

When intelligence and policy are mixed:

* Small prompt changes cause large behavior shifts
* Compliance logic becomes implicit and unprovable
* Audits turn into forensic exercises
* Teams fear touching the system
* “Model bugs” are actually policy bugs

These systems do not scale responsibly.

---

## Maturity Levels

**Level 1 – Entangled**

* Rules learned implicitly
* Prompts encode policy
* Retraining required for rule changes

**Level 2 – Partially Separated**

* Some rules externalized
* Inconsistent enforcement
* Limited auditability

**Level 3 – Clean Separation**

* Models produce signals only
* Policies are explicit and versioned
* Decisions are explainable and controllable

High-trust AI systems require Level 3.

---

## Reusable Across

This pattern applies to:

* LLM copilots and agents
* Credit and risk systems
* Content moderation
* Medical coding and claims
* Hiring and screening
* Pricing and eligibility engines

Anywhere decisions are constrained by **rules that change faster than models**.

---

## Why This Pattern Compounds

Separating intelligence from policy:

* Reduces operational risk
* Speeds up business iteration
* Simplifies audits
* Makes systems model-agnostic
* Enables safe automation gradients (P02)

This is one of the strongest predictors of AI systems that survive beyond pilots.

---

## One-Sentence Summary

> **Models should generate intelligence, not enforce rules. Durable AI systems separate probabilistic insight from deterministic policy.**

