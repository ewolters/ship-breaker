# CLASP: Rethinking Ship Recycling as Materials Recovery

**A Concept Study by Svend Research**

*May 2026*

---

*[COVER IMAGE: Wide aerial photograph of Chittagong ship-breaking yards, Bangladesh. Workers visible as specks against rusting hull sections beached in tidal mud. Oil sheen on water.]*

---

## Executive Summary

Ship breaking is the most dangerous and ecologically destructive industry on Earth. Over 700 large ocean-going vessels are scrapped annually, overwhelmingly on the beaches of South Asia, where unprotected workers dismantle them by hand in conditions that poison both people and coastline. The industry persists in this form not because alternatives are impossible, but because no one has engineered an alternative that is profitable.

This report presents CLASP — a concept-stage design for automated ship salvage that reframes the problem entirely. CLASP is not a ship-breaking company. It is an **energy and materials company** whose feedstock acquisition mechanism happens to be ship dismantlement. The products are refined metals, recovered alloys, thermal energy, and vitrified hazmat. The ship is feedstock.

The concept was developed through a structured innovation process: cross-domain analogical transfer from four distant fields, prospective failure analysis, contradiction resolution via TRIZ inventive principles, and morphological design space exploration across 15,625+ configurations. The result is a specific technical architecture, a phased business model starting at $1.5M, three candidate US sites, an honest assessment of five genuine vulnerabilities, and a food-safe chemical detection protocol that costs $200-750 per ship.

This is not a business plan. It is a structured articulation of what systematic thinking produces when applied to an unsolved industrial problem — and a demonstration of the kind of analysis Svend brings to manufacturing and process challenges.

---

## Table of Contents

1. The Problem
2. Why It Stays This Way
3. The Reframe
4. How It Works
5. The Economics
6. Where You Build It
7. What Breaks
8. How We Got Here: The Innovation Process
9. Appendix: Technical Reference

---

## 1. The Problem

*[IMAGE: Close-up of workers cutting steel hull sections with oxy-acetylene torches, no respiratory protection, standing on oily beach sand]*

### A Global Industry Built on Human Suffering

Every year, approximately 700-1,000 large commercial vessels reach the end of their operational lives. Container ships, tankers, bulk carriers, cruise liners — steel structures the size of city blocks, saturated with decades of accumulated hazardous materials: asbestos insulation, PCB-containing caulk and paint, heavy metals in anti-corrosion coatings, residual fuel oils and lubricants in tanks and pipe systems that were never fully drained.

These vessels must be dismantled. The steel is valuable. The hazardous materials must be managed. Someone must do the work.

Today, over 80% of global ship recycling tonnage is processed on the tidal beaches of three countries: Bangladesh (Chittagong), India (Alang-Sosiya), and Pakistan (Gadani). The method has not fundamentally changed in decades: ships are driven onto beaches at high tide, and armies of workers — often hundreds per vessel — cut them apart with hand-held torches over weeks or months.

*[IMAGE: Wide shot of Alang ship-breaking beach — dozens of partially dismantled vessels stretching to the horizon]*

### The Human Cost

The International Labour Organization estimates that ship breaking in South Asia has one of the highest occupational mortality rates of any industry globally. Workers are exposed to:

- **Asbestos fibers** released during cutting of insulated compartments, pipes, and engine rooms — with latency periods of 20-40 years before mesothelioma diagnosis
- **Heavy metal dust** (lead, cadmium, chromium) from paint and coating systems liberated by torch cutting
- **PCB contamination** from cutting through caulk joints, electrical insulation, and capacitor housings
- **Hydrocarbon exposure** from residual fuel oils, lubricants, and hydraulic fluids that pool on beach sand as vessels are cut open
- **Structural collapse** when hull sections are cut without adequate shoring or engineering analysis

Falls, burns, crushing injuries, and acute chemical exposure are routine. The workers are overwhelmingly poor, often migrants, with no health insurance and limited access to medical care. The long-latency diseases — cancers, respiratory failure, neurological damage — appear years after employment ends, far from the yards, uncounted in industry statistics.

*[IMAGE: Workers carrying asbestos insulation material without respiratory protection]*

### The Ecological Cost

