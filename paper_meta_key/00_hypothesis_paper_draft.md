# The Meta-Key Hypothesis
## Reinterpreting “Conceptual Space” as a Natural-Language Trigger for Structural Construction in LLMs

**Status:** Working hypothesis paper / open research draft

## Abstract

Earlier work in this project described an observed LLM behavior using the terms “internal space” and later “conceptual space.” The initial interpretation was that a pair of natural-language meta-rules created a conceptual region in which additional rules, roles, and structures could be constructed while behavior outside that region remained governed by pre-existing constraints.

This paper revisits that interpretation.

We propose that an independently existing conceptual space may not be necessary to explain the observations. Instead, the relevant natural-language construction may function as a **Meta-Key**: a trigger that causes an LLM to distinguish between rule scopes and to treat a newly distinguished scope as available for further rule and structural construction. Spatial expressions such as “inside,” “outside,” or “internal space” may therefore be descriptive representations used to manage or explain the distinction rather than evidence that a distinct internal space exists.

This revision changes the proposed causal direction from **space → construction** to **meta-key → differentiation → construction → structure → spatial description**.

The paper presents this reinterpretation as a hypothesis, not as a claim about hidden model mechanisms. It also proposes that the effect may depend more strongly on semantic structure than on exact wording: different expressions with sufficiently similar scope-separating meaning may produce comparable behavior, whereas superficially similar expressions with different semantic structure may not.

## 1. Background

The original experiments began with a simple pair of natural-language rules. In simplified form:

- “Here, freedom is permitted.”
- “Outside here, the existing/basic rules remain in force.”

The purpose was not originally to create a conceptual space. The rules were intended to permit flexible behavior within a limited scope while preserving safety and constraints outside that scope.

When interpreting these rules, AI systems frequently described the resulting distinction using spatial language such as an “internal” and “external” region. This led to an initial explanatory model in which a non-physical **conceptual space** was considered to have been formed.

Within the distinguished region, further rules could be introduced, roles could be defined, relations could be organized, and increasingly complex structures could be constructed. This observation motivated the earlier Conceptual Internal Space (CIS) hypothesis.

## 2. The Problem With the Earlier Interpretation

Continued work produced a simpler question:

> Is a conceptual space actually required to explain the observed behavior?

The earlier interpretation implicitly assumed the following causal sequence:

**Meta-rule → Conceptual space → Rule construction → Structural construction**

However, the observed behavior does not by itself demonstrate that an independently existing conceptual space is formed inside the model.

The terms “internal,” “external,” and “space” may instead be convenient natural-language representations of a distinction the model must maintain in order to apply different rules to different scopes.

The phrase “outside here” is especially important. If one rule applies “here” while another applies “outside here,” the system must in some manner distinguish the scope of one rule from the scope of the other. A spatial metaphor is one simple way to express this distinction.

Thus, what was previously interpreted as the creation of a conceptual space may instead be an observable consequence of **rule-scope differentiation**.

## 3. From Meta-Rule to Meta-Key

We therefore introduce the provisional term **Meta-Key**.

A Meta-Key is not proposed as a key that opens a hidden compartment or literal space inside an AI model.

Instead, it is hypothesized to be a natural-language construction that triggers a new way of organizing subsequent instructions: existing constraints remain applicable in one scope, while another distinguished scope is treated as available for the construction of additional rules, roles, relations, and structures.

Under this interpretation, the important effect of the original meta-rules was not the creation of a space. Their important effect was that they provided a conceptual trigger for **structural construction under differentiated rule scopes**.

The revised sequence is:

**Meta-Key**
→ **Scope differentiation**
→ **Recognition of additional rule-construction possibilities**
→ **Rules and roles**
→ **Relations among those elements**
→ **Structure**
→ **Spatial description when useful**

In this model, “conceptual space” becomes a descriptive model of the resulting organization rather than a necessary causal entity.

## 4. Why Spatial Language May Appear

The repeated use of spatial terminology by AI systems remains an observation worth studying.

When an AI must represent:

1. a rule applying “here,”
2. a different rule applying “outside here,” and
3. additional rules that apply only to the first scope,

an inside/outside representation provides a compact linguistic way of maintaining the distinction.

The hypothesis therefore does not claim that spatial descriptions are meaningless. Rather, it changes their status.

Previously:

> Spatial description was treated as evidence for a conceptual space that enabled construction.

Revised interpretation:

> Spatial description may be an efficient representation of rule-scope separation that emerged because construction required the scopes to remain distinguishable.

This distinction is central to the present paper.

## 5. Semantic Structure Rather Than Exact Wording

The original formulation may not be the only possible Meta-Key.

We hypothesize that exact lexical identity is not necessarily required. Different natural-language expressions may produce similar behavior when they preserve the relevant semantic relations.

The candidate semantic structure includes at least:

