# Paper 2 — Rule Discovery and Final Novelty Boundary

Status: Working positioning note; novelty candidate, not a priority or world-first claim.

## 1. Question examined

How much prior work already covers the case where a human begins with a problem or objective, but the rules or structures needed to solve it are not yet known, and human–AI dialogue is used to develop them?

This note compares the Dialogic Language Theory / dialogic construction program with adjacent work in human–AI conceptual design, interactive machine teaching, value elicitation, design science, and human-authorship frameworks.

## 2. What prior work already covers

### 2.1 Human–AI conceptual design

Recent design research already studies iterative human–AI ideation. Generative AI can contribute to problem definition and idea generation, while selection and evaluation remain substantially human-led. Therefore, neither iterative ideation nor human final judgment is unique to this program.

### 2.2 Human-led goals and ethical judgment

Recent reviews of AI across design thinking recommend that domain experts retain responsibility for goals, constraints, evaluation criteria, and ethical decisions while AI supports exploration. Therefore, the claim that humans should govern objectives and final decisions is important but not itself novel.

### 2.3 Interactive machine teaching

Interactive machine teaching includes cycles in which a system generates candidate rules and queries a human expert for feedback on rules and instances. Thus, interaction around candidate rules already exists in the literature. However, its typical objective is teaching or improving a model/task learner, rather than constructing an evolving operational rule/structure for the human–AI working environment itself.

### 2.4 Human-value elicitation

LLMs have been proposed as tools to help identify and analyze stakeholder values while retaining human judgment. Therefore, using dialogue or LLM assistance to surface values is also not unique.

### 2.5 Design science and iterative artifact construction

Design science already provides iterative build–evaluate–refine cycles for artifacts. Generative AI has also been used as a design/development partner through continuous conversation. Therefore, iterative construction and evaluation alone cannot define the novelty boundary.

### 2.6 Human authorship frameworks

Recent human–AI co-creation frameworks explicitly preserve human framing, refinement, and commitment. These overlap strongly with the principle that humans retain accountable adoption authority.

## 3. What must NOT be claimed as novelty

Paper 2 should not claim novelty for any of the following in isolation:

- humans and AI can collaborate;
- dialogue can improve a solution;
- AI can generate alternatives;
- humans can retain final judgment;
- natural language can specify rules;
- humans and AI can iteratively refine artifacts;
- LLMs can help elicit human values;
- candidate rules can be reviewed interactively;
- design decisions can be traced.

These ideas have substantial prior art.

## 4. Candidate remaining boundary

The remaining candidate contribution is a particular combination and research object:

> A human begins by defining a practical problem and intended objective, without requiring the final rule or system structure to be known in advance. Through natural-language dialogue, the human and AI generate and evaluate candidate rules or structures. The human retains adoption authority, while AI-side reasoning is used to test operational coherence, feasibility, contradictions, and efficiency. Adopted structures are then used in an AI environment, their observable consequences are recorded, and those observations are returned to the next dialogue cycle. The evolving sequence is studied as a construction trajectory rather than merely as a final artifact or conversation transcript.

This boundary is deliberately narrower than “human–AI co-creation.”

## 5. Human-defined problem structure

The current method assigns different responsibilities:

### Human responsibility
- define the initial problem;
- define or clarify the intended objective;
- specify non-negotiable human values and safety constraints where applicable;
- decide whether a proposal is adopted, rejected, revised, suspended, replaced, or reused;
- remain accountable for the resulting use.

### AI contribution
- analyze the stated problem;
- identify contradictions, missing conditions, and implementation difficulties;
- propose candidate solutions or structural modifications;
- compare alternatives for coherence and efficiency;
- explain why a candidate may or may not work in the relevant AI environment.

The AI's approval is not treated as evidence that a proposal is ethically correct or beneficial. “Operationally reasonable for the AI environment” is distinct from “advantageous to the AI.”

## 6. Dual evaluation

A candidate rule or structure should be evaluated along at least two separate dimensions.

### Human-objective fit
Does the proposal remain consistent with the human-defined purpose, values, safety conditions, and intended outcome?

### Operational coherence
Can the proposal be represented and used coherently in the target AI environment, without obvious contradiction or unnecessary structural cost?

Neither dimension substitutes for the other.

