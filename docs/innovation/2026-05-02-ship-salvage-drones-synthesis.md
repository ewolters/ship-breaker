# CLASP: Concept Synthesis

**Date:** 2026-05-02
**Source Artifacts:** Cross-Domain Transfer, Pre-Mortem, TRIZ Contradiction Analysis, Morphological Analysis
**Status:** Concept-stage synthesis — not a business plan, not a spec. A structured articulation of what the innovation techniques produced.

---

## The Reframe

This is not a ship-breaking company. It is an **energy and materials company that happens to dismantle ships.**

The insight emerged from morphological analysis (Combination 8): when hazmat treatment infrastructure — thermal destruction with heat recovery, pharmaceutical-grade fractionation — sits at a permanent hub, and modular demolition spokes feed it, the value chain inverts. The demolition is the intake process. The products are energy, refined metals, vitrified structural fill (from asbestos fiber), commodity-grade heavy metals, and chlorine-content chemicals. The ship is feedstock.

This reframe changes:
- **The investor pitch** — from "we solve an environmental problem" to "we operate a materials processing facility with a unique, low-cost feedstock supply"
- **The margin structure** — from "we charge for demolition" to "we sell refined outputs and charge a gate fee"
- **The regulatory posture** — from "grant us a demolition permit" to "we are a licensed materials recovery and waste-to-energy facility"
- **The competitive moat** — from "we have better robots" to "we have a vertically integrated supply chain from hull to commodity"

---

## The Architecture

### What We Build

**Hub:** A permanent materials recovery and energy facility at a single high-density scrapping geography. Contains:
- Thermal destruction with heat recovery (rotary kiln, waste-to-energy)
- Fractionation lines (contaminants as feedstock)
- Refined materials output (metals to commodity grade, asbestos vitrification to structural fill, PCB fractions to licensed chemical destruction markets)
- Century-scale monitored vault for irreducible residuals