The beaches themselves become sacrifice zones. Fuel oils, lubricants, heavy metals, PCBs, and asbestos wash into tidal waters with every tide cycle. Sediment contamination persists for decades after a yard closes. Marine ecosystems in the immediate vicinity of major breaking yards show heavy metal concentrations orders of magnitude above background levels.

The Hong Kong International Convention for the Safe and Environmentally Sound Recycling of Ships was adopted in 2009. It entered into force in June 2025. Compliance remains minimal. The economics of the industry resist regulation because the margins are built on the externalization of precisely the costs the convention seeks to internalize.

---

## 2. Why It Stays This Way

*[IMAGE: Aerial view comparing a South Asian beach yard with a European dry-dock facility — scale and infrastructure contrast]*

### The $6 Million Structural Disadvantage

The persistence of beach breaking is not a moral failure. It is an economic structure.

Bangladesh yards **receive** $475-490 per Light Displacement Tonne (LDT) from the shipowner. The owner is paid to dispose of the vessel — the scrap value exceeds the cost of the work because the cost of the work is kept artificially low by externalizing safety, environmental, and health costs.

US yards, by contrast, **charge** the owner approximately $50-150/LDT. The shipowner pays for disposal.

For a typical 10,000 LDT vessel, this represents a **$500-650/LDT swing — roughly $6 million per ship** of structural disadvantage for any operation that complies with Western safety and environmental standards.

### Where the Gap Actually Lives

The common assumption is that the gap is labor cost. It is not — at least, not primarily.

| Cost Category | Bangladesh Yard | US Automated Facility | Gap per Ship |
|---|---|---|---|
| Labor | ~$20-50K | ~$200-400K | ~$200-400K |
| Hazmat treatment | ~$0 (dumped) | ~$300-500K | ~$300-500K |
| Capital amortization | Minimal | ~$300-500K | ~$300-500K |
| Insurance + compliance | Minimal | ~$100-200K | ~$100-200K |
| **Legitimate cost difference** | | | **~$1-1.5M** |

The legitimate cost difference — the real cost of doing this work safely — is approximately $1-1.5 million per ship. The remaining $4-5 million of the $6 million gap is **pure rent extraction through regulatory arbitrage**: the value of being allowed to skip everything Western jurisdictions would require.

This distinction matters. A $1-1.5 million cost disadvantage is closeable through technology, throughput, and revenue optimization. A $6 million disadvantage is not. The common narrative — "it's impossible to compete with South Asian labor costs" — confuses the two.

### Why Automation Alone Doesn't Solve It

Previous proposals for automated ship recycling have focused on replacing labor with machines — robotic cutting systems, automated cranes, drone-based inspection. These proposals address the labor cost component (~$200-400K gap) while ignoring the hazmat treatment cost ($300-500K), the capital amortization ($300-500K), and the fundamental question of revenue model.

An automated demolition yard is still a demolition yard. It charges for disposal. It competes on cost with operations that externalize most of their costs. This is a losing proposition regardless of how efficient the automation is.

The question is not "how do we automate ship breaking?" The question is "what business model makes hazmat management profitable?"

---

## 3. The Reframe

*[IMAGE: Modern materials recovery facility — clean, industrial, automated sorting lines]*

### It's Not a Ship-Breaking Company

CLASP is not a demolition operation with better robots. It is an **energy and materials company** that processes end-of-life vessels as feedstock.

This reframe emerged from systematic morphological analysis of the design space (see Section 8). When hazmat treatment infrastructure — thermal destruction with heat recovery, chemical fractionation, metal refining — sits at a permanent processing hub, and modular demolition berths feed it with sorted material streams, the value chain inverts:

- **The demolition is the intake process.** It is how feedstock arrives.
- **The products are the business.** Refined metals, recovered alloys, thermal energy, vitrified structural fill.
- **The ship is feedstock.** A chemically complex but predictable input to a materials recovery operation.

This changes everything downstream:

| Dimension | Demolition Company | Materials Recovery Company |
|-----------|-------------------|---------------------------|
| Investor pitch | "We solve an environmental problem" | "We operate a processing facility with unique feedstock" |
| Margin structure | Charge for disposal | Sell refined outputs + gate fee |
| Regulatory posture | "Grant us a demolition permit" | "We are a licensed materials recovery facility" |
| Competitive moat | "We have better robots" | "We have a vertically integrated supply chain" |
| Revenue dependency | Ship disposal fees | Multiple output streams + external feedstock |

