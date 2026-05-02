# Red/Blue Analysis: CLASP Full Concept

**Date:** 2026-05-02
**Technique:** Red Team / Blue Team Adversarial Analysis
**Attack Dimensions:** Technical feasibility, Regulatory pathway, Commercial viability, Political durability, Competitive response

---

## Blue Team Defense

### Problem and Solution Fit
The US has a structural deficit in domestic ship recycling capacity. Navy and MARAD face $50-100M/yr in end-of-life vessel disposal with no domestic facility capable of handling contaminated naval tonnage at scale. Ships go to Turkey, Bangladesh, India — jurisdictions with lower standards and no security clearance capability. The Basel Convention increasingly constrains those exports. Defense industrial base modernization requires a domestic solution regardless of CLASP.

The reframing as energy/materials company is structural, not marketing: revenue from output streams (refined steel, recovered alloys, thermal energy, vitrified hazmat) rather than fees for labor. Traditional yards minimize effort; CLASP maximizes material yield.

### Design Robustness
- **Laminar slicing** solves the epistemological problem of unknown vessel state through sequential disclosure. Unknown unknowns become known unknowns at the moment of encounter.
- **Reactive coating** shifts hazmat detection from inferential sensor processing (probabilistic) to binary visual state change (deterministic). Camera classification of binary visual states is a solved problem.
- **Score-before-cut + granulate** are independent sequential controls — belt and suspenders for stochastic liquid release.
- **Phase 0 MVP** generates revenue from toll relationships while building capability, avoiding the cold-start capital problem.

### Key Assumptions
Three critical assumptions, all claimed to be testable in Phase 0:
1. Navy/MARAD market is accessible and sticky
2. Laminar slicing is mechanically feasible at ship scale
3. Indicator coating chemistry can be developed for shipboard conditions

### Competitive Advantage
Regulatory certification is claimed as the moat — takes years to build, cannot be quickly replicated. Hub location adjacent to Nucor EAF (Charleston) creates short logistics chain to premium buyer. Navy/MARAD relationship, once established, is sticky due to continuity/clearance/compliance requirements.

---

## Red Team Attacks

*Ranked by likelihood x impact, most dangerous first.*

### 1. The MVP Has No Moat [HIGH x HIGH]

The $1.5-2.5M "certified aggregation node" owns no processing equipment, performs no hazmat destruction, and subcontracts all value-generating work. Certification is a one-time cost, not a recurring barrier. The moment CLASP demonstrates the regulatory pathway works, any well-capitalized competitor can replicate it. CLASP has handed them a roadmap. The aggregation node phase generates thin broker margins while burning runway. There is no natural lock-in between Phase 1 and Phase 2. Political relationships built during Phase 1 are not exclusive.

**Worst case:** CLASP validates the regulatory pathway, a larger operator enters, and CLASP is priced out before vertical integration.

### 2. OSHA PSM Analogy Is Legally Broken [HIGH x HIGH]

OSHA PSM works because process chemistry is known in advance. Refineries have characterized, stable hazmat inventories. Ship demolition involves unique, partially documented, vessel-specific profiles. More critically: maritime vessels under 46 USC fall under Coast Guard jurisdiction until declared out of service. The handoff moment — when a vessel becomes an industrial worksite rather than a maritime asset — has never been cleanly resolved. Multi-agency jurisdiction (OSHA, EPA TSCA, state DEQ, Coast Guard) means no single certifying authority.

**Worst case:** Multi-year regulatory limbo with no single agency willing to be the certifying authority, each pointing to another.

### 3. Horizontal Laminar Slicing at Panamax Scale Is Unsolved [HIGH x HIGH]

32.3m continuous horizontal cut across a vessel beam. Ships have longitudinal framing; horizontal cuts sever load-bearing frames, causing the remaining hull to shift, list, and settle as mass is removed asymmetrically. Industrial cutting systems for 32m continuous marine cuts don't exist commercially. The "geometry solution" doesn't actually eliminate the information requirement — it defers it to structural modeling that must be continuously updated as cutting proceeds.