**Spokes:** Modular demolition berths deployable to vessel graveyard sites or port cities. Each spoke contains:
- A single-berth drydock with containment boundary
- CLASP coordination system with drone fleet (recon, logistics, structural)
- Automated crane array
- Containerized cold-stabilization for hazmat (packaged and shipped to hub)
- 90-day assembly timeline on leased industrial land (where geology permits) or floating pontoon configuration (where it doesn't)

### How We Cut: Horizontal Laminar Slicing

The morphological analysis surfaced the most important architectural decision: **horizontal laminar slicing from top down.**

Every other sequencing approach (guild-succession, scored cue stack, progressive flooding) requires solving the blueprint-reality gap first — you need to know what's inside before you decide the cutting sequence. The premortem identified this gap as the central condition of the work: ships that have been at sea for 30 years have undocumented modifications, fuel tanks where cargo holds should be, remade bulkheads, and corroded structures that scatter LIDAR returns.

Laminar slicing dissolves this problem by converting it from an information problem to a geometry problem. You cut in full horizontal planes progressing downward. Each completed slice is lifted clear before the next plane is scored. The structural load path is never interrupted because each layer is fully supported before the one below it is touched.

You encounter whatever you encounter, one layer at a time. The unknown internal state is not a risk to be managed — it is material to be processed.

This means:
- CLASP's adaptive logic operates within a constrained, predictable geometry rather than reasoning about arbitrary 3D structural relationships
- Sensor requirements are dramatically reduced — you need to characterize one horizontal plane at a time, not an entire vessel interior
- Crane sequencing is simplified — overhead lift of completed slices, not complex multi-axis support of arbitrary vertical segments
- The premortem's "Gothenburg incident" (CLASP issuing a segment-lift on an incorrectly assessed section) becomes structurally impossible — you never commit to a cut based on inference about hidden state below

### How We Sense: Reactive Chemical Indicator Coating + Laminar Geometry

The TRIZ analysis produced the most surprising solution: **modify the object being sensed, not the sensors.**

Before recon drones enter each newly exposed horizontal plane, the surface is sprayed with a reactive chemical indicator coating that:
- Fluoresces at corrosion voids and structural stress concentrations
- Changes color in the presence of asbestos fiber, PCB-laden condensate, heavy metal particulate
- Changes texture/reflectivity in response to structural stress

The recon drones' cameras read the coating directly — a binary, high-confidence ground truth that bypasses the entire inferential sensor processing chain. In the premortem's terms: the LIDAR scattering problem that caused the Gothenburg incident cannot occur because LIDAR is not the primary sensing modality. The ship tells you what's in it.

Laminar geometry compounds this: each newly exposed plane is a flat, accessible surface ideal for spray application and camera-based reading. You never need to send drones into cramped, corroded, partially flooded compartments to build a 3D model. You expose, coat, read, cut.

**Backup sensing** (for coating gaps or ambiguous readings): pulse-and-dwell multimodal consistency checking at flagged locations, with automatic escalation to human review when cross-modal confidence diverges. The differential human-in-loop from the TRIZ P37 solution: high-confidence readings self-authorize; low-confidence readings expand into human review. The threshold is calibrated to actual uncertainty, not applied uniformly.

### How We Contain: Geology-Adaptive Dual Strategy

The premortem identified membrane failure in non-European geologies as a site-specific risk. The TRIZ P28 solution (active hydraulic gradient) and the morph's pontoon skirt option provide two complementary approaches:

**Land-based spokes (pre-qualified geology):** Active hydraulic containment gradient. Extraction wells at the drydock perimeter maintain an inward pressure differential. Containment by fluid mechanics, not membrane integrity. Pre-qualified via tracer compound validation protocol (TRIZ P10) — 72-hour empirical test before any vessel enters.

**Non-qualifying geology or tidal sites:** Floating pontoon enclosure with membrane skirt. Circumferential pontoon ring suspends an impermeable membrane to the seafloor. No land-based geology dependency. Laminar slicing produces predictable debris fall patterns that the skirt geometry handles cleanly.

Both configurations include a sacrificial absorbent annulus (TRIZ P11) as a secondary buffer — catch layer for any transient that exceeds primary containment capacity.

### How We Get Approved: Envelope Certification + Actuarial Pricing

The premortem's most damaging failure mode was regulatory: "you cannot interrupt a regulatory transmission chain the same way you interrupt a contamination transmission chain."

The TRIZ P35 solution resolves this: **change what regulators approve.** Instead of approving the decision sequence (which must be adaptive and therefore unknowable in advance), regulators certify the constraint envelope:

- Maximum allowable contamination flux at the mesocosm boundary
- Minimum structural integrity threshold before cutting
- Maximum rate of structural change per hour
- Abort triggers and safe-state definitions

CLASP can generate any sequence within certified parameters. The regulatory object shifts from "what the system does" to "what the system cannot exceed." The closest existing precedent is **OSHA Process Safety Management (29 CFR 1910.119)** in chemical plants: regulators approve Safe Operating Limits and Mechanical Integrity programs, and the DCS (distributed control system) operates freely within those limits with logged exception handling. This is genuine envelope certification, already legally established for hazardous industrial operations in the US.

The morphological analysis added a second layer: **third-party actuarial authorization.** A licensed indemnity underwriter prices the operation based on probabilistic risk models. This serves two functions:
1. Regulatory acceptance of underwriter sign-off as a legal proxy (precedent: marine insurance already governs vessel operations)
2. Market-based risk discipline — the premium is a continuous feedback signal on operational safety

The morph's evaluator noted that actuarial authorization enforces information architecture coherence downstream: insurers demand auditable triggers (scored performance) and quantified confidence intervals (calibration pairs). The authorization mechanism selects for the sensor and sequencing approach.

### CLASP: The Orchestrator

From the transfer analysis: CLASP is the **expeditor** (cuisine), the **stage manager** (theater), the **keystone regulator** (ecology), the **incident commander** (epidemiology). It orchestrates but never executes. It calls the cue but does not strike the set.

Within the laminar slicing architecture, CLASP's role is constrained and well-defined:
1. **Pre-slice survey:** Dispatch recon drones to characterize the newly exposed horizontal plane (post-coating application)
2. **Hazmat routing:** Identify contamination locations, plan subterranean evacuation routing for this slice
3. **Cut planning:** Generate the cut geometry for this slice within the certified envelope
4. **Crane sequencing:** Queue automated cranes for slice lift-off, with physical-readiness confirmation (state assertion, not message receipt — the premortem's firmware lesson)
5. **Material routing:** Direct logistics drones to sort and containerize slice output — clean steel to materials recovery, hazmat to cold-stabilization for hub shipment
6. **Compliance logging:** Continuous Compliance Record (TRIZ P15) — cryptographically signed, timestamped, inspector-replayable

The adaptive guild-succession logic from the ecology transfer still applies, but operates at a higher level: CLASP sequences the *type* of work (hazmat extraction before structural cutting before materials recovery) within each slice, not the overall vessel decomposition strategy.

---

## Open Questions

These are not showstoppers. They are engineering and business questions that require investigation before this concept advances beyond synthesis.

### Technical
1. **Reactive coating chemistry:** Does a multi-indicator coating exist that can simultaneously signal for asbestos, PCBs, heavy metals, AND structural stress? What's the spray-to-readable time? What's the cost per square meter at vessel scale?
2. **Laminar slicing at scale:** What cutting technology handles a full-beam horizontal plane on a Panamax (32.3m beam)? Plasma? Oxy-fuel? What's the kerf width and how does it affect structural stability of the remaining hull?
3. **Hydraulic gradient energy cost:** Rough estimate: maintaining a 1m inward gradient on a 360x70m berth perimeter at typical coastal hydraulic conductivity is ~50-200 kW continuous, or $0.5-2M/year per spoke at industrial electricity prices. Not catastrophic but shifts breakeven by months — must be priced into economics explicitly.
4. **Fractionation economics and asbestos pathway:** Asbestos vitrification (e.g., Inertam in France) is industrially proven for producing inert glass/structural fill. The stronger claim — resaleable ceramic precursor — requires a specific commercial-grade asbestos-to-feedstock pathway that is not yet established. Default to vitrification with structural fill output unless a feedstock pathway can be cited. What are realistic commodity prices for recovered heavy metals and PCB fraction destruction fees? Is fractionation revenue material or symbolic?

### Regulatory
5. **Envelope certification precedent:** Has any maritime regulatory body accepted envelope-style certification for autonomous industrial operations? What's the closest precedent? Who do you talk to first — IMO, national maritime authority, or port authority?
6. **Public health vs. maritime jurisdiction:** If the facility operates under environmental/public health statutes rather than maritime salvage law, which regulatory body has jurisdiction? Is this a feature (faster approval) or a liability (jurisdictional ambiguity)?

### Commercial
7. **Hub site selection:** Where is the optimal location for the permanent hub? Proximity to vessel graveyards (South Asia), proximity to commodity markets (Europe/East Asia), or proximity to existing waste-to-energy infrastructure?
8. **Spoke economics:** What's the minimum vessel throughput at a spoke to justify 90-day deployment + teardown? How many end-of-life vessels per year are available in each geography?
9. **Competitive response:** How do Chittagong, Alang, and Gadani yards respond? Price competition (they drop gate fees)? Regulatory capture (they lobby against the new framework)? Or adoption (they license the technology)?

### Foundational
10. **Domain immersion requirement:** The premortem's yard owner was clear: "I would have spent six months in this yard first. Not studying. Working." Before any engineering begins, someone needs to spend time in an operating breaking yard understanding the actual work. This is not optional.

---

## What This Is Worth

### As a Concept
The concept has structural novelty in at least three areas that may be patentable or defensible:
- Reactive chemical indicator coating for pre-sensing vessel interior state
- Envelope certification framework for autonomous industrial deconstruction
- Hub-and-spoke materials recovery architecture with ships as feedstock

### As Content
The four source artifacts and this synthesis contain material for:
- A **5-part LinkedIn series** ("What cuisine taught us about ship salvage," "Three ways this fails before it starts," "The contradiction at the center," "15,625 combinations and the three that matter," "It's not a demolition company")
- A **whitepaper** suitable for submission to maritime safety conferences or environmental policy forums
- A **speaking proposal** for maritime industry events, sustainability conferences, or innovation methodology conferences

### As a Conversation Starter
This is the kind of concept that gets you invited into rooms. Maritime safety organizations, environmental NGOs, the IMO's Marine Environment Protection Committee, marine insurers (Lloyd's), and impact investors all have reasons to engage with a concept this developed. The public health reframing alone is a novel policy argument.

---

## The One-Line Pitch

**CLASP is a materials recovery and energy company that processes end-of-life vessels as feedstock — using drone-coordinated horizontal laminar slicing in contained spoke facilities, with hazmat routed to a permanent hub for pharmaceutical-grade fractionation and thermal destruction — replacing the most dangerous and ecologically destructive industry on Earth with a profitable, scalable, certifiable system.**

---

*Generated via: Cross-Domain Analogical Transfer (4 domains) → Pre-Mortem (3 perspectives) → TRIZ Contradiction Analysis (3 contradictions, 12 solutions) → Morphological Analysis (15,625 combinations) → Synthesis*
