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

This research uses a compact upper-level boundary rule that distinguishes exploratory reasoning from externally constrained action. The exact operational wording is intentionally omitted from the public paper. Its function is not to override platform, legal, organizational, or safety rules, but to define when exploratory analysis is permitted and when external constraints must govern behavior.

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


## 6. Early Implementation Experiments

### 6.1 Experimental pattern

The early experiments followed a repeated pattern:

1. the human described a desired function in natural language;
2. the AI interpreted the request;
3. the AI generated or selected formal operations;
4. the operation was executed;
5. the result was inspected;
6. further changes were requested in natural language.

The user’s direct input was therefore primarily natural-language design and correction rather than hand-written implementation code.

### 6.2 Excel writing

A natural-language requirement to create an Excel writing robot was decomposed into file opening, sheet selection, cell mapping, value writing, and saving.

The design later evolved to externalize field-to-cell mappings, for example:

```text
Name → B3
Date → D3
Work description → B6
```

This makes the mechanical operation reusable while allowing the conversational layer to decide what information belongs in each field.

### 6.3 Google Sheets

A cloud test created a Google Sheet, wrote a test string into a cell, then read the same cell back. This demonstrated a complete path from conversational instruction to modification of cloud-hosted data and verification of the result.

### 6.4 Microsoft Excel and OneDrive

Excel files were generated and uploaded to Microsoft OneDrive. This demonstrated that a natural-language-driven workflow could extend beyond local files into cloud storage.

For rigorous publication, repeated same-file update tests should be logged with pre-value, requested change, resulting value, and read-back verification.

### 6.5 Word documents

A natural-language request was used to generate a `.docx` document containing a specified test phrase. This confirmed the path from natural-language instruction to Word-file generation.

The experiment also led to an architectural simplification: Word, PDF, Markdown, and text output may be grouped under a generalized document-writing robot, while Excel remains more specialized because of its workbook, sheet, cell, and formula structure.

### 6.6 Converting linguistic functions into Python

Functions that had originally been described only in language—such as state storage, registration, file writing, and repeated transformations—were selectively converted into Python-based processing.

The theoretical framework remained intact after this conversion. This supported the interpretation that Python was not the theory itself, but one possible formalization of functions discovered or specified through dialogue.

---

## 7. Evaluation Plan

The current implementation results are preliminary. The next stage is controlled comparison.

### 7.1 Comparison conditions

A useful evaluation set is:

| Condition | System form |
|---|---|
| A | single ordinary prompt |
| B | iterative natural-language construction |
| C | iterative construction + explicit meta-rule/free region |
| D | natural-language coordination + fixed Python execution |
| E | full NAVI-style hybrid system with agents, robots, and external memory |

### 7.2 Evaluation dimensions

The following measures are proposed:

- task success rate;
- reproducibility across repeated runs;
- number of corrections;
- execution errors;
- amount of user-authored code;
- amount of natural-language interaction;
- latency and token use;
- portability between AI platforms;
- incorrect external actions;
- recovery after a model change or context reset.

### 7.3 Meta-rule test

The effect of meta-rules should be tested directly rather than assumed. Identical tasks can be run with and without a boundary rule. The experiment should test whether a short upper-level rule measurably changes consistency between exploratory reasoning and constrained external execution.

### 7.4 Natural-language versus fixed execution

The same repeated task, such as writing to a known Excel template, can be implemented in two forms:

- re-interpret the operation in natural language every time;
- interpret the user’s intent but call a fixed, validated write function.

This comparison can test the hypothesis that natural language is better for flexible interpretation while fixed code is better for repeatability.

### 7.5 Model portability

The same role definitions, meta-rules, external records, and task state can be reconstructed on multiple AI platforms. The goal is not identical wording or identical hidden reasoning. The goal is functional reconstruction of the same role and workflow structure.

### 7.6 External memory test

Long-running tasks should be compared with and without external state. Measures should include retrieval accuracy, contamination from unrelated information, and ability to continue after changing AI models.

---

## 8. Relationship to Prior Work

This research overlaps with several established directions and does not claim that natural-language code generation itself is novel.

### 8.1 Language Model Programming and LMQL

Beurer-Kellner, Fischer, and Vechev proposed Language Model Programming and LMQL, combining text prompting, scripting, control flow, and output constraints. Their work demonstrates that prompting can be treated more systematically as programming.

