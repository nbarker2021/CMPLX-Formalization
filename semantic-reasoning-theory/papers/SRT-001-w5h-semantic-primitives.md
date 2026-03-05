# SRT-001: W5H Frames as Semantic Primitives

**Status:** 🔴 Planning  
**Area:** Semantic Reasoning Theory  
**Target Venue:** Journal of Logic and Computation / TACL  
**Authors:** [TBD]

---

## Abstract

We present a formal semantics for the CMPLX W5H (Who, What, When, Where, Why, How) frame system, demonstrating that these six primitives form a complete basis for situational reasoning. We define a logic $\mathcal{L}_{W5H}$ with frame semantics based on situation theory [1], proving completeness and decidability results. Our framework explains how causal DAG structures in the Receipt system encode semantic dependencies between W5H dimensions, enabling automated reasoning about computational provenance.

---

## 1. Introduction

The W5H framework in CMPLX provides six primitive dimensions for describing any computational situation:

| Dimension | Semantic Role | Formal Type |
|-----------|--------------|-------------|
| Who | Agent/Subject | Entity |
| What | Action/Object | Event |
| When | Temporal location | Time |
| Where | Spatial location | Place |
| Why | Causal explanation | Reason |
| How | Method/Process | Procedure |

This paper formalizes these intuitions in a logical framework.

---

## 2. Preliminaries

### 2.1 Situation Theory

We build on Barwise and Perry's situation semantics [1]...

### 2.2 Frame Semantics

Following Fillmore [2], we use frames as structured meaning representations...

---

## 3. The Logic $\mathcal{L}_{W5H}$

**Definition 3.1** (Syntax). The language $\mathcal{L}_{W5H}$ consists of:
- Atomic propositions: $P, Q, \ldots$
- W5H operators: $\mathbf{WHO}, \mathbf{WHAT}, \mathbf{WHEN}, \mathbf{WHERE}, \mathbf{WHY}, \mathbf{HOW}$
- Connectives: $\wedge, \vee, \neg, \Rightarrow$
- Quantifiers: $\forall, \exists$

**Definition 3.2** (Frame). A W5H-frame is a structure:
$$\mathcal{F} = \langle S, D, R, A, T, L, C, M \rangle$$
where:
- $S$ is a set of situations
- $D$ is the domain of individuals
- $R \subseteq S \times S$ is the accessibility relation
- $A : S \to \mathcal{P}(D)$ assigns agents (Who)
- $T : S \to \mathcal{P}(Time)$ assigns times (When)
- etc.

---

## 4. Causal DAG Semantics

The Receipt system's causal DAG structure encodes semantic dependencies...

**Theorem 4.1** (Causal Completeness). Every valid inference in $\mathcal{L}_{W5H}$ corresponds to a path in some Receipt DAG.

---

## 5. Receipt Semantics

We interpret Receipts as proof certificates in $\mathcal{L}_{W5H}$...

---

## 6. Related Work

- Situation semantics [1]
- Frame semantics [2]
- Causal inference [3]

---

## References

[1] Barwise, J. and Perry, J. *Situations and Attitudes*. MIT Press, 1983.

[2] Fillmore, C.J. "Frame semantics." *Linguistics in the Morning Calm*, 1982.

[3] Pearl, J. *Causality*. Cambridge University Press, 2009.

---

**Source Materials:**
- `source-materials/w5h-analysis.md`
- `source-materials/receipt-semantics-notes.md`
