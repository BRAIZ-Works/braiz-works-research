# Evidence-First AI Operations

## Making agentic work attributable, current, recomputable, and reviewable

**BRAIZ Works Research**
**WP-03 · Version 1.0.0 · September 24, 2026**

> Public-safe research. This paper describes principles and control outcomes, not private UBuildOS implementation.

## Executive summary

Enterprise AI needs more than persuasive output. It needs evidence that is tied to the exact subject, current enough for the decision, attributable to a source, and reproducible by a reviewer. This paper defines an evidence-first operating model for agentic work at a public-safe level.

## Why output-first operations are fragile

A polished answer can conceal stale inputs, missing dependencies, unsupported assumptions, or an operation that never actually completed. As agentic systems take on longer workflows, the gap between “output exists” and “evidence supports the claimed state” grows.

NIST’s AI RMF emphasizes documented testing, measurement, governance, and context throughout the lifecycle. [3][5] Evidence-first operations turn those ideas into a practical operating question: what evidence would a skeptical reviewer need in order to accept this exact result?

## The evidence binding contract

Every material evidence object should identify at least five things: the subject it proves, the source or producer, the time/currentness basis, its role in the proof, and a way to recompute or independently inspect it.

| Evidence property | Why it matters |
| --- | --- |
| Exact subject | Prevents proof from drifting across versions |
| Source/provenance | Makes attribution inspectable |
| Currentness | Prevents stale evidence from silently surviving change |
| Role | Shows which requirement or claim the evidence supports |
| Recomputability | Lets a reviewer verify instead of merely trust |

## Evidence is a graph, not a folder

A large evidence directory can still be incomplete. What matters is whether every material obligation has a closed path from requirement to test to evidence to recovery, and whether every evidence object has a legitimate role. Orphan evidence creates noise; orphan requirements create risk.

A mature system therefore maintains bidirectional traceability: requirement to proof and proof back to requirement.

## Currentness and invalidation

Evidence has a dependency surface. If a source, model, file, environment, authority, or implementation changes in a way that affects the proof, the affected evidence must be invalidated and replaced. Unaffected evidence can remain valid. This localized invalidation avoids two extremes: blindly reusing stale proof or needlessly rebuilding everything.

## Recomputation over assertion

A checksum listed in a report is an assertion until someone recomputes it. A manifest is not authoritative merely because it exists. A test result is not current merely because it once passed.

For consequential claims, the producer should assume that supplied PASS labels are untrusted inputs and reconstruct the underlying population independently. This reduces the chance that a reporting layer hides an incomplete denominator or stale object.

## Evidence strength and uncertainty

Not every claim needs the same evidence. A low-risk drafting suggestion may need little beyond source attribution. A high-consequence release or deployment needs stronger identity, authority, recovery, and readback. The important point is explicitness: measured, documented, modeled, illustrative, target, and unknown states should not be silently converted into one another.

## Portable evidence for independent review

Independent review should not require access to the producer’s private filesystem, chat history, or inaccessible runtime. Admission-critical evidence should travel with the review subject in a self-contained, immutable handoff. That design improves portability, reduces reviewer dependence on the producer, and exposes hidden assumptions earlier.

## Public-safe disclosure boundary

The principles above can be public without releasing proprietary evidence schemas, validator code, attack sets, or private evidence corpora. Enterprises benefit from knowing what evidence qualities to require; vendors can preserve implementation-level intellectual property.

## Limitations

Evidence-first operation cannot make bad requirements good, guarantee source truth, or eliminate uncertainty. It improves the auditability of what a system knows and claims. The strength of any conclusion remains bounded by source quality, scope, currentness, and review coverage.

## References

[1] Stanford Institute for Human-Centered Artificial Intelligence. *The 2026 AI Index Report — Economy*. 2026. https://hai.stanford.edu/ai-index/2026-ai-index-report/economy

[2] McKinsey & Company. *AI at work but not at scale*. December 10, 2025. https://www.mckinsey.com/featured-insights/charts/ai-at-work-but-not-at-scale

[3] Tabassi, E. *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*. NIST AI 100-1. National Institute of Standards and Technology, 2023. https://doi.org/10.6028/NIST.AI.100-1

[4] Autio, C., Schwartz, R., Dunietz, J., Jain, S., Stanley, M., Tabassi, E., Hall, P., Roberts, K. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile*. NIST AI 600-1, 2024; NIST page updated April 8, 2026. https://doi.org/10.6028/NIST.AI.600-1

[5] National Institute of Standards and Technology. *NIST AI RMF Playbook*. https://www.nist.gov/itl/ai-risk-management-framework/nist-ai-rmf-playbook

[6] BRAIZ Works LLC. *UBuildOS Verified Completion™ Thesis v1.0.5*. September 15, 2026. DOI: https://doi.org/10.5281/zenodo.22775537 ; public repository: https://github.com/BRAIZ-Works/ubuildos-verified-completion-thesis

[7] BRAIZ Works LLC. *The Enterprise Execution Gap*. BRAIZ Works Research WP-02 v1.0.0. September 23, 2026.



### Source-currentness note

External references [1]-[5] are carried forward from the independently reviewed and publicly released WP-02 v1.0.0 canary. This batch does not claim a new live-web currentness check. Time-sensitive statistics are used only where explicitly cited and dated. First-party references [6]-[7] are BRAIZ Works publications.

## Rights and disclosure boundary

© 2026 BRAIZ Works LLC. All rights reserved.

This public artifact intentionally excludes private prompts, proprietary routing/controller logic, internal thresholds, private attack sets, protected evidence schemas, credentials, customer data, and reconstruction-sensitive implementation details.
