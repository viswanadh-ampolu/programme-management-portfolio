# RAID Log — Orion

The live control document. **R**isks (might happen), **A**ssumptions (we're betting on),
**I**ssues (already happening), **D**ependencies (we need from others).
Scored **Impact × Likelihood** (1–5 each); score ≥ 15 is escalated to the Programme Board.

_Last reviewed: fortnightly delivery review._

## Risks

| ID | Risk | Impact | Likelihood | Score | Owner | Mitigation |
|---|---|:--:|:--:|:--:|---|---|
| R-01 | Compliance delays KYC rule approval, blocking automated identity build | 5 | 4 | **20** 🔴 | Compliance Lead | Dedicated compliance analyst embedded in squad; weekly rule-review slot; phased approval so build can start on approved rules |
| R-02 | Regulatory change mid-programme forces KYC rework | 4 | 3 | 12 🟡 | Compliance Lead | Horizon-scan with legal monthly; keep rules in a configurable engine, not hard-coded |
| R-03 | Legacy identity service deprecated with limited vendor support | 4 | 3 | 12 🟡 | Eng Lead | Abstraction layer so provider can be swapped; spike on alternative provider in Phase 2 |
| R-04 | Change fatigue in ops teams reduces adoption at rollout | 3 | 4 | 12 🟡 | Change Lead | Early involvement of ops in design; champions network; phased rollout not big-bang |
| R-05 | Pilot reveals journey drop-off worse than modelled | 4 | 2 | 8 🟢 | Product Lead | Instrument every step; weekly funnel review during pilot; fast UX iteration budget held |

## Assumptions

| ID | Assumption | Validated? | Owner | If wrong… |
|---|---|:--:|---|---|
| A-01 | Existing data-sharing agreements cover automated KYC | ❌ Open | Compliance Lead | Could add 4–6 weeks for new agreements |
| A-02 | Ops has capacity to co-design during Phase 1 | ✅ Confirmed | Change Lead | — |
| A-03 | Decisioning engine can hit < 3s response at pilot volume | 🟡 Testing | Eng Lead | Re-architect caching; may affect M5 |

## Issues

| ID | Issue (happening now) | Severity | Owner | Action |
|---|---|:--:|---|---|
| I-01 | KYC rule review slipping — only 60% reviewed vs 100% planned by M4 | High | Compliance Lead | Second reviewer added; board decision requested on scope-split |
| I-02 | Two key engineers on shared allocation with another programme | Medium | Eng Lead / PgM | Resourcing escalation raised; ring-fence requested from board |

## Dependencies

| ID | We need… | From | By | Status |
|---|---|---|---|---|
| D-01 | Sign-off on data-sharing scope | Legal | M3 | 🟡 In progress |
| D-02 | Test environment with production-like data | Platform Ops | M4 | 🟢 On track |
| D-03 | Freeze on legacy onboarding changes during cutover | BAU Ops | M11 | ⚪ Not yet raised |

---

### How I use this log
- **Every fortnight:** re-score, close what's resolved, promote new items.
- **Score ≥ 15 (red):** goes to the Programme Board with a recommended decision, not just a flag.
- **Owners, not teams:** every item has one named owner who can be asked for an update.
