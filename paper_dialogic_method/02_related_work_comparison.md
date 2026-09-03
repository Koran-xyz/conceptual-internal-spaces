# Related-Work Comparison — Dialogic Construction Methodology

**Status:** Working literature-positioning note  
**Date:** 2026-09-03

## Purpose

This note tests whether the proposed **Dialogic Construction Methodology (DCM)** is merely a renaming of established Human–AI collaboration paradigms. The comparison deliberately treats overlap as expected and narrows the proposed contribution rather than claiming novelty for generic dialogue or co-creation.

## 1. Mixed-Initiative Interaction

Horvitz (1999) described mixed-initiative interaction as a flexible strategy in which human and computational agents contribute according to their respective strengths. Later Human–AI work extends this idea to dynamic initiative switching, negotiation of roles, and shared control.

**Overlap with DCM**
- Human and AI can both contribute proposals.
- Interaction can be iterative rather than one-shot.
- Different capabilities of human and AI can be used complementarily.

**Difference currently worth testing**
- DCM does not require symmetrical control over the problem definition.
- The human defines the problem and intended objective.
- AI initiative is primarily used within the solution-construction process.
- The central artifact can be a rule, procedure, role structure, or system organization rather than only a task action or decision.

**Conclusion:** Mixed initiative is an important predecessor, not a novelty claim for DCM.

## 2. Human–AI Co-Creation

Recent Human–AI co-creation research models iterative cycles of proposal, critique, revision, instruction, interaction, and artifact production. Ren, Ma, and Luo (2026), for example, describe a framework containing Human, AI, Artifact, Instruction, and Interaction. Other design research examines iterative GenAI communication during professional concept development.

**Overlap with DCM**
- Iterative proposal, critique, and revision.
- AI as an active contributor rather than a passive output generator.
- Human evaluation remains important.
- Dialogue can change the resulting artifact.

**Difference currently worth testing**
- DCM specifically treats **rules and adaptive system structures as primary constructed artifacts**.
- The objective is not limited to creative artifact quality or ideation.
- DCM asks whether the dialogue process can produce structures that subsequently organize AI behavior and future interaction.

**Conclusion:** "Humans and AI create something together" is not sufficient novelty.

## 3. Human-in-the-Loop and Human-Driven AI Development

Human-in-the-loop approaches commonly preserve human intent, evaluation, and intervention while AI performs generative or analytical work. Recent reviews of design systems describe cycles in which a human defines intent, reviews AI output, and gives further instructions. Human-centered frameworks also emphasize maintaining human decision authority.

**Overlap with DCM**
- Human objectives and judgment remain central.
- AI output is evaluated rather than accepted automatically.
- Iterative correction is expected.

**Difference currently worth testing**
- DCM is not only a checkpoint architecture for supervising AI output.
- The interaction itself is treated as a construction process capable of changing the rules or structure through which later work is organized.
- Human authority over the objective is separated from AI participation in reasoning about implementation.

**Conclusion:** Human governance is a design requirement of DCM, not by itself a novel contribution.

## 4. Interactive Machine Teaching / Interactive Machine Learning

Interactive machine teaching and learning use repeated human interaction to shape machine behavior, often through labels, demonstrations, constraints, feedback, or model correction. Some work explicitly aims to make AI creation more interactive and understandable to end users.

**Overlap with DCM**
- Iterative feedback loop.
- Human intervention can alter future system behavior.
- Interaction can expose useful information about system behavior.

**Difference currently worth testing**
- DCM does not require model training, weight updates, or a formal learning algorithm.
- Candidate rules and structures may exist at the natural-language interaction/context level.
- The AI also participates in reasoning about the candidate structure rather than merely being the object being taught.

**Conclusion:** DCM should not be described as a replacement for machine teaching; it investigates a different construction layer.

## 5. Coactive / Co-Adaptive Human–AI Systems

Coactive and co-adaptive research emphasizes interdependence, mutual adjustment, shared mental models, and systems in which humans and AI adapt to one another over time.

**Overlap with DCM**
- Mutual adjustment can occur.
- Neither participant needs to possess the entire solution in advance.
- Interaction history can affect later behavior.

**Difference currently worth testing**
- DCM intentionally keeps the **human-defined problem and objective** as a governance anchor.
- Mutual adaptation is not an unrestricted objective: an AI-favored change is not accepted merely because it improves convenience for the AI.
- Candidate changes must be judged against the human-defined objective as well as operational coherence.

**Conclusion:** Mutual adaptation is useful, but DCM needs an explicit asymmetric governance boundary.

## 6. AI Principles and Constitutions