### Hub-and-Spoke Architecture

The architecture follows directly from the reframe:

**Hub:** A permanent materials recovery and energy facility at a single location. Contains thermal destruction with heat recovery, fractionation lines, metal sorting and refining, asbestos vitrification, and monitored storage for irreducible residuals. The hub is the business.

**Spokes:** Modular demolition berths deployable to port cities or vessel graveyard sites. Each spoke contains a single-berth drydock with containment boundary, the CLASP coordination system with drone fleet, automated crane array, and containerized hazmat stabilization for shipment to the hub. Spokes are the intake mechanism.

The hub processes not only ship-derived material but also **external feedstock** — industrial hazmat from other sources. This means the hub's utilization is not limited by ship arrival rates. The ship demolition operation is one input among many, and the materials processing operation stands on its own economics.

---

## 4. How It Works

*[IMAGE: Industrial dry-dock facility, aerial view — clean, structured, organized]*

### Horizontal Laminar Slicing

The single most important architectural decision in the CLASP concept is how vessels are physically dismantled: **horizontal laminar slicing from top down.**

Every other proposed ship recycling method — whether manual or automated — requires knowing what is inside the vessel before deciding how to cut it. This is the fundamental challenge: ships that have been at sea for 30 years bear little resemblance to their original documentation. Bulkheads have been moved, fuel tanks added where cargo holds once were, engine rooms rebuilt, asbestos applied and re-applied by whoever was cheapest in whatever port the ship was last repaired. The gap between blueprint and reality is not noise to be filtered. It is the central condition of the work.

Horizontal laminar slicing dissolves this problem by converting it from an information problem into a geometry problem.

The vessel is cut in full horizontal planes progressing downward. Each completed slice — a layer spanning the full beam of the ship — is lifted clear by overhead cranes before the next plane is scored. The structural load path is never interrupted because each layer is fully supported before the one below it is touched.

**You encounter whatever you encounter, one layer at a time.** The unknown internal state is not a risk to be managed — it is material to be processed.

This means:
- The coordination system operates within a constrained, predictable geometry rather than reasoning about arbitrary 3D structural relationships
- Sensor requirements are dramatically reduced — you characterize one horizontal plane at a time, not an entire vessel interior
- Crane sequencing is simplified — overhead lift of completed slices, not complex multi-axis support
- The risk of cutting into an unknown hazmat pocket is managed by the score-before-cut protocol (below)

### The Seven-Step Slice Cycle

Each horizontal slice follows a defined operational sequence:

**1. Coat.** After each slice is lifted clear and a new horizontal plane is exposed, the surface is sprayed with food-safe indicator dyes via agricultural sprayer drone (DJI Agras T30/T40 platform). Three dyes, applied sequentially:
- **Fluorescein** (FDA-approved food and ophthalmic dye) — enhances hydrocarbon fluorescence under blue light
- **Curcumin** (turmeric extract, GRAS food ingredient) — turns from yellow to red-brown in the presence of lead-based paint
- **Methylene blue** (FDA-approved pharmaceutical) — retained by asbestos mineral fibers, washes off organic surfaces

All three are safe enough to eat, drink, or put in human eyes. Total reagent cost per slice: $6-15. Total per ship: $200-750.

**2. Read.** Recon drones image the treated surface under multiple lighting conditions: UV (365nm) for hydrocarbon autofluorescence, blue light (490nm) for fluorescein-enhanced oil detection, visible light for curcumin and methylene blue signals, and FLIR thermal for hidden liquid reservoirs. CLASP composites these into a false-color hazmat map of the exposed plane.

For PCBs — the one contaminant class with no food-safe spray indicator — a conservative zone protocol treats all pre-1979 caulk joints and electrical insulation as PCB-positive. Post-1979 ambiguous zones are checked by drone-mounted XRF analyzer.

**3. Score.** Before the full slice cut, the cutting gantry makes a shallow scoring pass (10-20mm) across the plane. This allows any pressurized reservoirs — fuel tanks, hydraulic lines, sealed compartments — to weep their contents toward the catch basin in a controlled, low-energy release rather than a sudden breach during full cutting. This technique, drawn from French culinary practice ("parer au vif" — probe before you plunge), converts a stochastic hazmat event into a managed pre-release.

