Section | Pattern | Question | Score (0-2) | Evidence / Notes | Risk if Missing
---

## SECTION 1 — System Framing & Foundations

| Section     | Pattern  | Question                                                             | Score | Evidence / Notes | Risk if Missing        |
| ----------- | -------- | -------------------------------------------------------------------- | ----- | ---------------- | ---------------------- |
| Foundations | P00, P01 | Is there a clear separation between model output and final decision? |       |                  | Model-driven decisions |
| Foundations | P00, P01 | Can the system outlive any single model or vendor?                   |       |                  | Vendor lock-in         |
| Foundations | P00, P01 | Is AI framed as a decision system, not a model?                      |       |                  | Fragile architecture   |

---

## SECTION 2 — Decision Authority & Automation

| Section          | Pattern | Question                                            | Score | Evidence / Notes | Risk if Missing        |
| ---------------- | ------- | --------------------------------------------------- | ----- | ---------------- | ---------------------- |
| Decision Control | P02     | Is automation graduated (support → partial → full)? |       |                  | Over-automation        |
| Decision Control | P02     | Are automation stages explicitly defined?           |       |                  | Sudden authority jumps |
| Decision Control | P03     | Are intelligence and policy cleanly separated?      |       |                  | Hidden rules           |

---

## SECTION 3 — Economic Control Surface

| Section   | Pattern  | Question                                           | Score | Evidence / Notes | Risk if Missing     |
| --------- | -------- | -------------------------------------------------- | ----- | ---------------- | ------------------- |
| Economics | P04, P14 | Is cost per decision measurable?                   |       |                  | Cost explosion      |
| Economics | P04, P14 | Is value per decision estimated?                   |       |                  | Poor prioritization |
| Economics | P04, P14 | Can cost–quality–risk be tuned without retraining? |       |                  | Slow iteration      |

---

## SECTION 4 — Human Judgment Placement

| Section       | Pattern | Question                                       | Score | Evidence / Notes | Risk if Missing     |
| ------------- | ------- | ---------------------------------------------- | ----- | ---------------- | ------------------- |
| Human-in-loop | P05     | Are humans triggered by uncertainty or impact? |       |                  | Wasted human effort |
| Human-in-loop | P09     | Does confidence actively route decisions?      |       |                  | Unsafe automation   |
| Human-in-loop | P05     | Are humans handling edge cases, not the bulk?  |       |                  | No scalability      |

---

## SECTION 5 — Failure & Resilience Design

| Section    | Pattern | Question                                 | Score | Evidence / Notes | Risk if Missing        |
| ---------- | ------- | ---------------------------------------- | ----- | ---------------- | ---------------------- |
| Resilience | P06     | Are unacceptable failure modes defined?  |       |                  | Catastrophic incidents |
| Resilience | P10     | Are graceful degradation paths designed? |       |                  | Hard failures          |
| Resilience | P06     | Are failure responses pre-defined?       |       |                  | Panic during incidents |

---

## SECTION 6 — Auditability & Ownership

| Section   | Pattern | Question                                         | Score | Evidence / Notes | Risk if Missing |
| --------- | ------- | ------------------------------------------------ | ----- | ---------------- | --------------- |
| Audit     | P07     | Can decisions be reconstructed end-to-end?       |       |                  | Audit failure   |
| Ownership | P13     | Are ownership and seams explicitly defined?      |       |                  | Blame shifting  |
| Audit     | P07     | Are model, policy, and override versions logged? |       |                  | Legal exposure  |

---

## SECTION 7 — Agentic & Multi-Step Behavior

| Section | Pattern | Question                                     | Score | Evidence / Notes | Risk if Missing     |
| ------- | ------- | -------------------------------------------- | ----- | ---------------- | ------------------- |
| Agentic | P08     | Does the system operate in controlled loops? |       |                  | Runaway behavior    |
| Agentic | P08     | Are loop depth, cost, and actions bounded?   |       |                  | Cost / risk blow-up |

---

## SECTION 8 — Long-Tail & Edge-Case Strategy

| Section   | Pattern | Question                                | Score | Evidence / Notes | Risk if Missing    |
| --------- | ------- | --------------------------------------- | ----- | ---------------- | ------------------ |
| Long Tail | P15     | Is the long tail explicitly identified? |       |                  | Hidden risk        |
| Long Tail | P15     | Are tail cases routed differently?      |       |                  | Automation plateau |
| Long Tail | P15     | Is tail learning intentional?           |       |                  | Repeated failures  |

---

## SECTION 9 — Progressive Trust

| Section | Pattern | Question                                          | Score | Evidence / Notes | Risk if Missing     |
| ------- | ------- | ------------------------------------------------- | ----- | ---------------- | ------------------- |
| Trust   | P16     | Is trust treated as a measurable system property? |       |                  | Political decisions |
| Trust   | P16     | Are there explicit gates for scope expansion?     |       |                  | Premature scaling   |
| Trust   | P16     | Can autonomy be reduced quickly?                  |       |                  | Irreversible damage |

---

## SECTION 10 — Governance & Evolution

| Section    | Pattern | Question                                         | Score | Evidence / Notes | Risk if Missing |
| ---------- | ------- | ------------------------------------------------ | ----- | ---------------- | --------------- |
| Governance | P17     | Are policies versioned independently of models?  |       |                  | Audit confusion |
| Governance | P18     | Is post-deployment learning gated and auditable? |       |                  | Silent drift    |

---

## SECTION 11 — Silent Failure Detection

| Section        | Pattern | Question                                 | Score | Evidence / Notes | Risk if Missing |
| -------------- | ------- | ---------------------------------------- | ----- | ---------------- | --------------- |
| Silent Failure | P19     | Are behavioral drift signals monitored?  |       |                  | Late discovery  |
| Silent Failure | P19     | Is “too quiet” considered suspicious?    |       |                  | Hidden harm     |
| Silent Failure | P19     | Are override and routing trends tracked? |       |                  | Trust erosion   |

---