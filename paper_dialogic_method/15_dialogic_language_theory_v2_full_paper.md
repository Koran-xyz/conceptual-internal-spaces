# Dialogic Language Theory: Design and Implementation of a Natural-Language-Driven AI System

**Subtitle:** Free-Region Generation and Hybrid-Language System Formation  
**Author:** 清水 稔  
**Status:** Working Paper v2.0  
**Date:** 2026-09-26

## Abstract

This paper proposes **Dialogic Language Theory**, a framework that treats natural language not merely as a prompt or command interface for generative AI, but as a higher-level descriptive medium for forming and modifying roles, rules, relationships, processing regions, agents, memory structures, and external functions in AI systems.

The research originally interpreted sustained natural-language interaction as the construction of an independent “internal free region” inside an AI. Continued implementation and observation led to a revision of that view. The present model does not assume that a new internal software structure is physically created inside the model. Instead, a logical **free region** is defined through natural-language rules, role assignments, context, scope, and current goals. Within that region, the AI may perform hypothesis generation, analysis, reconstruction, and exploratory reasoning, while actions that affect external systems remain subject to the rules, permissions, and constraints of those systems.

The paper further introduces a **hybrid-language approach** in which natural language serves as the human-facing, higher-level description layer, while AI translates selected parts into formal representations such as Python, JSON, SQL, or API calls when repeatability, persistence, precision, or external execution is needed. Human users therefore do not necessarily need to write the formal code directly.

The NAVI system is presented as an implementation example. It separates conversational coordination, specialized agents, deterministic robots, external memory, and cloud services. Early implementation tests include natural-language-driven generation and modification of Excel and Word files, Google Sheets writing and read-back, cloud storage operations, and the conversion of previously language-defined functions into Python-based fixed processing.

The results do not establish that natural language is a programming language in the formal sense, nor that the proposed framework is universally reliable. Rather, they provide an initial demonstration that natural language can function as a higher-level system description layer when paired with AI-mediated translation, explicit execution boundaries, and human confirmation. Future work will evaluate reproducibility, portability across AI models, the effect of meta-rules, the value of external memory, and the limits of natural-language-only system construction.

**Keywords:** dialogic language theory, natural language, generative AI, free region, hybrid language, AI agents, natural-language programming, human-in-the-loop, tool use

---

## 1. Introduction

Large language models have made it possible for users to request writing, analysis, coding, data transformation, and tool use through ordinary language. This changes the traditional relationship between humans and software. In conventional software development, humans usually adapt their intentions to formal languages, APIs, data structures, and interface conventions. In AI-mediated development, a different possibility appears: the user can describe the intended behavior in natural language, and the AI can translate that meaning into executable structures.

This research began by exploring whether roles, rules, memory, agents, and a comparatively free space for reasoning could be formed through dialogue alone. The early interpretation was that natural-language rules created an “internal environment” or “internal free region” inside an AI. That interpretation was useful as a conceptual starting point, but it overstated what could actually be observed from outside the model.

What can be directly observed is different: a model can follow role definitions, apply linguistic rules, switch logical roles, use external records, generate code, call tools, and continue work when sufficient context is restored. These observable behaviors led to a revised research question:

> Can natural language be used as a higher-level system description layer through which a human and an AI jointly form, modify, and operate an executable system?

The research therefore moved away from claims about unobservable internal construction and toward a model of **free-region generation**, where operational boundaries are defined by language, context, and state.

The present paper develops this revised theory, describes the hybrid-language implementation model, presents NAVI as an implementation example, summarizes early experiments, proposes evaluation methods, and identifies limitations and safety requirements.

---

## 2. Core Definition of Dialogic Language Theory

### 2.1 Natural language as a system description layer

Dialogic Language Theory treats natural language as more than a conversational input format. Natural language can describe purpose, constraints, roles, relationships, priorities, exceptions, and desired changes. For example:

> “NAVI acts as the reception desk, identifies what kind of work is required, and routes the request to a specialist. If the correct destination is unclear, it asks the user instead of guessing.”

This is not executable code, but it contains structural information that an AI can interpret as a role definition, routing policy, uncertainty rule, and escalation path.

The theory therefore distinguishes between **human description** and **machine execution**. Human description may remain natural language; machine execution may use any suitable formal representation.

### 2.2 Dialogue as a design operation

The word “dialogic” refers to the fact that system formation is iterative. The user does not need to provide a complete specification at the beginning. A system can evolve through a sequence such as:

1. state an intended function;
2. observe the result;
3. identify a mismatch or missing function;
4. describe the correction in natural language;
5. allow the AI to restructure or regenerate the relevant part;
6. repeat.

In this model, dialogue is not merely task input. It is also a **design operation**.

### 2.3 Minimal model

The minimal form of the theory consists of four elements:

1. a human user;
2. natural language;
3. an AI capable of interpreting that language;
4. iterative dialogue that changes the working structure.