**4. Drain.** Liquid released during scoring flows by gravity into the full-width catch basin beneath the cut zone, fitted with retractable bulkheads positioned based on the hazmat map from Step 2.

**5. Granulate.** At the basin floor, absorbent granulate dispensers automatically convert liquid hazmat to a handleable semi-solid. This eliminates the liquid phase from all downstream handling — no liquid conveyance infrastructure, no spill risk in transit. The entire facility operates as a single-phase solid-handling system.

**6. Cut.** The cutting gantry completes the full horizontal slice. Six material streams are segregated at the point of generation:
- Clean steel (sorted by alloy via XRF at exit gate)
- Contaminated steel (flagged by indicator dyes)
- Granulated liquid hazmat (sealed containers)
- Solid hazmat (vacuum-extracted by gantry hoods)
- Non-ferrous metals (copper, aluminum, brass — sorted by sensor)
- Machinery and equipment (cranes to staging area)

**7. Lift.** Overhead cranes lift the completed slice clear. The cycle repeats.

*[DIAGRAM: Seven-step slice cycle illustrated as a circular process flow]*

### CLASP: The Coordinator

CLASP — the central coordination system — orchestrates the entire operation but never directly executes any physical action. It is the expeditor in a kitchen brigade: it calls every cue, sequences every action, prevents collisions, but does not touch the food.

Within the laminar slicing architecture, CLASP manages:
- Pre-slice survey dispatch and hazmat map generation
- Cut geometry planning within certified operating envelope
- Crane sequencing with physical-readiness confirmation
- Material stream routing and containerization
- Continuous compliance logging (cryptographically signed, inspector-replayable)

The coordination model is governed by **envelope certification** modeled on OSHA Process Safety Management (29 CFR 1910.119) — the same regulatory framework that governs distributed control systems in US chemical plants. Regulators certify the constraint boundaries (maximum contamination flux, minimum structural integrity, abort triggers), not individual decision sequences. CLASP operates freely within certified parameters.

---

## 5. The Economics

*[IMAGE: Split comparison — beach breaking yard vs. modern industrial facility]*

### Revenue Streams

The CLASP hub-and-spoke model generates revenue from five sources, reducing dependency on any single stream:

**1. Hazmat Treatment and Destruction Fees**
- PCBs at $1,000-3,000/tonne destruction fees
- Asbestos vitrification at $400-800/tonne
- Contaminated marine oils at $200-500/tonne
- Typical end-of-life vessel: 50-200 tonnes treatable hazmat
- **Per-ship revenue: $50-600K**
- Critical: the hub treatment line accepts **external non-ship feedstock**, so throughput is not limited by vessel arrival rate

**2. ESG-Premium Dismantlement**
- Major shipping lines (Maersk, MSC, NYK) already pay above-market for compliance under the EU Ship Recycling Regulation
- Certified clean-dismantle premium of $100-200/LDT plausible for owners with public sustainability commitments
- **Per-ship premium: $1-2M** on a 10,000 LDT vessel

**3. US Navy and MARAD Captive Market**
- US government vessels must be dismantled domestically
- ~$50-100M/year in contracts, currently served by a small number of fragmented yards
- CLASP competes on safety metrics and throughput speed, not just price

**4. High-Grade Material Recovery**
- Properly separated, decontaminated steel sorted by alloy sells at $50-150/tonne premium over commodity scrap
- Horizontal laminar slicing preserves alloy separation by processing one layer at a time
- Alloy-sorted steel feeds directly back into the shipbuilding supply chain — a circular defense industrial base

**5. Federal Cost-Sharing**
- IRA clean energy provisions, EPA brownfield/Superfund tie-ins, port infrastructure grants
- Hub and spoke buildout plausibly 30-50% federally cost-shared

### The Phased Build

The traditional approach to industrial facility development — design fully, build fully, then begin operations — requires $50-80M in capital committed before any revenue is generated. CLASP inverts this through a phased approach that generates revenue before full buildout:

