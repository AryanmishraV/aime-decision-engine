# AIME Module Structure

This document defines the functional boundaries and responsibilities of each
module within the AIME system.

---

## 1. Manufacturer Module

Handles manufacturing-related decision evaluation using predefined rules,
capacity limits, and cost constraints.

The module determines whether production decisions are viable before execution.

---

## 2. Transport Module

Handles transport and logistics decisions using rules related to availability,
movement cost, capacity constraints, and operational feasibility.

The module prevents transport decisions that exceed acceptable limits.

---

## 3. Digital Twin Module

Runs simulated decision scenarios using the same logic applied to live
operations.

This allows testing of decisions without real-world execution or risk.

---

## 4. DMCE (Decision-Making Cost Evaluation)

Analyzes proposed decisions using historical decision data and past mistake
records.

The module compares current decisions against previously executed decisions
that resulted in losses, delays, or cost overruns.

DMCE applies loss-first logic to quantify potential downside risk and prevent
repetition of known failures.

---

## System Rules

- No adaptive or learning behavior  
- No probabilistic outputs  
- No cross-module logic modification  
- Decisions remain deterministic and repeatable
