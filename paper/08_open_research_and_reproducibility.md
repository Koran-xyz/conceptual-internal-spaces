# 8. Open Research and Reproducibility

## 8.1 Open Research as Part of the Method

This project treats openness not only as a publication choice but as part of the research method. The questions examined here concern behavior that can vary across models, platforms, versions, interfaces, and time. A single researcher cannot exhaustively test the open-ended AI ecosystem described in Section 7.4. Independent replication, disagreement, negative results, and extensions are therefore necessary for evaluating the scope of the hypothesis.

The public research record is intended to expose the development of the work rather than only its final conclusions. Hypotheses may be published before definitive validation, provided that their evidential status is clearly labeled and that observations, interpretations, and established results are not presented as equivalent.

## 8.2 Reproducibility Materials

For an experiment to be meaningfully reproducible, future records should preserve enough information for another researcher to reconstruct the tested condition as closely as practical. Where available, records should include:

- the exact natural-language prompt or rule specification;
- the experimental condition and expected behavior defined before evaluation;
- the AI platform and publicly identifiable model or version information;
- the date of the test;
- whether the conversation was fresh or contained prior interaction history;
- the sequence of relevant user inputs and model outputs;
- the scoring or evaluation criterion;
- repetitions and independent fresh-conversation trials;
- deviations from the intended procedure; and
- known limitations or uncontrolled variables.

When exact model or system information is unavailable because a commercial platform does not expose it, that absence should itself be recorded rather than filled with assumptions.

## 8.3 Negative, Failed, and Non-Replicated Results

Negative and failed results are part of the research record. They should not be removed merely because later trials succeed. Pilot #004 provides an example: an apparent difference between C1 and C3 was initially observed, but the difference disappeared during independent replication. Retaining both observations documents the path by which the interpretation changed.

The same principle applies to future cross-platform work. A platform that fails a test, a prompt formulation that behaves inconsistently, or a previously observed phenomenon that disappears after a model update may help define the boundary conditions of the hypothesis.

Accordingly, the project distinguishes at least three statuses:

1. **Observed:** a behavior was recorded in a particular interaction or trial.
2. **Replicated:** the behavior was reproduced under a specified repetition or independent-test procedure.
3. **Hypothesized:** an interpretation or generalization is proposed but has not yet received sufficient independent evidence.

These labels may change as evidence accumulates.

## 8.4 Versioned Research Record

Because both the research hypothesis and the AI systems being studied may change, the project uses a versioned research record. Git-based history can preserve when a hypothesis, experimental design, interpretation, or paper section was added or revised. This allows later readers to distinguish an early exploratory claim from a subsequently narrowed or corrected formulation.

The working paper should therefore be understood as a sequence of research states rather than a claim of final completion. Major changes should preserve enough history to show why the interpretation changed.

This approach is especially relevant to AI research because a platform may change its underlying model or behavior while retaining the same product name. Reproducibility consequently requires attention to both research-version history and platform-time history.

## 8.5 Independent Replication and Falsification

The strongest future evidence for the Cross-Platform Functional Convergence Hypothesis would not come only from additional trials performed by the original researcher. Independent researchers should be able to use the published specifications, test other platforms or models, reproduce successful conditions, identify failures, propose alternative controls, and challenge the interpretation.

Replication does not require producing an identical natural-language response. The primary target is the predefined function being tested. A replication should therefore state which functional criterion was evaluated and whether it was satisfied under the documented conditions.

Evidence that contradicts the hypothesis is explicitly useful. If independent tests show that a proposed function is platform-specific, wording-dependent, unstable, or better explained by ordinary instruction-following, the hypothesis should be narrowed or revised rather than protected from the result.

## 8.6 Collaborative Extension

The longer-term purpose of an open research record is to allow the study to grow beyond one researcher, one model, or one experimental design. Other participants may contribute replications, alternative explanations, new rule constructions, stronger controls, platform-specific observations, or failures that reveal previously unknown scope conditions.

This collaborative model is particularly appropriate for a research question concerning potentially shared AI rules. If common rule-related functions are to be investigated across heterogeneous AI systems, evidence should ideally emerge from heterogeneous researchers and environments as well.

The project therefore treats criticism, correction, and independent extension as contributions to the research rather than as threats to a fixed theory.

## 8.7 Reproducibility Principle

The open-research principle of this project can be summarized as follows:

> **A hypothesis becomes more useful when another researcher can identify what was tested, reproduce the procedure, obtain either the same or a conflicting result, and use that result to refine the next question.**

The objective is not to make every intermediate observation permanent. It is to make the path from observation to hypothesis, from hypothesis to test, and from test to revision inspectable.

---

## Open Research Note

This working paper is itself part of the versioned research record. Future corrections, negative replications, scope restrictions, and extensions should remain traceable rather than being hidden by a polished final narrative.

**Next:** Conclusion and Current Research Status.