**Worst case:** Structural collapse of a partially dismantled vessel with hazmat release.

### 4. Reactive Coating Doesn't Exist at Required Specificity [MEDIUM x HIGH]

Asbestos is a physical fiber — no colorimetric indicator detects fiber presence. PCB detection requires solvent extraction. Radioactive material detection requires radiation interaction. The coating concept conflates fundamentally different detection modalities into a single product that does not exist. Even partial versions face ambiguous color interpretation on corroded, painted, non-uniform surfaces.

**Worst case:** False negatives on hazmat detection, acute worker exposure during cutting.

### 5. Navy/MARAD Pipeline Inaccessible to Startup [MEDIUM x HIGH]

Federal vessel disposal contracts require NAVSEA certification, past performance records, bonding capacity, and environmental liability insurance that no startup can obtain without operating history. Political access is not contract award. Past performance requirements in DoD contracting are structurally exclusionary to first-time entrants without teaming arrangements with cleared incumbents.

**Worst case:** The political window opens, contracts are awarded to established yards, CLASP's beachhead has no entry point.

---

## Adjudication

### Covered by Blue Defense
None fully covered. The blue defense addresses the *concept* of each vulnerability but provides insufficient *evidence* that the mitigations work.

### Genuine Vulnerabilities

| # | Finding | Verdict | Decision Relevance |
|---|---------|---------|-------------------|
| 1 | MVP has no moat | **GENUINE** | HIGH — reshape Phase 0 to prioritize exclusive toll agreements or long-term Navy relationships BEFORE capability is proven |
| 2 | PSM jurisdiction gap | **GENUINE** | HIGH — threshold viability question. Must be answered BEFORE capital raised, not during Phase 0 |
| 3 | Laminar slicing unsolved | **GENUINE but testable** | MEDIUM-HIGH — engineering problem with defined boundaries, not epistemological. Requires explicit kill switch in capital plan |
| 4 | Coating specificity | **GENUINE but scopable** | MEDIUM — scope claim down to specific contaminant class until chemistry validated. Partial functionality still valuable |
| 5 | Navy/MARAD access | **GENUINE** | HIGH — restructure around teaming agreement with NAVSEA-certified incumbent, or the $50-100M/yr figure is not credible |

### What the Red Team Missed

The "orchestrates never executes" model is a double-edged sword. If CLASP owns no execution capability, it is permanently dependent on subcontractor performance and pricing. The orchestrator-only model protects against liability but prevents the vertical integration that Phase 2+ depends on. This structural tension between orchestrator-as-moat and orchestrator-as-dependency was not fully surfaced by either team.

### Single Most Important Finding

**Finding 2 — the PSM jurisdiction gap — is the most important.** Not because it is necessarily fatal, but because the entire CLASP value proposition (certification as moat, regulatory premium, ESG positioning, hazmat fees) rests on the assumption that a coherent certification pathway exists. If no agency has clear authority to issue a PSM-equivalent envelope certification for decommissioned naval vessels, CLASP's differentiation disappears before the first contract is signed.

**Every other finding is conditioned on this one being resolved.** It must be answered before capital is raised, not during Phase 0.

---

## Pre-Phase 0 Requirements (from Adjudication)

Before spending $1 on the MVP, the following must be established:

1. **Regulatory jurisdiction mapping** — Engage OSHA, EPA Region 4/6, and USCG counsel to define the vessel-to-worksite handoff moment and identify the certifying authority for envelope-style operational limits
2. **NAVSEA teaming partner** — Identify and pre-negotiate a teaming arrangement with an existing NAVSEA-certified contractor to access the Navy/MARAD pipeline without past performance history
3. **Moat architecture** — Design Phase 0 to create structural lock-in (exclusive toll contracts, long-term site lease, proprietary process data) before proving the pathway for competitors
4. **Laminar slicing feasibility test** — Define a scaled prototype test with an explicit kill switch: what result means stop?
5. **Coating chemistry scoping** — Engage materials science faculty/lab to establish which contaminant classes are addressable with surface-applied colorimetric detection, and which require alternative methods