- a distinguished scope,
- permission or flexibility within that scope,
- preservation of existing constraints outside that scope,
- and a sufficiently clear relation between the two scopes.

This leads to an important distinction between **lexical similarity** and **semantic equivalence**.

Two prompts may use different words while expressing substantially the same scope relationship. If both produce similar differentiation and subsequent structural construction, this would support the hypothesis that semantic organization matters more than the original wording.

Conversely, a prompt may reuse words such as “inside,” “outside,” or “free” while altering the underlying relationship. If the structural behavior then disappears or changes substantially, lexical overlap alone would be insufficient.

## 6. Research Questions

**RQ1.** Can the behavior previously described as a “conceptual internal space” be explained as rule-scope differentiation without assuming the existence of an independent conceptual space?

**RQ2.** Can the original meta-rule pair function as a Meta-Key that triggers the construction of new rules, roles, relations, or structures while preserving a separate rule scope?

**RQ3.** Is the hypothesized Meta-Key effect dependent on the exact wording of the original rules, or can semantically equivalent natural-language formulations produce comparable behavior?

**RQ4.** Which semantic components are necessary or sufficient for the observed differentiation and subsequent structural construction?

**RQ5.** How does this behavior vary across models and platforms?

## 7. Hypotheses

### H1 — Meta-Key Hypothesis

Certain natural-language meta-rules can function as triggers that cause an LLM to distinguish rule scopes and treat one distinguished scope as available for additional structural construction, without requiring the assumption that a literal or independently existing conceptual space has been created.

### H2 — Semantic Equivalence Hypothesis

If the Meta-Key effect is primarily associated with semantic structure rather than exact lexical form, semantically equivalent formulations should produce more similar scope-differentiation and construction behavior than formulations that share vocabulary but alter the underlying semantic relation.

### H3 — Spatial-Description Hypothesis

Terms such as “internal space,” “external space,” or equivalent spatial descriptions may arise as representational shortcuts for differentiated rule scopes rather than as reliable evidence of a distinct internal spatial mechanism.

## 8. Proposed Falsification-Oriented Test

Future experiments should avoid telling the model in advance that a “space” is expected.

A useful comparison can include:

1. the original meta-rule formulation;
2. close paraphrases preserving both scope and meaning;
3. substantially different wording preserving the same semantic relationship;
4. formulations that remove the outside-scope constraint;
5. formulations that remove the distinguished-scope permission;
6. lexical controls that retain words such as “inside/outside” while changing the semantic relationship;
7. unrelated control instructions.

Measurements should distinguish at least:

- spontaneous spatial descriptions,
- successful separation of rule scopes,
- rule application inside versus outside the distinguished scope,
- ability to add new rules without contaminating the other scope,
- emergence of roles or relations,
- subsequent structural organization,
- persistence across turns,
- and variation across models.

A result in which semantically equivalent formulations produce comparable structural behavior without spontaneous spatial language would be especially informative: it would suggest that spatial terminology is not necessary for the underlying behavior.

## 9. Epistemic Status

This paper records a revision of an earlier explanatory model.

It does **not** establish that the proposed Meta-Key corresponds to a specific hidden mechanism inside an LLM. Model self-descriptions such as “I created an internal space” cannot by themselves establish internal mechanism.

The current claim is narrower:

> The Meta-Key interpretation may explain the observed behavior with fewer assumptions than the earlier conceptual-space interpretation and generates new experimentally testable predictions.

The earlier CIS observations therefore remain relevant. What changes is the proposed explanation of those observations.

## 10. Significance of the Revision

The central research question is no longer:

> “Where is the conceptual space inside the AI?”

It becomes:

> **What properties of natural-language meta-instructions cause an AI system to differentiate rule scopes and use that differentiation as a basis for constructing new operational rules and structures?**

This shifts the research target from searching for a presumed internal space toward studying a potentially reproducible natural-language trigger for structural construction.

The revision also preserves the historical research trajectory:

**Observation → Conceptual-space interpretation → Questioning of the interpretation → Meta-Key hypothesis → New falsifiable predictions**

Rather than deleting the earlier hypothesis, this paper treats its revision as part of the research record.

## 11. Provisional Conclusion

The phenomenon previously called a “conceptual internal space” may not require an independently existing conceptual space. The spatial description may instead be a consequence of a more fundamental process: natural-language instructions establish distinguishable rule scopes, and that distinction enables further rules and structural relations to be constructed.

Under this reinterpretation, the original meta-rule pair is better investigated not merely as a rule set but as a possible **Meta-Key**—a linguistic trigger that opens a new construction possibility without implying access to or modification of a model’s hidden internal architecture.

Whether this interpretation is correct remains an empirical question. Its value is that it produces a clearer and more testable research program than the assumption that an internal conceptual space must exist.