Dialogic Language Theory differs in emphasis. It does not define one dedicated query language. Instead, it treats natural language as the persistent human-facing layer while allowing the AI to select among multiple formal representations underneath.

### 8.2 DSPy

DSPy represents language-model pipelines as declarative modules and computational graphs and compiles them into optimized LM pipelines.

The present research shares the move away from large hand-written prompt strings. Its distinct research question is whether a non-programmer can form and modify the higher-level system structure itself primarily through dialogue, with formal implementation generated or modified beneath that layer.

### 8.3 AutoGen and multi-agent systems

AutoGen provides a framework for composing conversable agents that can use LLMs, human input, and tools. This is closely related to NAVI’s agent structure.

However, multi-agent coordination is only one component of Dialogic Language Theory. The theory also applies to single-model role structures, external memory, formalization, and human-guided system redesign.

### 8.4 Tool use

Toolformer showed that language models can learn when and how to call external tools through APIs. NAVI similarly treats tools as external capabilities.

The implementation emphasis here is role separation: AI interprets meaning and selects actions, while deterministic robots perform constrained external operations.

### 8.5 Human-in-the-loop agentic systems

Magentic-UI and related work emphasize human oversight and collaboration in increasingly capable agentic systems. Dialogic Language Theory strongly aligns with this direction: asking the user is treated as a valid system operation rather than a failure.

### 8.6 No-code and low-code systems

No-code systems reduce the need to write source code by exposing visual components or configuration interfaces. The proposed approach goes one step further in interface abstraction: natural-language dialogue itself can become the design interface.

### 8.7 Novelty boundary

The individual ingredients of this research have substantial prior art. The research contribution should therefore be evaluated at the level of the combined model:

- iterative natural-language system formation;
- free-region generation through linguistic boundaries;
- selective conversion of flexible linguistic functions into fixed formal execution;
- separation of external state from the AI model;
- reconstruction across AI platforms;
- dialogue as the continuing design interface.

A systematic literature review is still required before making a strong novelty claim.

---

## 9. Limitations and Safety

### 9.1 Ambiguity

Natural language is ambiguous. Requests such as “organize this data” can imply sorting, summarization, deletion, restructuring, or export. External actions should not be triggered from unresolved ambiguity when materially different interpretations exist.

### 9.2 Separation of reasoning and action

A central safety rule is:

```text
Exploratory region:
  hypotheses, comparison, reconstruction may be flexible

External action region:
  use confirmed targets, permissions, and constraints
```

The ability to imagine an action should not automatically grant permission to execute it.

### 9.3 Consultation is part of the system

When information is missing, the system should return to the human rather than inventing a critical parameter.

```text
uncertainty
  ↓
material consequence?
  ↓ yes
ask the user
  ↓
update the working rule or configuration
```

### 9.4 Model variation

Different AI systems may interpret the same natural-language rule differently. Portability therefore means reconstructing equivalent functional roles and boundaries, not assuming identical behavior.

### 9.5 Least privilege

Robots should receive only the permissions required for their role. Reading, writing, deleting, sending, and financial or contractual actions should be treated as distinct capabilities.

### 9.6 Logging

Operational logs should record user request, selected function, target, action, success or failure, and relevant external result. The goal is operational traceability rather than storing hidden chain-of-thought.

### 9.7 Memory quality

External memory can preserve mistakes as well as correct facts. Persistent records should distinguish confirmed facts, hypotheses, temporary notes, and obsolete information, with source and update metadata when possible.

### 9.8 Controlled self-modification

A system that can change through dialogue should separate:

- user-editable preferences;
- automatically appendable history;
- protected core rules;
- permission settings requiring explicit human approval.

Flexible evolution must not mean uncontrolled mutation of the system’s safety and authority boundaries.

---

## 10. Future Directions

### 10.1 Evolving AI database

One application is an AI-mediated database that does not only store text but interprets new information, structures it, links it to existing entities, and retrieves relevant subsets through natural-language questions.

The long-term research question is whether the database can evolve its structure through dialogue while preserving traceability and consistency.

### 10.2 Enterprise AI deployment

The same architecture can be applied to enterprise deployment:

```text
Employee
  ↓ ordinary language
NAVI
  ↓
Company-specific agents / robots / databases
  ↓
Existing Excel, Word, cloud storage, and internal systems
```