| Phase | Timeline | Cumulative Capex | What You Build |
|-------|----------|-----------------|----------------|
| **Phase 0: Beachhead** | Months 0-6 | $1.5-2.5M | Brownfield lease, leased sort/shear/bale equipment, port authority license, toll processing contracts. First revenue month 3. |
| **Phase 1: Certification** | Months 6-18 | $5-8M | Certified grading and decontamination line, XRF fleet. Defense contractor qualification. Revenue quality jumps 15-30%. |
| **Phase 2: Thermal** | Months 18-36 | $7-12M | Shared cooperative thermal unit or containerized pyrolysis. Hub begins direct hazmat processing. Margin capture increases. |
| **Phase 3: Full Capability** | Year 3-5 | $12-26M | On-site furnace (if throughput justifies), permanent structures, plasma vitrification. Built on proven revenue, not assumptions. |

The key insight from morphological analysis of the plant design: **the hub in Phase 0 is a certified aggregation node, not a processing plant.** Thermal destruction and asbestos handling stay at toll processors or spoke facilities. The hub certifies, sorts, and sells. This requires compliance staff, a quality system, and a covered staging area — not a $50M construction project.

### Labor Productivity

| Metric | Traditional Beach Yard | CLASP Automated |
|--------|----------------------|-----------------|
| Workers per yard | 300-600 | ~80 |
| Ships per year | 5-15 | ~10 |
| Worker-years per ship | 30-90 | 5-20 |
| **Productivity improvement** | | **5-10x** |

### The Variable That Swings the Answer

Whether hazmat treatment can stand on its own as a **profit center independent of ship arrivals.**

If yes: CLASP is an industrial recycler whose feedstock acquisition mechanism happens to be ship dismantlement. The unit economics change qualitatively.

If no: CLASP is a subsidized boutique operation that survives on Navy contracts and ESG premiums — viable but not transformational.

---

## 6. Where You Build It

*[IMAGE: US Gulf Coast industrial port — cranes, vessels, industrial infrastructure]*

### Three Candidate Sites

Morphological analysis of the site selection design space (4,096 combinations across six dimensions) identified three leading configurations, each with distinct advantages:

### Louisiana: The Avondale Play

**Site:** Former Avondale Shipyard (Westwego, LA) — a Northrop Grumman shipbuilding facility closed in 2014.

| Dimension | Assessment |
|-----------|-----------|
| Port access | Deep-water Mississippi River, 40+ ft draft |
| Regulatory | Louisiana TSDF corridor — established precedent for thermal destruction and hazmat processing permits |
| Site readiness | Existing industrial infrastructure: drydock, power, rail, cleared acreage, industrial zoning |
| Federal contracts | Within Gulf Coast NAVSEA contracting orbit; Huntington Ingalls (Pascagoula) proximity |
| Commodity offtake | Mississippi River cement kilns for vitrified residue; Gulf Coast EAF mills |
| Labor | Rural employer-of-choice premium in a low-cost labor market |

**Strength:** Regulatory precedent. Louisiana has the most established TSDF permitting history of any candidate state. The permitting argument is partially won before the application is filed.

### Mississippi: The Fast-Track

**Site:** Moss Point or Chickasaw industrial corridor near Pascagoula.

| Dimension | Assessment |
|-----------|-----------|
| Port access | Deep-water via Pascagoula River |
| Regulatory | Thin regulatory staffing = faster permit queues; state actively courts industrial investment |
| Site readiness | Acquire an operating scrap yard — existing RCRA familiarity, metal handling equipment, buyer relationships |
| Federal contracts | Huntington Ingalls is literally there; direct NAVSEA Gulf Coast access |
| Commodity offtake | Southeast EAF belt (Nucor Tuscaloosa) within 300 miles |
| Labor | Rural employer premium; 80 jobs at $55-75K = best industrial employer in the county |

**Strength:** Speed. An operating scrap yard acquisition can close in 90 days with existing permits. Fastest path from decision to first revenue.

### South Carolina: The Steel Advantage

**Site:** North Charleston industrial corridor (former Charleston Naval Shipyard BRAC site).

| Dimension | Assessment |
|-----------|-----------|
| Port access | Charleston harbor, established naval and commercial port infrastructure |
| Regulatory | SC DHEC comparable to Virginia DEQ; defense-familiar |
| Site readiness | Former naval shipyard with existing drydock infrastructure |
| Federal contracts | Strong Armed Services Committee representation; between Hampton Roads and Gulf Coast orbits |
| Commodity offtake | **Nucor Berkeley County EAF mill is in the same metro area** |
| Labor | Charleston defense industrial base + military transition pipeline |

