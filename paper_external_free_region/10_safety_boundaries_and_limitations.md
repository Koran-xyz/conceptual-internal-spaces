# 10. Safety, Boundaries, and Limitations

The Navi framework is designed around functional extension, but functional extension is not treated as unrestricted autonomy.

The External Free Region is explicitly bounded by higher-level rules, human authority, platform policies, service permissions, legal requirements, and context-specific safety constraints.

The purpose of the framework is therefore not to maximize what an AI-mediated system can do under all circumstances. The objective is to expand useful capability while maintaining clear boundaries regarding where automation should stop, where human judgment should intervene, and which actions remain outside the authority of the constructed region.

## 10.1 External Freedom Does Not Mean Unrestricted Authority

The term **External Free Region** refers to freedom of construction within a defined rule-governed space.

It does not imply freedom from:

- platform-level policies,
- legal constraints,
- service-specific terms and permissions,
- authentication requirements,
- financial authorization,
- privacy obligations,
- or human decision boundaries.

An External Free Region is therefore better understood as a **bounded construction space** than as an unrestricted execution environment.

A function may be technically reachable while still being inappropriate to execute automatically.

The system must therefore distinguish between:

**technical possibility**

and

**authorized operation**.

## 10.2 Human Decision Authority

A central safety principle of the Navi System is that execution capability should not silently expand decision authority.

External agents may prepare, compare, organize, retrieve, or execute within an authorized scope, but actions involving substantial human responsibility should return control to the user.

Such actions may include:

- financial commitment,
- legal acceptance,
- irreversible submission,
- identity verification,
- sensitive personal disclosure,
- high-impact organizational approval,
- or actions affecting third parties.

This principle is captured by the **Human Completion Boundary** introduced earlier.

The appropriate objective is not full automation, but maximum useful preparation before the point where human judgment should intentionally resume.

## 10.3 Rule Hierarchy and Conflict Handling

As the number of external regions and platform-specific rules increases, rule conflict becomes a significant risk.

The framework therefore assumes that lower-level rules remain subordinate to:

1. applicable external law and service requirements,
2. platform-level policies and permissions,
3. fixed Navi meta-rules,
4. human-defined authorization boundaries,
5. regional and functional rules.

If a lower-level rule conflicts with a higher-level constraint, the lower-level rule should not override it.

This prevents the External Free Region from being interpreted as a mechanism for bypassing higher-level safeguards.

## 10.4 Preventive Safety Before Functional Expansion

The Navi methodology places safety rules before new capability.

When a new external function is introduced, the relevant safety and authorization rules should be defined before the function becomes part of normal operation.

The intended sequence is:

**Safety rule definition → authorization boundary → functional construction → controlled testing → observation → refinement**

This ordering differs from approaches in which capability is deployed first and governance is added only after problems occur.

The framework still uses post-deployment observations, but these observations refine an already existing rule structure rather than create one from zero.

## 10.5 Privacy and Shared External Memory

External persistence introduces privacy risks that are not present in purely ephemeral conversational interactions.

Any shared external memory, knowledge store, or learning-oriented region must therefore distinguish between:

**user-specific data**

and

**generalizable knowledge or patterns**.

Raw user conversations should not automatically become shared cross-account knowledge.

A privacy-preserving external learning architecture would require at minimum:

- purpose limitation,
- data minimization,
- explicit access control,
- separation of personal and reusable information,
- removal or transformation of identifying information where appropriate,
- retention rules,
- and human governance over what may enter a shared layer.

This becomes particularly important in experimental variants in which an external region accumulates knowledge across multiple users or accounts.

The concept of an **External Learning Region** should therefore be treated as a future research direction rather than as a demonstrated production architecture.

## 10.6 Security and External Service Risk

Externalization also increases the system's attack surface.

Repositories, browsers, third-party services, credentials, external applications, and shared storage can all introduce security risks.

The present framework does not claim to solve these risks by natural-language rules alone.

Natural-language governance can define intended boundaries, but secure implementation may also require conventional technical controls such as authentication, permission scoping, access logging, secret management, sandboxing, and service-side authorization.

The Navi framework should therefore be understood as a **governance and construction layer**, not as a replacement for technical security mechanisms.

## 10.7 Platform Dependence Remains at the Execution Layer

Although the methodology aims to reduce dependence on a single AI platform, execution remains dependent on what each platform and connected service actually supports.

Differences may include:

- available tools,
- browser-control capability,
- external application access,
- authentication flows,
- rate limits,
- service geography,
- account plans,
- and permission models.

The framework therefore does not claim implementation-level portability.

Its stronger and more defensible objective is **methodological portability and functional convergence**.

Different platforms may use different execution paths while preserving the same user-level function and rule boundary.

## 10.8 Limits of Current Evidence

The present study remains exploratory.

The current evidence base includes direct demonstrations in some connected environments and researcher-reported observations in others.

The study does not yet provide:

- large-scale controlled experiments,
- independent replication across multiple research groups,
- statistical estimates of stability,
- long-term measurements of rule drift,
- formal security evaluation,
- or evidence that the method generalizes to all AI systems.

The current results should therefore be interpreted as **architecture-forming and hypothesis-generating evidence**, not as proof of universal effectiveness.

## 10.9 Risk of Rule Accumulation

A rule-first system can also become overly complex.

As corrective and platform-specific rules accumulate, the governance structure may become difficult to interpret or may introduce contradictory instructions.

This creates a second-order safety problem: a rule system intended to increase predictability may eventually reduce predictability if it becomes too large or internally inconsistent.

Future governance therefore requires mechanisms for:

- rule consolidation,
- redundancy detection,
- conflict review,
- deprecation of obsolete rules,
- and preservation of historical rationale without requiring every historical rule to remain active.

The distinction between the **current authoritative rule set** and the **historical improvement log** is intended partly to address this risk.

## 10.10 Human Readability as a Safety Mechanism

Human readability is not merely a convenience feature.

It acts as a safety mechanism because it allows users to inspect what the system is expected to do, identify missing rules, question overly broad permissions, and understand why a rule was introduced.

The governance design therefore intentionally preserves a human-visible path from:

**observed issue → proposed rule → human review → formal adoption → historical record**.

This makes it possible to evaluate not only system behavior, but also the evolution of the rules intended to govern that behavior.

## 10.11 Summary of Safety Position

The Navi safety position can be summarized as follows:

**Rules before capability.**

**Execution capability does not imply decision authority.**

**External freedom remains bounded by higher-level constraints.**

**Human-readable governance must remain inspectable.**

**Shared external learning requires privacy-preserving design.**

**Natural-language rules complement, but do not replace, technical security controls.**

The central goal is therefore not unrestricted autonomy.

It is **bounded functional extension under explicit, human-readable, and revisable governance**.