Employees would not need to learn every underlying API or file-operation detail.

### 10.3 Domain-specific derivatives

A shared core could support specialized products such as AI-assisted POS analysis, company knowledge systems, personal assistants, or workflow systems.

The important architectural principle is reuse: the underlying language-driven coordination system remains shared while domain modules change.

### 10.4 Multi-AI environment

A future NAVI environment may treat AI models as replaceable or specialized inference components:

```text
Shared rules + shared state + shared tools
          ↓
  AI-A / AI-B / AI-C
```

The research goal is not to make all models identical, but to preserve the work structure when models change.

### 10.5 Natural-language-centered system development

A longer-term possibility is a development environment in which a user describes an organization or workflow in ordinary language, the AI proposes structures, formal components are generated, and the user continues to revise the running system through conversation.

This can be viewed as a step toward a natural-language-centered operating layer. The term “natural-language OS” is currently only a future analogy, not a demonstrated operating-system architecture.

---

## 11. Conclusion

This research began with a hypothesis that natural-language rules were constructing a persistent free space inside an AI. Continued implementation led to a more defensible interpretation.

The central research object is not an assumed hidden internal space. It is the **systemic behavior that can be formed through natural-language dialogue**.

Dialogic Language Theory therefore proposes that natural language can be used as a higher-level description layer for roles, rules, boundaries, relationships, and system changes. A logical free region can be generated by language, context, scope, and role without claiming that the model’s internal software architecture has been rewritten.

The hybrid-language approach extends this idea into executable systems. Human intent remains primarily in natural language; AI translates selected parts into formal representations such as Python, JSON, SQL, or API calls when precision, persistence, and repeatability are needed.

NAVI provides an implementation example in which conversational coordination, specialized agents, deterministic robots, external memory, and cloud services are separated but connected through a common natural-language interface.

The early implementation results demonstrate that this approach can move beyond text generation into file creation, structured-data writing, cloud operations, and formalized reusable processing. These results are initial demonstrations, not a proof of universal reliability.

The central future question is therefore:

> **Can humans form practical computer systems in their own language, while AI translates meaning into formal execution without removing human control?**

The current work suggests that this is a testable and potentially useful direction. Its value will ultimately depend on reproducibility, portability, safety, and controlled comparative evaluation.

---

## References

1. Beurer-Kellner, L., Fischer, M., & Vechev, M. (2022). *Prompting Is Programming: A Query Language for Large Language Models*. arXiv:2212.06094. https://arxiv.org/abs/2212.06094
2. Khattab, O., Singhvi, A., Maheshwari, P., Zhang, Z., Santhanam, K., Vardhamanan, S., Haq, S., Sharma, A., Joshi, T., Moazam, H., Miller, H., Zaharia, M., & Potts, C. (2024). *DSPy: Compiling Declarative Language Model Calls into State-of-the-Art Pipelines*. ICLR 2024. https://proceedings.iclr.cc/paper_files/paper/2024/hash/f1cf02ce09757f57c3b93c0db83181e0-Abstract-Conference.html
3. Wu, Q., Bansal, G., Zhang, J., Wu, Y., Li, B., Zhu, E., Jiang, L., Zhang, X., Zhang, S., Awadallah, A., White, R. W., Burger, D., & Wang, C. (2024). *AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation*. COLM 2024. https://www.microsoft.com/en-us/research/publication/autogen-enabling-next-gen-llm-applications-via-multi-agent-conversation-framework/
4. Schick, T., Dwivedi-Yu, J., Dessì, R., Raileanu, R., Lomeli, M., Zettlemoyer, L., Cancedda, N., & Scialom, T. (2023). *Toolformer: Language Models Can Teach Themselves to Use Tools*. arXiv:2302.04761. https://arxiv.org/abs/2302.04761
5. Mozannar, H., Bansal, G., Tan, C., Fourney, A., Dibia, V., Chen, J., et al. (2025). *Magentic-UI: Towards Human-in-the-loop Agentic Systems*. Microsoft Research Technical Report MSR-TR-2025-40. https://www.microsoft.com/en-us/research/publication/magentic-ui-report/

---

## Research Status

This document is a **working paper**. It intentionally distinguishes observed implementation results from theoretical interpretation. Claims about novelty, reproducibility, portability, and the measurable effect of meta-rules remain open to further controlled experiments.