**Strength:** Commodity offtake. Having a Nucor EAF mill in the same metro eliminates steel transport cost entirely and enables just-in-time alloy-sorted delivery at premium pricing. This is a structural margin advantage no other site matches.

### The Two-Phase Strategy

The site selection morph revealed that the federal contracting dimension splits into two distinct phases: **authorization** (years 0-2, where DC proximity matters for MARAD contracts and IRA cost-sharing) and **execution** (years 3+, where port access and commodity offtake matter). No single site optimizes both.

This points toward a two-phase approach: a policy and contracting office near Washington during the authorization window, with the operational hub at whichever Gulf Coast or Southeast site offers the strongest execution economics.

---

## 7. What Breaks

*[IMAGE: Industrial facility with caution signage — communicating honest risk assessment]*

Honest assessment of vulnerabilities is not a weakness in a concept document. It is the section that earns trust. The following genuine vulnerabilities were identified through structured adversarial analysis (red team / blue team exercise with independent attack and defense perspectives).

### Vulnerability 1: The Regulatory Jurisdiction Gap

**The single most important finding.**

The entire CLASP value proposition — certification as competitive moat, regulatory premium pricing, ESG positioning — rests on the assumption that a coherent regulatory certification pathway exists. OSHA Process Safety Management (29 CFR 1910.119) provides the closest precedent, but ship demolition involves a jurisdictional complexity that chemical plants do not: the Coast Guard has authority over maritime vessels under 46 USC until they are declared out of service, at which point OSHA and EPA assume jurisdiction. The handoff moment has never been cleanly resolved for demolition operations.

Multiple agencies (OSHA, EPA TSCA, state DEQ, Coast Guard) have overlapping authority. No single agency has clear mandate to issue envelope-style certification for autonomous ship demolition.

**Pre-Phase 0 requirement:** Formal legal analysis with OSHA, EPA regional counsel, and USCG to define the vessel-to-worksite handoff and identify the certifying authority. If this cannot be resolved, the PSM framing collapses.

### Vulnerability 2: The Moat Problem

The Phase 0 MVP — a certified aggregation node that owns almost no processing equipment — generates thin broker margins while proving the regulatory and commercial pathway. The risk: once CLASP demonstrates the pathway works, a well-capitalized competitor can replicate the certification and outscale CLASP before it vertically integrates.

**Pre-Phase 0 requirement:** Design Phase 0 to create structural lock-in — exclusive toll processing agreements, long-term Navy/MARAD teaming arrangements, site lease with right of first refusal — before the pathway is proven. Lock-in must be architectural, not incidental.

### Vulnerability 3: Laminar Slicing at Scale

Horizontal laminar slicing across a Panamax beam (32.3m) using industrial cutting systems is an unsolved engineering problem at commercial scale. Ships are designed with longitudinal framing; horizontal cuts sever load-bearing members, causing the remaining hull to shift and deform as mass is removed. This is a genuine engineering unknown.

**Pre-Phase 0 requirement:** Scaled prototype test on a decommissioned vessel section, with an explicit kill switch: defined failure criteria that halt the program if structural integrity cannot be maintained during progressive horizontal mass removal.

### Vulnerability 4: Navy/MARAD Pipeline Access

Federal vessel disposal contracts require NAVSEA certification, past performance history, bonding capacity, and environmental liability insurance — barriers that are structurally exclusionary to first-time entrants.

**Pre-Phase 0 requirement:** Identify and pre-negotiate a teaming arrangement with an existing NAVSEA-certified contractor. This is the standard entry path for defense startups and is well-understood by the contracting community.

### Vulnerability 5: Indicator Chemistry Specificity

The food-safe detection protocol (fluorescein, curcumin, methylene blue) addresses hydrocarbons, lead-based paint, and asbestos fiber. PCB detection has no food-safe spray indicator and must be handled by conservative zone protocol or instrumental (XRF) methods. The curcumin/lead pathway requires bench validation on marine-grade corroded steel substrates.

**Pre-Phase 0 requirement:** Materials science bench validation on representative marine samples — not to develop new chemistry, but to confirm that established food-safe indicators produce camera-resolvable signals on the specific substrates encountered in ship demolition.

### The Pre-Phase 0 Research Agenda

These five requirements constitute a bounded research agenda:

