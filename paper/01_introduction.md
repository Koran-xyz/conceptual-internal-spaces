# Natural-Language Rule Construction Across LLM Environments

## An Exploratory Study of Conceptual Internal Spaces and Cross-Platform Functional Convergence

**Status:** Working Paper — Version 0.2  
**Research stage:** Exploratory / hypothesis-forming  
**Last updated:** 2026-09-03

> This is an open research process. This document is not presented as a finished answer. Chapters, experiments, unexpected results, failures, and revisions will be added as the research develops. Independent replication, criticism, falsification, and extension are welcome.

# 1. Introduction

Large language models (LLMs) are increasingly deployed across different platforms, each with its own model architecture, system design, instruction hierarchy, and operational constraints. Despite these differences, natural language remains the primary interface through which users define tasks, roles, constraints, and expected behavior.

This raises a more specific empirical question: **Under what conditions can rules constructed solely through natural language produce comparable rule-related functions across different LLM environments?**

If semantically comparable natural-language rules can support comparable functions across independently implemented AI environments, natural language may provide a lightweight and portable method for specifying behavioral structures without requiring direct modification of model parameters or a single platform-specific software implementation. This possibility does not imply identical internal representations or universal behavior across all AI systems.

In exploratory interactions with multiple LLM environments, natural-language-defined rules were observed to produce some functionally similar rule-following behavior despite differences in platform-specific responses. These observations are uneven in evidential strength: the current project contains recorded pilot evidence for some conditions and historical exploratory observations for others. They therefore motivate standardized cross-platform testing rather than establish universal portability.

To describe and test context-dependent rule structures without making claims about hidden model internals, we use the working concept of a **Conceptual Internal Space (CIS)**. CIS is an operational framework, not a claim about a discovered physical, neural, or uniquely implemented structure inside an LLM. It describes a conceptually defined contextual structure in which natural-language boundaries can organize rules, states, or roles and produce observable context-dependent behavior.

The primary research questions of this work are therefore:

> **RQ1:** Under what conditions can natural-language-constructed rules produce comparable rule-related functions across different LLM environments?
>
> **RQ2:** When platform-specific responses or structural realizations differ, which rule-related functions—such as boundary recognition, contextual separation, switching, persistence, or scope restoration—converge across environments, and where does that convergence fail?

These questions replace a stronger universal formulation with a scope-sensitive one. The aim is not to demonstrate that one identical structure exists across every AI system. Instead, the research seeks to identify the classes of systems, experimental conditions, and rule-related functions for which cross-platform functional convergence can or cannot be reproduced.

This paper presents these questions as part of an exploratory and open research program. Rather than claiming definitive evidence of a universal internal mechanism or platform-independent rule layer, we report preliminary observations, define an operational framework, retain negative and non-replicated results, identify alternative explanations, and formulate hypotheses that can be independently tested, challenged, narrowed, or extended.

---

## Open Research Note

This working paper is versioned as the research develops. Future updates may revise terminology, experimental conditions, scope claims, and interpretations in response to replication, failure, model changes, and criticism. The purpose of this repository is to expose that research process rather than present every intermediate hypothesis as a final conclusion.
