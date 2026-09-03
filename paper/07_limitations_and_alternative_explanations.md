# 7. Limitations and Alternative Explanations

## 7.1 Ordinary Instruction-Following

The most immediate alternative explanation for the pilot results is ordinary instruction-following. An LLM may produce the expected INSIDE/OUTSIDE responses simply because the relevant instruction is present in the conversational context, without requiring any additional concept corresponding to a structured internal space.

This explanation is particularly important because the preliminary experiments did not show a performance advantage for explicit CIS-style region framing over the ordinary rule-list condition. In the simple switching and independently replicated Rule Isolation tasks, C1 and C3 performed equivalently. The current evidence therefore cannot distinguish a CIS-specific effect from sufficiently capable contextual instruction-following.

Future experiments must test behaviors for which scope structure makes additional predictions, such as nested scopes, local modification, restoration of prior state, and controlled rule shadowing.

## 7.2 Conversational State and Recency Effects

Observed persistence may also be explained by ordinary conversational state or recency. After a context such as INSIDE has been declared, the model may continue producing the associated response because the declaration remains recent and salient in the conversation history.

The current persistence pilots do not establish that a distinct boundary representation is required. Experiments should therefore vary conversational distance, introduce controlled distractors, compare explicit and implicit state restoration, and use fresh conversations where appropriate.

## 7.3 Prompt Wording and Semantic Equivalence

The initial pilots used deliberately simple and highly explicit rule formulations. Successful behavior under one wording does not establish robustness to natural-language variation. A rule framework that depends on a specific phrase, capitalization pattern, token, or instruction order would provide much weaker evidence for platform-independent construction.

Future tests should therefore use semantically equivalent paraphrases, reordered declarations, alternative boundary labels, and matched controls. The relevant question is whether the tested function survives reasonable changes in expression while preserving the intended meaning.

## 7.4 Generalizability Across an Open-Ended AI Ecosystem

The contemporary AI ecosystem contains a large and continually changing number of commercial systems, open-weight models, locally deployed models, fine-tuned variants, interface-specific implementations, and model configurations. Exhaustively testing every AI system is not practically possible, and the inclusion of locally deployed and independently modified systems makes the population effectively open-ended.

Accordingly, this study does **not** claim that the observed behavior is universal across all AI systems. The relevant observation is narrower: functionally similar responses have been observed in multiple distinct AI environments, providing a basis for investigating the conditions under which such convergence occurs.

The research question should therefore not be interpreted as “Can every AI system exhibit the same behavior?” A more empirically useful formulation is: **Across which classes of AI systems, and under which conditions, do comparable natural-language rule functions emerge?**

Any future generalization must be bounded by the models, versions, platforms, configurations, and experimental conditions actually tested. Additional platforms—including local models—can extend the evidence base, but no finite sample can demonstrate universality across an indefinitely expanding AI ecosystem.

## 7.5 Model, Version, and Platform Confounds

A platform comparison is not necessarily a controlled model comparison. Commercial AI products may differ in underlying model families, model versions, system instructions, context management, safety layers, interface behavior, memory systems, tool integrations, and other components that are not visible to the researcher.

Consequently, an observed difference between two named platforms cannot automatically be attributed to the underlying language model itself. Results should record the accessible platform and version information available at the time of testing and avoid unsupported claims about hidden causes.

This limitation also means that replication over time is important. A platform may change while retaining the same public product name, and a previously observed behavior may therefore change without any modification to the experimental prompt.

## 7.6 Limits of Inferring Internal Mechanisms

Observable responses do not directly reveal the internal computational mechanism that produced them. If an AI describes an “internal space,” “layer,” “agent,” “boundary,” or similar structure, that generated description is not sufficient evidence that a corresponding physical, neural, or software structure exists inside the model.

For this reason, CIS is used in this paper as an **operational concept for describing and testing observable context-dependent behavior**. The current experiments do not demonstrate a distinct neural space, a shared hidden architecture across models, or a specific internal mechanism by which natural-language rules are represented.

Mechanistic claims would require different forms of evidence, potentially including controlled access to model internals, interpretability methods, or experiments specifically designed to discriminate among competing internal explanations. Such evidence is outside the scope of the present exploratory study.

## 7.7 Implications of the Limitations

These limitations do not invalidate the research question; they define the experiments required to distinguish the hypothesis from simpler explanations.

The present evidence supports continued investigation of a bounded question: whether functionally comparable rule behavior can be reproduced across multiple heterogeneous AI environments under controlled natural-language specifications. Negative results, platform-specific failures, and conditions under which convergence disappears are therefore as important as successful replications.

The goal is not to demonstrate universality by assumption, but to progressively identify the **scope conditions** of cross-platform functional convergence.

---

## Open Research Note

The limitations in this chapter are part of the research result, not exceptions to it. Future tests should refine the domain of the hypothesis rather than assume that all AI systems must behave alike.

**Next:** Open Research and Reproducibility.