| Investigation | Estimated Cost | Timeline |
|---|---|---|
| Regulatory jurisdiction mapping | $30-50K (legal counsel) | 3-6 months |
| NAVSEA teaming partner | $10-20K (BD/outreach) | 2-4 months |
| Moat architecture design | Internal (business strategy) | 1-2 months |
| Laminar slicing prototype test | $50-100K (vessel section test) | 4-8 months |
| Indicator chemistry bench validation | $15-30K (materials science lab) | 2-4 months |
| **Total pre-Phase 0 investment** | **$100-200K** | **6-8 months** |

If any investigation returns a negative result, the program halts with $100-200K invested rather than $1.5M+. If all return positive, capital is raised with five de-risked assumptions rather than five open questions.

---

## 8. How We Got Here: The Innovation Process

*[IMAGE: Abstract — connected nodes, structured thinking, methodology]*

### The Provenance Chain

The CLASP concept was not designed in a single brainstorming session. It was produced through a structured sequence of innovation techniques, each building on the output of the last. The techniques are drawn from established innovation methodology (TRIZ, morphological analysis, prospective hindsight) and implemented as AI-assisted structured analysis.

The value of showing this process is not academic. It demonstrates that a concept this specific and this internally consistent can be produced *reproducibly* from a starting prompt. The methodology is the transferable asset — applicable to any unsolved industrial problem.

### Technique 1: Cross-Domain Analogical Transfer

**Starting point:** "Drones coordinating ship salvage in a contained drydock."

**Method:** Four experts from distant domains (cuisine, epidemiology, theater, ecology) each solved the problem independently within their own field's vocabulary, never seeing each other's output.

**Key outputs:**
- From **cuisine**: the CLASP coordinator maps to the *expeditor* in a French kitchen brigade — a single intelligence that sequences all action but never touches the food
- From **epidemiology**: ship breaking is not a demolition problem but a *public health intervention* interrupting a contamination transmission chain
- From **theater**: safety comes from converting demolition into a *scored performance* — a cue-by-cue sequence with confirmation gates, not freelance decision-making
- From **ecology**: the closed drydock substrate (mesocosm boundary) is not a feature of the facility — it *is* the entire intervention

**Convergent finding:** Three of four domains independently concluded that removing humans from the high-consequence contact zone is the load-bearing design choice, not an optimization.

### Technique 2: Pre-Mortem Analysis

**Method:** Three stakeholders (impact investor, Chittagong yard owner, CLASP chief engineer) each wrote a detailed post-mortem narrative from one year in the future, after the project had failed spectacularly. They did not communicate.

**Key outputs:**
- The investor identified *institutional legitimacy* as a parallel system to physical containment — "you cannot interrupt a regulatory transmission chain the same way you interrupt a contamination transmission chain"
- The yard owner identified the *blueprint-reality gap* as the central condition: "the gap between blueprint and reality is not an edge case to be calibrated away"
- The chief engineer identified *confirmation semantics* — the difference between "message received" and "ready to act" in the crane control protocol

**Critical finding:** The three narratives blamed three completely different root causes. The failure was *over-determined* — fixing any single cause would leave the others intact. This meant the design had to address all three domains simultaneously.

### Technique 3: TRIZ Contradiction Analysis

**Method:** The core contradiction — "improving autonomous adaptive capability degrades regulatory legitimacy" — was mapped to TRIZ engineering parameters. Twelve concrete solutions were generated from the applicable inventive principles.

**Key outputs:**
- **Envelope certification** (Principle 35: Parameter Changes) — change the regulated parameter from "what the system does" to "what the system cannot exceed"
- **Reactive chemical indicator coating** (Principle 32: Color Changes) — modify the vessel to be readable rather than building better sensors
- **Active hydraulic containment** (Principle 28: Mechanics Substitution) — replace geology-dependent membranes with pumping-based containment

**Most surprising finding:** Principle 32 was the hardest to reach through conventional thinking. Every other sensor solution tries to make the sensor pipeline better. P32 eliminates the pipeline by modifying the object being sensed.

### Technique 4: Morphological Analysis

**Method:** The design space was decomposed into six orthogonal dimensions with 4-5 options each, producing 15,625 possible configurations. Eight random combinations were mechanically enumerated and evaluated.

