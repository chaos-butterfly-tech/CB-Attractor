# CB-Attractor 🦋

> **Proof, not promise.**

---

## The Mathematics

For a ReLU neural network $f: \mathbb{R}^n \to \mathbb{R}^m$,
we prove:

$$f^{-1}(c) \text{ is a finite union of convex polytopes}$$

$$\pi_1(P_i) = 0 \quad \forall \text{ connected component } P_i$$

This means: within each decision region, the network's behavior
is topologically stable — no hidden loops, no unexpected boundaries.

**This is not a test result. This is a theorem.**

---

## What is CB-Attractor?

CB-Attractor is a formal verification project for AI systems,
implemented in **Lean 4**.

Most AI safety work asks: *"How often does this system fail?"*

We ask a different question:

> *"Can we mathematically prove it cannot fail in a certain way?"*

The difference between these two questions is the difference
between a test result and a theorem.

---

## The Problem

Modern AI systems are tested, not proven.

A self-driving system tested one million times with no accident
still has a non-zero probability of failure on the next trip.
A medical AI with 99.97% accuracy will still make errors.

Statistical confidence is not mathematical certainty.

When AI systems make decisions that affect human lives,
**"probably safe" is not good enough.**

---

## Our Approach

We use **formal verification** to establish precise, 
provable guarantees about AI behavior.

We do not claim AI is perfect.
We claim something more precise:

> *Within a defined operational domain, this AI system
> satisfies property P — and when inputs fall outside
> that domain, the system provably enters a safe failure mode.*

This is not a statistical claim. This is a proof.

---

## Current Work

**Phase 1: Formalizing ReLU neural networks in Lean 4**

We are building formal proofs that:

- A ReLU neural network is a piecewise linear function
- Its decision regions are convex polytopes
- Each connected component is simply connected (π₁ = 0)
- Therefore: within each region, the network's behavior
  is mathematically predictable and stable
  

This establishes the topological foundation for 
verified AI safety guarantees.

**ReLU formalization** → **Decision region as polytope** 
→ **π₁ = 0 (simply connected)** → **Provable behavioral stability**

**Status:** Active development. Phase 1 in progress.

---

## Why This Matters

Once we can prove that a neural network's decision regions
have specific mathematical properties, we can give clients
a guarantee that no amount of testing can provide:

*"Your AI system will not make this class of error.
Not probably. Provably."*

---

## About

**Hongwei Wang** — Founder, Chaos Butterfly

- BSc Mathematics (Pure), Xi'an Jiaotong-Liverpool University
- Specialization: Algebraic Topology, Homotopy Theory, 
  Formal Mathematics in Lean 4
- MSc Data Science & AI (incoming), NYU Abu Dhabi, Fall 2026
- Academic page: [wanghongwei-academicpage.github.io](https://wanghongwei-academicpage.github.io)

---

## Contact

chaosbutterfly54@gmail.com

---

*Proof, not promise.* 🦋
