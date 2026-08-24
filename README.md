# Cognitive Merkle Trees

**Persistent Cognitive State as a Versioned Intermediate Representation**

[Read the paper (PDF)](paper.pdf)

## Overview

Personalized AI systems can retain information about a person, but the durable person-specific object is often left undefined when evidence grows, state construction changes, or the underlying foundation model is replaced.

This paper introduces **Persistent Cognitive State (PCS)**: a versioned, external, evidence-addressable intermediate representation of documented cognition. The central separation is simple:

> **Evidence is memory. State is interpretation. Intelligence is execution.**

A person-specific state should be determined by admissible evidence and the procedure that compiles it—not by the particular model that happens to execute it.

## Cognitive Merkle Trees

**Cognitive Merkle Trees (CMT)** are a reference architecture for constructing and maintaining this state over time. CMT combines immutable temporal artifacts, provenance-preserving reconciliation, explicit temporal semantics, revocation-local regeneration, and content-addressed commitments while keeping persistent state independent of the runtime executor.

The goal is not to make generated semantics true by hashing them. It is to make the lifecycle of person-specific state **versioned, inspectable, auditable, and portable across compatible models**.

## Evaluation

The paper introduces **CMT-L5**, a leakage-controlled longitudinal corpus of 29,321 public authored posts from five anonymized individuals, together with a future-held-out evaluation protocol. The reported stress test isolates one structural failure mode—unsupported temporal-horizon extension—while explicitly separating that contract result from behavioral accuracy.

The broader behavioral question remains falsifiable: given the same evidence, executor, and representation budget, can a persistent state better predict later authored judgments than alternative representations?

Research from [BootLoader Labs](https://bll.ac/).
