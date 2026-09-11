# Rule-First External Agent Construction in the Navi System

## Subtitle
External Free Regions, Cross-Platform Functional Extension, and Human-Readable Governance

## Japanese Title
Navi Systemにおけるルール先行型外部エージェント構築 ― 外部自由領域、クロスプラットフォーム機能拡張、人間可読ガバナンス

## Research Question

Can externally constructed, rule-governed agent environments extend the usable functions of AI systems without modifying the underlying model, while preserving human-readable rules, safety boundaries, and human oversight?

## Abstract

This paper presents an exploratory framework for rule-first external agent construction within the Navi System. The approach begins with explicit natural-language meta-rules and construction rules before executable functions are introduced. Rather than modifying an AI model or attempting to bypass platform constraints, the framework places selected functions in an externally constructed environment, termed an *External Free Region*. Agents operating in this region follow its defined rules and may interact with external services while the originating AI system remains subject to its own platform-level constraints.

A central design principle is that functional extension should remain human-readable and auditable. GitHub is used as the authoritative source for active rule sets, while Notion provides a human-readable layer for rule review, improvement proposals, historical changes, and onboarding of additional AI systems. This separation allows rules to evolve without erasing the reasons for previous modifications.

Initial observations suggest that external placement may allow system-level functions to be extended across heterogeneous AI environments even when the internal capabilities of individual platforms differ. The study does not claim universal portability or unrestricted execution. Instead, it investigates whether rule-governed external structures can provide a reproducible method for extending functionality while preserving safety, predictability, and human control.

The paper further proposes an iterative evaluation process in which the same core structure is tested under different contexts, with resulting observations returned to the core rule set for refinement.
