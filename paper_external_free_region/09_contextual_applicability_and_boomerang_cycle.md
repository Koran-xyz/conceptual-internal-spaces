# 9. Contextual Applicability Testing and the Boomerang Research Cycle

The Navi research program does not treat each new application domain as an independent project.

Instead, different domains are used as **test contexts** for evaluating the same underlying construction principles under changing conditions.

A personal travel scenario, an enterprise workflow, an external repository task, or an experimental learning environment may appear unrelated at the application level. However, each can expose different strengths, weaknesses, and boundary conditions of the same core Navi architecture.

This research style is referred to here as the **Boomerang Research Cycle**.

The term describes a recurring process in which the core system is extended into a new context, tested under that context's specific requirements, and then returned to the core with newly observed information.

The cycle can be represented as:

**Core structure → New context → Practical testing → Observation → Rule or structural refinement → Return to core**

The metaphor is intentional: the research may travel outward into apparently different domains, but the resulting observations are brought back to the same central structure.

## 9.1 Contexts as Experimental Environments

Different application domains are therefore treated as **experimental environments** rather than as final product categories.

For example, personal travel planning may test:

- multi-stage planning,
- transportation comparison,
- accommodation selection,
- budgeting,
- scheduling,
- web-based service interaction,
- and human confirmation boundaries.

Enterprise use may introduce:

- authorization,
- approval workflows,
- organizational policy,
- auditability,
- persistent records,
- and role separation.

A learning-oriented external region may instead expose:

- shared knowledge accumulation,
- rule evolution,
- access restrictions,
- reusable patterns,
- and long-term external memory.

Each context therefore stresses a different part of the same architecture.

## 9.2 Broad Testing Before Narrow Specialization

The Navi methodology intentionally favors broad contextual testing before narrowing the system toward a specific market or organizational use case.

Beginning directly with an enterprise workflow, for example, may prematurely constrain the architecture around approval structures, budgets, formal roles, and existing business processes.

Personal-use contexts often provide a wider range of behavior, preferences, and interaction patterns.

Testing across broad individual contexts can therefore reveal unexpected use cases, interaction requirements, accessibility needs, flexibility requirements, and structural weaknesses before the system is specialized for enterprise deployment.

The objective is not to prioritize consumer use over enterprise use.

Rather, broad contexts are used to avoid reducing the design space too early.

## 9.3 Contextual Differences as Sources of Core Improvement

A weakness discovered in one context may have broader significance.

For example, a difficulty observed in an older-user scenario may reveal that the interface requires unnecessary complexity.

A problem observed in enterprise use may reveal insufficient approval or audit rules.

A travel-planning experiment may expose weak coordination between search, scheduling, and external execution.

These findings should not automatically remain isolated within their original domain.

Instead, the framework asks:

**Is this a context-specific problem, or does it reveal a general weakness in the core architecture?**

If the issue is generalizable, the corresponding improvement should be returned to the shared core.

## 9.4 User Diversity as a Test Variable

The principle that different users may complete the Navi system differently introduces an additional dimension of testing.

The same core may be used by individual users, younger users, older users, researchers, employees, managers, or organizations.

The intended outcome is not that each group receives an identical experience.

Instead, the core should provide a sufficiently stable foundation while allowing the final configuration to reflect the user's actual goals, environment, and preferences.

User diversity therefore becomes a research variable rather than a problem to eliminate.

## 9.5 The 80/20 Construction Principle

The current Navi design uses an informal **80/20 construction principle**.

The system aims to provide a substantial shared foundation while intentionally preserving a portion of the design space for user-defined construction.

The first portion contains the common core, safety principles, external connections, and reusable structures.

The remaining portion is completed through user-specific dialogue, preferences, and contextual needs.

The exact percentage is conceptual rather than a measured engineering ratio.

Its purpose is to prevent the system from becoming so fully predetermined that the user can only operate within a fixed product mold.

This principle reflects a broader design philosophy:

**the system should provide capability without eliminating user authorship.**

## 9.6 From Product Templates to Possibility Proposals

This approach also changes how practical applications are presented.

Rather than presenting a single fixed workflow as the product, the Navi framework can present multiple possible use cases and allow users or organizations to extend the structure through dialogue.

For example, a travel-planning capability may lead a user to ask whether the same structure can support business travel, expense preparation, restaurant reservations, calendar integration, mobility assistance, or event coordination.

Such questions are not treated as deviations from the original design.

They are part of the construction process.

The system therefore emphasizes **possibility proposals** rather than rigid templates.

## 9.7 Continuous Completion

The Boomerang Research Cycle also supports the concept of **continuous completion**.

A system version may be sufficiently complete for current use while still remaining open to future extension.

As contextual experiments identify new reusable functions or rules, some of those improvements return to the shared core.

The enlarged core then becomes the foundation for a new generation of user-specific construction.

The resulting process can be represented as:

**Core₁ → Contextual extension → Discovery → Generalization → Core₂ → New extension**

Completion is therefore temporary but meaningful.

The system is complete enough to use, but not complete in the sense of closing future possibilities.

## 9.8 The Boomerang Cycle as a Research Method

The Boomerang Research Cycle can therefore be summarized as five stages:

**1. Launch** — Apply the current core structure to a new context.  
**2. Stress** — Expose the structure to the specific requirements and constraints of that context.  
**3. Observe** — Record successes, failures, behavioral tendencies, and rule gaps.  
**4. Return** — Bring generalizable findings back to the shared core.  
**5. Relaunch** — Test the revised core in another context.

This method is exploratory by design.

It is intended to discover the applicability boundaries of the architecture before making broad claims about generality.

## 9.9 Research Interpretation

Under this framework, movement across domains should not be interpreted as uncontrolled topic switching.

The relevant question is whether each contextual branch returns useful evidence to the same central research problem.

If it does, the branch functions as an experimental extension of the core research program.

The method can therefore be summarized as:

**Expand outward to discover; return inward to refine.**