A proposal that is easy for an AI to follow but violates the human objective fails. A proposal that expresses a desirable human goal but cannot function coherently in the target environment also requires revision rather than forced adoption.

## 7. Rule discovery rather than rule translation

A useful distinction for Paper 2 is:

**Rule translation:** a desired rule is already known and natural language is used to express, formalize, compile, or enforce it.

**Rule discovery/construction:** the problem is known, but the appropriate rule or structure is not yet known; dialogue is used to discover candidate solutions, evaluate them, deploy selected candidates, observe effects, and revise the structure.

Dialogic Language Theory is currently positioned primarily in the second category.

This does not establish that no prior method performs rule discovery. It defines the comparison target for a more exhaustive literature review.

## 8. Construction trajectory as the unit of analysis

A proposed trajectory record is:

1. Human-defined problem
2. Intended objective
3. Constraints / safety conditions
4. Candidate proposal
5. Proposal origin: human / AI / jointly developed
6. Reasoning and objections
7. Human decision: adopt / revise / reject / suspend / replace / reuse
8. Implemented rule or structure
9. Target AI environment
10. Observable result
11. Failure, side effect, or new problem
12. Next dialogue cycle

The trajectory is therefore not only decision traceability. It connects dialogue, decision, implementation, observation, and subsequent reconstruction.

## 9. Candidate research questions

### RQ1
Under what conditions can human-initiated natural-language dialogue function as a reproducible method for discovering, constructing, and revising operational rules or structures when the solution is not fully specified in advance?

### RQ2
How do human-proposed, AI-proposed, and jointly developed candidates differ in their paths through evaluation, adoption, rejection, revision, replacement, and reuse?

### RQ3
How does feedback from the observable behavior of an implemented rule or structure alter subsequent dialogue and reconstruction decisions?

RQ3 creates the clearest separation from a purely conversational or ideation framework, because the method explicitly closes the loop from dialogue to implementation to observation and back to dialogue.

## 10. Candidate contribution statement

A cautious contribution statement is:

> This work proposes a human-governed dialogic construction methodology for studying how initially underspecified practical problems can be transformed into operational rules and adaptive structures through iterative human–AI natural-language interaction. Its proposed unit of analysis is the construction trajectory linking problem definition, candidate generation, human-governed adoption decisions, implementation, observable consequences, and subsequent reconstruction.

This is a proposed methodological contribution. It is not yet a demonstrated universal method.

## 11. Relationship to the wider research program

Paper 2 studies **how structures are constructed and reconstructed**.

Paper 1 studies whether some natural-language-constructed rule functions can be observed and compared across LLM environments.

Later papers can study where those structures should reside (internal/external/hybrid), whether persistent safety functions are better realized as agents or layers, and how heterogeneous AI systems coordinate through shared workspaces.

Thus Paper 2 should not absorb the empirical claims of the other papers. It provides the methodological trunk from which those studies emerged.

## 12. Current novelty status

**Not established as unique or world-first.**

The literature reviewed so far creates substantial overlap with human–AI co-design, mixed-initiative interaction, design science, interactive machine teaching, value elicitation, human-authorship frameworks, natural-language programming, policy authoring, requirements engineering, and design rationale.

The defensible candidate boundary is therefore the integrated method and its unit of analysis, especially:

- human-originated problem framing;
- solution/rule/structure not necessarily specified in advance;
- candidate generation by human, AI, or both;
- explicit separation of human-objective fit from AI-environment operational coherence;
- human-governed adoption authority;
- deployment of the selected natural-language rule/structure;
- observation of resulting behavior;
- return of observations into the next construction cycle;
- construction trajectory as the reproducible record of that evolution.

The next scholarly step is not to broaden this claim, but to test whether this exact combination has already been formalized under another name.

## 13. Sources checked in this comparison

- Chen et al. (2025), *How generative AI supports human in conceptual design*, Design Science.
- Recent qualitative review of AI across design thinking (2026), Design Science.
- *Interactive Machine Teaching by Labeling Rules and Instances*, TACL / MIT Press.
- Herrmann, Mircea & Schneider (2025), *Aligning AI Systems with Human Values*.
- Recent Design Science / human–AI co-creation work on iterative design and human judgment.
- Jacob et al. (2026), *Operationalizing Human Authorship in AI Systems: A Design Science Study of the FERC Framework*.

Exact bibliographic formatting and a broader systematic search remain pending before submission.
