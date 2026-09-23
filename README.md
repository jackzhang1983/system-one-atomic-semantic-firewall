# Atomic Semantic Firewall for System One Models

**An early System One Models architecture for exhaustive atomic rule-state verification, high-recall semantic QA, and exception escalation to System Two reasoning.**

**Author:** Zhang Liang (张亮)  
**First public technical note:** 2026-09-23  
**Version:** V0.1

## Core idea

Atomic Semantic Firewall (ASF) compiles large natural-language knowledge assets into **atomic semantic rules**, then compares bounded local state windows against a large or exhaustive set of those rules using high-throughput **System One Models**.

> **Local state window × Atomic Rule Bank → high-throughput semantic verification → escalate only anomalies**

The architecture is motivated by a new cost regime: when narrow semantic judgments become sufficiently fast and cheap, it becomes practical to trade **inference volume for long-context and retrieval dependence**.

## Why System One Models matter

Traditional systems usually choose between:

- deterministic code for exact rules; or
- large general-purpose models for semantic reasoning.

System One Models create a third layer: **high-volume semantic predicates**.

ASF uses that layer for tasks such as:

- canon and character consistency;
- local contradiction detection;
- AI-style and prose pattern scanning;
- educational-content rule checking;
- agent / Skill acceptance testing;
- product-metadata truthfulness;
- translation consistency.

Ambiguous or multi-hop cases are escalated to System Two reasoning.

## Public technical note

See:

**[Atomic Semantic Firewall for System One Models — Technical Note V0.1](./Atomic_Semantic_Firewall_for_System_One_Models_Technical_Note_V0.1.md)**

The technical note defines:

1. Atomic Rule Banks;
2. bounded local state windows;
3. exhaustive or near-exhaustive rule-state verification;
4. the “computation for context” principle;
5. System One / System Two division of labor;
6. false-positive control as a first-class requirement;
7. benchmark hypotheses and limitations.

## Citation

Zhang, Liang. **“Atomic Semantic Firewall for System One Models: Exhaustive Atomic Rule–State Verification for High-Recall Semantic Quality Control.”** Technical Note V0.1, 23 September 2026.

Machine-readable citation metadata is available in `CITATION.cff`.

## Scope

This repository publicly documents the architecture and terminology.

It does **not** publish proprietary production rule banks, private canon files, historical bug corpora, fine-tuning datasets, thresholds, or production pipelines.

## License

The public technical note and repository documentation are intended for citation and reuse under **CC BY 4.0** unless otherwise stated.

