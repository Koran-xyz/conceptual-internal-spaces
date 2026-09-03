# Adjacent Fields and the Novelty Boundary

**Status:** Working related-work analysis  
**Paper:** Dialogic Construction Methodology  
**Purpose:** Stress-test the proposed methodology against adjacent research before making novelty claims.

## 1. Result of the Second-Pass Search

A broader comparison substantially narrows what can responsibly be claimed as distinctive.

The following ideas are **not sufficient novelty claims** on their own:

- humans and AI iteratively creating something together;
- humans framing goals while AI generates alternatives;
- humans retaining final decision authority;
- AI critiquing, evaluating, or refining human proposals;
- natural language being used to specify system requirements;
- iterative requirements elicitation with LLMs;
- natural-language end-user programming;
- participatory or value-sensitive design of AI systems;
- maintaining traceability from requirements or constraints to later artifacts;
- multiple AI agents collaborating on requirements or system design.

All of these have meaningful precedents in adjacent fields.

## 2. Human–AI Co-Design and Co-Creation

Recent human–AI co-creation frameworks explicitly model iterative interaction between a human, AI, instructions, and an evolving artifact. Other work describes proposal–critique–revision cycles, human control, and AI as co-generator, co-evaluator, or co-explorer.

Therefore, **iteration and mutual contribution are background conditions, not the main novelty claim**.

Relevant examples include Ren, Ma, and Luo (2026), Kadenhe et al. (2025), and the broader conceptual-design literature.

## 3. Participatory and Value-Sensitive Design

Participatory design and value-sensitive approaches already place human or community values at the center of system design. Recent work extends these ideas directly to AI development and governance.

Therefore, **"humans define values and AI should serve them" is also not enough to distinguish the method**.

The present methodology should instead state more narrowly that the human supplies the problem and governing objective for a particular construction trajectory, while AI proposals remain subordinate to that objective and to external safety constraints.

## 4. Requirements Engineering

Requirements Engineering (RE) is a particularly close neighboring field.

LLMs are already used for:

- eliciting requirements;
- generating and reformulating requirements;
- detecting ambiguity;
- validating requirements;
- converting stakeholder needs into structured artifacts;
- iterative human–LLM requirements analysis;
- multi-agent elicitation, modeling, verification, and specification.

Some recent frameworks explicitly retain human oversight and iterative refinement. Requirements traceability also provides mature precedents for tracking how constraints propagate through later design artifacts.

This means the proposed methodology **cannot claim to have invented conversational rule elicitation, human validation, iterative specification, or traceability**.

## 5. End-User Programming and Natural-Language Programming

LLMs increasingly allow non-programmers to describe desired behavior in natural language and obtain executable or reusable systems. Research has studied how humans communicate programming tasks to LLMs and how complex prompts can function as reusable application specifications.

Therefore, **"natural language can construct system behavior" is not itself a sufficient novelty claim**.

The distinction must lie elsewhere.

## 6. The Remaining Candidate Boundary

After removing the overlapping claims above, a narrower candidate remains worth investigating:

> **The object of study is the trajectory by which a human-defined problem is progressively transformed, through human–AI dialogue, into an adopted and revisable rule or structural configuration, with explicit records of proposal origin, reasoning, acceptance, rejection, replacement, reuse, and observed consequences.**

The emphasis is not merely on the final artifact or requirement document. It is on the **construction trajectory itself** as a research object.

A candidate trajectory record is:

1. Human-defined problem.
2. Human-defined objective and non-negotiable constraints.
3. Candidate proposal from human or AI.
4. AI-side critique of coherence, feasibility, efficiency, conflicts, and expected operational behavior.
5. Human-side judgment of objective alignment, acceptability, safety, and value fit.
6. Decision: adopt, revise, reject, defer, replace, or reuse.
7. Resulting rule or structural change.
8. Observable consequence.
9. New problem or discrepancy.
10. Next dialogue cycle.

This is currently a **candidate research boundary**, not a confirmed novelty claim.

## 7. Two-Axis Acceptance

A central distinction proposed for the methodology is that acceptance should not be reduced to either human preference or AI agreement.

A candidate should be examined on at least two separate axes:

### Human-objective alignment
Does the proposal actually serve the problem, objective, values, safety requirements, and constraints defined by the human?

### Operational reasonableness
Given the observable capabilities and constraints of the AI environment, is the proposal coherent, interpretable, feasible, and unlikely to create contradictions with the intended construction?

AI agreement alone does not establish operational reasonableness. Human preference alone does not establish feasibility.

The method therefore rejects the inference:

