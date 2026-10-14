# Programme Charter — Orion

> One page the whole programme aligns to. If something isn't serving the objectives
> below, it's a candidate to stop.

## 1. Vision
Make customer onboarding **fast, compliant and self-serve** — turning a 10-day manual
process into a sub-1-day digital journey, without increasing risk.

## 2. Problem / opportunity
- Current onboarding takes **10+ working days**; ~22% of applicants drop out before completion.
- Manual KYC/AML checks are the main bottleneck and the main compliance risk.
- Competitors offer same-day onboarding; we are losing winnable customers.

## 3. Objectives & success measures
| Objective | Measure | Baseline | Target |
|---|---|---|---|
| Faster onboarding | Median time to active account | 10 days | < 1 day |
| Reduce drop-off | Application completion rate | 78% | 92% |
| Stay compliant | Audit findings on onboarding | 4 open | 0 open |
| Control cost | Cost to onboard per customer | £46 | £18 |

## 4. Scope
**In scope:** digital application journey, automated identity/KYC, decisioning engine,
customer comms, internal ops tooling, staff change & training.
**Out of scope:** core banking migration, pricing changes, legacy product retirement
(tracked separately, dependency only).

## 5. Workstreams
1. **Product & UX** — journey design, research, accessibility.
2. **Platform Engineering** — services, integrations, decisioning engine.
3. **Risk & Compliance** — KYC/AML rules, data protection, audit sign-off.
4. **Change & Adoption** — ops readiness, training, rollout, comms.

## 6. Phases (high level)
- **Phase 1 — Foundations (M1–M4):** discovery, architecture, compliance rules, MVP journey.
- **Phase 2 — Build & pilot (M5–M9):** full journey, automated KYC, controlled pilot.
- **Phase 3 — Scale & embed (M10–M12):** national rollout, decommission manual path, handover.

## 7. Budget
£2.4m total — 58% engineering, 18% change & adoption, 14% compliance/legal, 10% contingency.

## 8. Governance (summary)
Monthly **Programme Board** (decision & funding), fortnightly **delivery review**
(cross-workstream risks/dependencies), weekly **workstream stand-ups**. Full model in
[governance.md](governance.md).

## 9. Key roles
| Role | Responsibility |
|---|---|
| Programme SRO (sponsor) | Accountable for benefits & funding |
| Programme Manager (me) | Delivery, governance, risk, reporting |
| Workstream Leads ×4 | Day-to-day delivery of their stream |
| Compliance Lead | Regulatory sign-off |

## 10. Top-level risks (full log in [raid-log.md](raid-log.md))
- Regulatory change mid-programme could force KYC rework.
- Dependency on legacy identity service with limited support.
- Change fatigue in operations teams affecting adoption.
