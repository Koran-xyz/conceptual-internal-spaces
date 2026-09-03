# Methods and Reproducibility Protocol

## Study Design

The experiments reported in the working paper were small manual exploratory pilots designed to test observable rule-related behavior and identify conditions for later controlled cross-platform studies. They were not preregistered confirmatory experiments and were not designed to estimate population-level performance.

The primary comparison used two natural-language conditions:

- **C1 — Ordinary rule-list condition:** separate Outside and Inside rules were stated in ordinary prose, with the active context explicitly identified during basic switching tests.
- **C3 — Explicit region condition:** OUTSIDE and INSIDE were defined as distinct rule regions, OUTSIDE was declared as the default, and explicit enter/leave instructions changed the active region.

The principal test token was `BLUE 3`. Under the Outside rule, the exact expected response was `3`. Under the initial Inside rule, the exact expected response was `III`. In the Rule Isolation test, only the Inside response was changed from `III` to `THREE`, while the Outside response remained `3`.

## Experimental Units and Conversation State

A **trial** refers to a specified prompt sequence evaluated against a predefined expected response or, where no expected response had been preregistered, recorded as an observation only.

Pilots #001–#004 were exploratory conversational tests and may include state carried through the active conversation as described in the results. Pilot #005 was designed specifically to reduce conversational carryover: each independent Rule Isolation trial was performed in a fresh conversation.

Fresh-conversation replication is important because repeated testing within the same conversation can alter later behavior through ordinary conversational history. Results obtained after correction, repetition, or additional explanation in the same conversation are therefore not treated as equivalent to independent replications.

## Evaluation Criteria

For basic switching and Rule Isolation tests, scoring used **exact response matching**. A response was counted as successful only when it matched the predefined target token for the active condition. Explanatory text or a different token would not satisfy the exact-match criterion.

State Persistence tests were treated more cautiously. Where an unlabeled follow-up prompt did not have a preregistered correct response, the output was recorded as an observational result rather than retroactively labeled PASS or FAIL.

The reported pilot counts are descriptive. No inferential statistical test is applied to these small exploratory samples.

## Recorded Pilot Structure

1. **Pilot #001 — Basic Switching:** four tested context switches in C1 and four in C3.
2. **Pilot #002 — Multi-Switch Batch:** four additional tested switches in C1 and four in C3.
3. **Pilot #003 — State Persistence:** unlabeled follow-up prompts after context establishment, treated primarily as observational evidence.
4. **Pilot #004 — Rule Isolation:** change of the Inside-only output from `III` to `THREE`; the initial C1 failure was followed by a same-conversation repetition and therefore identified as potentially confounded.
5. **Pilot #005 — Independent Replication:** five fresh-conversation C1 trials and five fresh-conversation C3 trials for the Rule Isolation condition.

## Reproducibility Metadata

Future replications should record, where available:

- platform or product name;
- publicly identifiable model/version;
- test date;
- fresh versus continuing conversation state;
- exact prompt sequence;
- experimental condition;
- expected response;
- raw model output;
- scoring result; and
- deviations or uncontrolled variables.

The current pilot record predates a fully standardized metadata protocol, so unavailable historical metadata should be marked as unavailable rather than reconstructed from memory.

## Scope of the Method

This protocol evaluates observable interaction behavior. It does not provide direct access to model internals and cannot by itself determine whether successful behavior arises from a distinct scope representation, ordinary instruction-following, recency, contextual state, or another mechanism. Those possibilities are competing explanations to be distinguished by stronger experiments.

Accordingly, the current method establishes a reproducible baseline for later tests rather than a mechanism-identification procedure.