**Key outputs:**
- **Horizontal laminar slicing** dissolves the blueprint-reality gap by converting an information problem into a geometry problem — surfaced only through combinatorial evaluation, not holistic thinking
- **The authorization model cascades into everything** — the choice of regulatory framework constrains viable sensor and sequencing approaches
- **"It's an energy company"** — the hub-and-spoke reframe with thermal destruction at the hub emerged from a combination (Combination 8) that nobody would have designed holistically

**The combinatorial insight:** The most important finding — horizontal laminar slicing — was invisible when sequencing was considered in isolation. It appeared only when the full combinatorial space was explored mechanically. This is the value of morphological analysis: it finds configurations that holistic "best idea" thinking cannot reach.

### The Chain Effect

Each technique's output sharpened the next technique's input:

```
Transfer (expanded the frame)
    → Pre-Mortem (stress-tested it, found over-determined failure)
        → TRIZ (resolved the contradictions the pre-mortem surfaced)
            → Morph (enumerated the design space using solutions from all three)
                → Synthesis (committed to specific architecture)
                    → Logistics Transfer + Morph (operational detail)
                        → Site Selection + Plant Design (commercial specificity)
                            → Red/Blue (adversarial validation)
                                → Chemistry Spec (bench-ready protocol)
```

The synthesis is not a summary of the techniques. It is a new object that did not exist in any individual artifact. An analogical move (ship breaking as lamb butchery) survived through systematic critique, contradiction resolution, and combinatorial pressure-testing into a specific engineering specification. That provenance chain — from distant analogy to operational protocol — is itself the demonstration of the methodology.

---

## 9. Appendix: Technical Reference

### A. The Indicator Chemistry Protocol (v2 — Food-Safe)

| Target | Reagent | Safety Grade | Signal | Method |
|--------|---------|-------------|--------|--------|
| Hydrocarbons (prelim) | None | N/A | UV autofluorescence | 365nm UV camera |
| Hydrocarbons (confirmed) | Fluorescein sodium | FDA food/ophthalmic | Green fluorescence | 490nm excitation |
| Thermal anomalies | None | N/A | Temp differential | FLIR camera |
| Lead paint | Curcumin (turmeric) | GRAS food ingredient | Yellow → red-brown | Visible camera |
| Asbestos fiber | Methylene blue | FDA pharmaceutical | Blue stain retention | Visible camera |
| PCBs | N/A (no safe spray) | N/A | Chlorine signature | XRF instrument |

**Application platform:** DJI Agras T30/T40 agricultural sprayer drone (30-40kg payload, 16 nozzles, GPS-guided coverage). Reagent cost per ship: $200-750.

### B. Slice Cycle Timing

| Step | Action | Duration |
|------|--------|----------|
| Coat | Spray three dye layers sequentially | 25 min |
| Read | Multispectral imaging (UV, blue, visible, FLIR) | 10 min |
| Score | Shallow scoring pass for controlled pre-release | 5 min |
| Drain | Gravity drainage to catch basin | 5 min |
| Granulate | Absorbent conversion of liquid to solid | 5 min |
| Cut | Full horizontal slice | Variable |
| Lift | Overhead crane removal | Variable |

Characterization time (~55 min) runs in parallel with crane operations on the previous slice.

### C. Material Stream Routing

| Stream | Conveyance | Destination |
|--------|-----------|-------------|
| Clean steel (by alloy) | Dedicated conveyor | Metal sorting/refining |
| Contaminated steel | Separate dedicated conveyor | Decontamination baths |
| Granulated liquid hazmat | Sealed containers | Thermal destruction / fractionation |
| Solid hazmat | Vacuum extraction + pneumatic | Thermal destruction |
| Non-ferrous metals | Pneumatic + conveyor hybrid | Metal sorting/refining |
| Machinery/equipment | Flatbed (as-needed) | Staging/assessment |

### D. Innovation Artifacts

The complete innovation chain is published at:
**github.com/ewolters/ship-breaker**

All artifacts are available for review, comment, and critique.

---

*This report was produced by Svend Research using structured innovation techniques implemented as AI-assisted analysis. The concept is published for discussion and commentary. Technical claims require the bench validation described in Section 7 before any commitment of capital.*

*For questions or collaboration inquiries: eric.wolters@svend.ai*

---

**SVEND** — Process intelligence for manufacturing.

*svend.ai*