**"The AI approved it, therefore it is correct."**

It also rejects:

**"The human wants it, therefore the AI system can reliably realize it."**

The research question is whether dialogue can help expose and reduce the gap between these two axes.

## 8. Human Governance Boundary

The methodology is human-initiated and human-governed:

- the human defines the problem;
- the human defines the intended objective;
- either human or AI may propose candidate solutions;
- AI may critique or identify conflicts;
- the human retains authority over adoption within applicable external rules and safety constraints.

This prevents the method from being interpreted as selecting whatever is "best for the AI." A proposal that benefits an AI-defined objective but conflicts with the human-defined legitimate objective is not a successful result of the method.

At the same time, the human should not treat AI objections as commands. They are information to be examined. The method requires reasons and observable consequences wherever possible.

## 9. Construction Trajectory vs Requirements Traceability

This distinction needs special care because Requirements Engineering already studies traceability.

Traditional requirements traceability often asks how a requirement connects to design, implementation, testing, or later artifacts.

The proposed **construction trajectory** instead asks how the rule or structure itself emerged through dialogue before and during implementation:

**problem → proposal → critique → decision → structural change → observation → revision**.

The two ideas may overlap. Future literature review must determine whether this trajectory is genuinely under-modeled in existing RE, co-design, or interactive-programming research.

Therefore the paper should not claim novelty here until that comparison is complete.

## 10. A More Defensible Research Question

A stronger RQ candidate is:

> **RQ1: Can human–AI construction trajectories be represented and evaluated as reproducible records of how human-defined problems are transformed into adopted, revised, rejected, or replaced natural-language rules and structures?**

A second question can test the acceptance mechanism:

> **RQ2: Does explicitly separating human-objective alignment from operational reasonableness improve the transparency and reproducibility of decisions made during human–AI rule and structure construction?**

A third question can address outcomes without assuming superiority:

> **RQ3: Under what conditions does a recorded dialogic construction process produce rules or structures that remain understandable, revisable, and testable by another researcher?**

## 11. What Would Falsify or Weaken the Contribution?

The proposed contribution becomes weak or redundant if literature review shows that an existing methodology already provides, as its central object:

- human-defined problem framing;
- bilateral human/AI proposal and critique;
- separate evaluation of human objective alignment and AI-operational feasibility;
- human-governed adoption;
- explicit state transitions among adoption, revision, rejection, replacement, and reuse;
- trajectory-level provenance from problem through observed structural consequences;
- reproducibility by another researcher from the trajectory record.

If such a framework already exists, the correct response is to position this work as an application, extension, or empirical comparison rather than rename an existing idea.

## 12. Current Position

The second-pass comparison suggests that the broad philosophy of the method belongs within established human–AI collaboration, co-design, requirements engineering, and natural-language programming research.

The potentially distinctive contribution is narrower:

> **treating the human–AI construction trajectory itself as a first-class, reproducible research artifact for rule and structure formation, while separating human-governed objectives from claims of AI-side operational reasonableness.**

This remains a hypothesis about research positioning. It must survive deeper literature review and empirical case reconstruction before being presented as a novel methodology.

## Selected Sources for the Next Citation Pass

- Ren, R., Ma, J., & Luo, J. (2026). *Human-AI co-creation: why, what, and how?* Proceedings of the Design Society.
- Kadenhe, N., Al Musleh, M., & Lompot, A. (2025). *Human-AI Co-Design and Co-Creation: A Review of Emerging Approaches, Challenges, and Future Directions.* Proceedings of the AAAI Symposium Series.
- Fang, C., et al. (2025). *Generative AI-enhanced human-AI collaborative conceptual design: A systematic literature review.* Design Studies, 97, 101300.
- Jin, D., Jin, Z., Chen, X., & Wang, C. (2024). *MARE: Multi-Agents Collaboration Framework for Requirements Engineering.* arXiv:2405.03256.
- Norheim, J. J., Kerbrat, A., & de Weck, O. L. (2024). *Challenges in applying large language models to requirements engineering tasks.* Design Science.
- Park, H., et al. (2025). *How Humans Communicate Programming Tasks in Natural Language and Implications for End-User Programming with LLMs.* CHI 2025.
- Sarkar, A., et al. (2022). *What is it like to program with artificial intelligence?* PPIG 2022.
- Mahajan, S., & Helbing, D. (2026). *Co-designing AI systems with value-sensitive citizen science.* AI & Society.

**Citation status:** source records were identified in the 2026-09-03 comparison pass. Bibliographic details and claims should receive a dedicated citation audit before submission.