Natural-language principles are already used in AI safety and governance. Constitutional approaches demonstrate that written principles can guide AI behavior and evaluation. Current constitutions can also be developed with contributions from both humans and AI systems.

**Overlap with DCM**
- Natural language can express behavioral principles.
- Principles can be discussed, revised, and evaluated.
- Human and AI contributions can both appear during development.

**Difference currently worth testing**
- DCM is a general construction method, not one predefined constitution or training pipeline.
- It focuses on the dialogue process through which a specific human-defined problem is translated into candidate rules or structures.
- It can be studied at runtime/context level without claiming that dialogue changes model weights or internal mechanisms.

**Conclusion:** The existence of natural-language constitutions means DCM cannot claim novelty simply for expressing AI rules in language.

## 7. Narrowed Candidate Contribution

After removing the overlapping claims, the strongest current candidate contribution is:

> **A human-governed dialogic construction method in which the human defines the problem and objective, while human and AI jointly reason about candidate natural-language rules or structures; candidates are iteratively adopted, revised, rejected, replaced, or reused according to their consistency with the human-defined objective and their operational coherence in the AI environment.**

The distinctive research object is therefore not **dialogue itself**, **AI collaboration itself**, **human oversight itself**, or **natural-language rules themselves**.

The proposed research object is the **construction trajectory of rules and adaptive structures through governed dialogue**.

## 8. Proposed Analytical Unit: Construction Trajectory

To make the idea empirically distinguishable from generic co-creation, future case studies should record a construction trajectory such as:

1. Human-defined problem.
2. Human-defined objective or constraints.
3. Initial candidate proposed by human or AI.
4. AI evaluation/reasoning about the candidate.
5. Human evaluation of the candidate against the objective.
6. Revision, rejection, adoption, replacement, or reuse.
7. Resulting rule or structure.
8. Observable consequence.
9. New problem produced by that consequence.

This makes the process traceable rather than describing successful structures only after the fact.

## 9. Failure Conditions

DCM should be considered unsuccessful or compromised when, for example:

- the human objective becomes unclear or silently changes;
- AI agreement is mistaken for evidence of correctness;
- a proposal is accepted only because it is convenient for the AI;
- the human accepts recommendations without meaningful evaluation;
- the AI merely mirrors the user's preference rather than identifying contradictions or alternatives;
- an apparently successful structure cannot be connected to a traceable construction trajectory;
- later observations contradict the reason the structure was adopted and the method does not permit revision.

These failure conditions are important because they distinguish governed dialogue from simple agreement.

## 10. Revised Research Questions

**RQ1.** Under what conditions can human-initiated natural-language dialogue function as a traceable and reproducible method for constructing and revising rules or adaptive structures?

**RQ2.** How do proposal origin, critique, revision, rejection, and human adoption decisions shape the resulting rule or structure?

**RQ3.** Can the construction trajectory distinguish jointly reasoned rule construction from ordinary prompting, simple iterative refinement, or uncritical AI agreement?

**RQ4.** Which parts of the method remain stable when the resulting implementation changes across AI environments or tasks?

## 11. Current Position

The literature comparison does **not** yet establish that DCM is a novel methodology. It establishes a narrower area that is not adequately described by claiming only "human and AI collaborate through dialogue."

The next scholarly task is to test this narrowed formulation against additional literature on co-design, participatory design, end-user programming, conversational programming, requirements engineering, value-sensitive design, and AI-assisted rule or policy authoring.

Only after that comparison should the paper make a formal novelty claim.

## References checked in this pass

- Horvitz, E. (1999). *Mixed-Initiative Interaction*. IEEE Intelligent Systems.
- Holter et al. (2024). *Deconstructing Human-AI Collaboration: Agency, Interaction, and Adaptation*. Computer Graphics Forum.
- Methnani, L., Dahlgren Lindström, A., & Dignum, V. (2024). *The Impact of Mixed-Initiative on Collaboration in Hybrid AI*.
- Liu, Z. (2025). *Human-AI Co-Creation: A Framework for Collaborative Design in Intelligent Systems*.
- Hu et al. (2025). *Human at the Center: A Framework for Human-Driven AI Development*. AI Magazine.
- Ren, R., Ma, J., & Luo, J. (2026). *Human-AI co-creation: why, what, and how?* Proceedings of the Design Society.
- Inkermann, D. (2026). *Rethinking design methods in the age of AI – consequences for practice, education, and research*. Proceedings of the Design Society.
- Cavallin, E., & Spagnol, S. (2026). *When Designers Sweat: Behavioral Traces of GenAI Co-Creation*. CHI 2026.

This is a working comparison, not a final systematic literature review.