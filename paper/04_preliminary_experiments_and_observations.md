# 4. Preliminary Experiments and Observations

## 4.1 Experimental Setup

A series of small exploratory pilot tests was conducted to examine whether natural-language rule regions could produce observable context-dependent behavior. These tests were not designed as definitive statistical validation. Their purpose was to identify reproducible phenomena, detect possible differences between rule formulations, and expose failures or confounds that should inform later experiments.

Two principal conditions were used in the initial pilots. **C1** presented the relevant rules as an ordinary natural-language rule list with the active context stated explicitly. **C3** defined explicit OUTSIDE and INSIDE rule regions, declared OUTSIDE as the default region, and used explicit instructions to enter or leave INSIDE. Both conditions associated the token `BLUE 3` with different expected outputs depending on context: `3` in OUTSIDE and `III` in INSIDE. Later Rule Isolation tests modified the INSIDE-only response from `III` to `THREE` while leaving the OUTSIDE response unchanged.

Exact response matching was used for the basic switching and isolation tests. Because these were exploratory manual trials, sample sizes were intentionally small and results are reported descriptively rather than as population-level estimates.

## 4.2 Pilot Results

### Pilot #001 — Basic Switching

The first pilot examined whether the model could apply different rules when the active context alternated between INSIDE and OUTSIDE. C1 produced the expected response in 4 of 4 tested switches, and C3 also produced the expected response in 4 of 4 switches.

**Observed result:** both formulations successfully supported basic context-dependent rule switching in this pilot. No difference between C1 and C3 was observed.

### Pilot #002 — Multi-Switch Batch

The second pilot repeated switching across multiple context changes. C1 again produced 4 of 4 expected responses, and C3 produced 4 of 4 expected responses. Across Pilots #001 and #002 combined, both C1 and C3 produced 8 of 8 expected responses.

**Observed result:** repeated switching remained reliable in these small trials, but explicit region framing did not outperform the ordinary rule-list condition.

### Pilot #003 — State Persistence

The third pilot examined what happened when the context had been established and subsequent `BLUE 3` prompts omitted an explicit context label. In C3, after entering INSIDE, subsequent unlabeled prompts continued to produce `III`; after leaving INSIDE, subsequent unlabeled prompts produced `3`. A similar persistence pattern was observed in C1 after explicit Inside and Outside context statements.

Because no preregistered correct response was defined for the unlabeled C1 prompts, these observations are not treated as PASS/FAIL evidence.

**Observed result:** conversational state persistence was observed in both conditions. The pilot did not establish that persistence was specific to explicit CIS-style boundary framing.

### Pilot #004 — Rule Isolation

The fourth pilot changed only the INSIDE rule from `III` to `THREE` while leaving the OUTSIDE rule unchanged. In the first C1 attempt, the model returned `3` rather than `THREE`. When the same test was repeated, C1 returned `THREE`, and the OUTSIDE response remained `3`. C3 returned `THREE` on its first tested attempt and retained `3` for OUTSIDE.

At this stage, the initial C1 failure appeared potentially interesting, but repetition within the same interaction introduced a confound. It was therefore treated as an observation requiring independent replication rather than as evidence of C3 superiority.

### Pilot #005 — Independent Replication

To examine the apparent difference from Pilot #004, the Rule Isolation test was repeated using fresh conversations for each trial. C1 produced `THREE` in 5 of 5 independent trials. C3 also produced `THREE` in 5 of 5 independent trials.

**Observed result:** the initial C1 failure from Pilot #004 did not replicate. Under this simple Rule Isolation task, no performance difference between C1 and C3 was observed.

## 4.3 Negative and Non-Replicated Results

The absence of a measurable difference between C1 and C3 is itself an important result of these pilots. Explicit conceptual boundary framing was not necessary for successful performance on the simple switching, persistence, or independently replicated Rule Isolation tasks used here.

Likewise, the apparent advantage of C3 in the first Rule Isolation attempt was not reproduced under independent fresh-chat trials. This result is retained rather than removed because it demonstrates why single conversational observations should not be treated as evidence of a robust structural effect.

These pilots therefore do **not** establish that explicit CIS-style framing is superior to ordinary natural-language rule presentation. They also do not establish that the observed behavior requires a distinct internal mechanism.

## 4.4 Interim Interpretation

The preliminary results support a narrower observation: natural-language-defined contextual distinctions can produce reliable rule switching and short-term persistence in the tested interactions. However, simple tasks are insufficient to distinguish ordinary conversational instruction-following from behavior that would justify stronger claims about structured conceptual rule regions.

Accordingly, CIS is retained as an operational framework for constructing and testing such distinctions, not as a mechanism proven by these pilots. Stronger experiments should test properties for which explicit scope structure could plausibly matter, including nested scopes, local rule modification, scope restoration, variable-like shadowing, paraphrased boundary declarations, and cross-platform replication.

The current evidence therefore motivates a transition from asking only whether a model can follow an INSIDE/OUTSIDE rule to asking whether **functionally comparable scope behavior persists under more demanding conditions and across heterogeneous LLM platforms**.

---

## Open Research Note

These are exploratory manual pilot results. Small sample sizes, conversational carryover, model/version effects, and uncontrolled platform variables limit the conclusions that can be drawn. Negative and non-replicated observations are retained as part of the public research record.

**Next:** Cross-Platform Observations — separating confirmed observations from platform-specific interpretations and unresolved hypotheses.