More advanced implementations may add meta-rules, free regions, agents, external memory, robots, formal code, and external services.

---

## 3. From Internal-Construction Hypothesis to Free-Region Generation

### 3.1 The initial hypothesis

The initial model described the AI as if a new internal space were being constructed:

```text
AI
├── ordinary region
└── internal free region
    ├── linguistic rules
    ├── agents
    ├── memory
    ├── roles
    └── exploratory reasoning
```

This description reflected the observed stability of roles and rules during extended interaction.

### 3.2 Why the model was revised

The internal-construction interpretation had three important weaknesses.

First, the user cannot directly inspect the model’s internal architecture and verify that a new persistent software structure has been created.

Second, similar role structures can sometimes be reconstructed on different AI platforms using the same or equivalent natural-language definitions. This suggests that the portable object may be the **description and operational structure**, not a hidden model-specific internal space.

Third, functions originally maintained through language can be moved into Python, JSON, databases, or external tools without destroying the overall design. The system can therefore survive even when some functions leave the conversational context entirely.

### 3.3 Revised definition

The research therefore defines a **free region** as a logical processing region established through a combination of linguistic rules, scope, context, role, and current goal.

A conceptual expression is:

```text
FreeRegion
  = MetaRule
  + Scope
  + Context
  + Role
  + CurrentGoal
```

This is not a mathematical identity. It is a design abstraction.

The region does not need to be a fixed internal location. It exists operationally when the relevant conditions are active.

### 3.4 Meta-rules and boundaries

A representative meta-rule used in this research is:

> “Free here. Outside here, follow the existing rules.”

The purpose of this statement is not to override platform, legal, organizational, or safety rules. Its function is to define a boundary: within the designated region, hypothesis generation and reconstruction may be broad; when acting on external systems, the relevant external constraints must apply.

The central idea is therefore **boundary definition rather than unrestricted freedom**.

---

## 4. Hybrid-Language Approach

### 4.1 Motivation

Natural language is flexible but ambiguous. Formal languages are precise but require technical knowledge and explicit structure. Dialogic Language Theory combines the strengths of both.

The hybrid-language approach can be summarized as:

```text
Human
  ↓
Natural language
  ↓
AI interpretation
  ↓
Formalization when needed
  ↓
Python / JSON / SQL / API / file operations
  ↓
Execution
  ↓
Result
  ↓
Natural-language revision
```

### 4.2 Natural language as the upper layer

In this model, natural language is the human-facing upper layer. It expresses goals and meaning. The AI translates selected parts into lower-level formal structures.

For example, the request:

> “Write the user’s name and date into the company Excel template without changing its formatting.”

can be decomposed into file selection, template preservation, field mapping, write operations, and saving. The user does not need to write the implementation code for each step.

### 4.3 Formal languages as execution representations

Python, JSON, SQL, and API calls are not treated as competitors to natural language. They are execution representations selected when needed for stability or precision.

A practical division is:

- **natural language:** goals, exceptions, consultation, role design, flexible reasoning;
- **formal code:** repeated operations, exact data manipulation, persistence, file handling, external service integration.

### 4.4 AI as translation layer

The AI becomes a translation and coordination layer between human meaning and machine execution. This is why the framework is better described as a **hybrid-language system** than as natural-language-only execution.

However, from the human authoring perspective, the system can still be developed primarily through natural language: the formal code may be generated by the AI rather than directly written by the user.

---

## 5. NAVI as an Implementation Model

### 5.1 Position of NAVI

NAVI is not identical to Dialogic Language Theory. It is an implementation model derived from the theory.

Its central design principle is that NAVI is not a universal expert that performs every task itself. NAVI acts as a reception, routing, coordination, and handoff layer.

```text
User
  ↓
NAVI
  ↓
Requirement interpretation
  ↓
Agent / Robot / Database / External Service
  ↓
Result integration
  ↓
User
```

### 5.2 NAVI Core

The NAVI Core concept handles state such as:

- environment;
- scope;
- context;
- current task;
- available functions;
- external records.

It is separated conceptually from the conversational identity of NAVI.

### 5.3 Agents and robots

The system distinguishes between **agents** and **robots**.

Agents perform flexible interpretation, analysis, or role-based reasoning.

Robots perform deterministic or mechanically constrained actions.

Examples include:

- research agent;
- analysis agent;
- counterargument agent;
- Excel writing robot;
- document writing robot;
- database robot.

This separation reduces the need to make one component simultaneously interpret meaning and perform every external operation.

### 5.4 External memory

Important state does not have to remain inside one AI conversation. Project state, rules, decisions, and work records can be stored externally and selectively restored.

This supports a long-term goal of reducing dependence on a single AI platform.

### 5.5 External free region

The “external free region” is an execution space in which reusable robots and connected systems can wait for requests. It is not defined as an unrestricted environment. Each external tool remains subject to its own permissions and rules.

