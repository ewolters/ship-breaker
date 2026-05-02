# TRIZ Analysis: Automated Ship Salvage via CLASP Drone Coordination

**Date:** 2026-05-02
**Technique:** TRIZ Contradiction Analysis + Inventive Principles

---

## Contradictions

### Primary — Autonomous Adaptive Sequencing vs. Regulatory Legitimacy

- **Improving:** Adaptability/Versatility (TRIZ #35) — ability to reason from unknown ship state, generate novel sequences, handle undocumented modifications
- **Degrading:** Ease of Operation (TRIZ #33) — institutional operability, ability of regulators and licensed engineers to exercise statutory approval roles
- **Applicable principles:** 1 (Segmentation), 15 (Dynamics), 35 (Parameter Changes), 37 (Differential Response)
- **Statement:** Increasing the system's capacity to adapt to unknown ship state requires emergent, machine-generated decision sequences that structurally exclude the human approval chain mandated by the Hong Kong Convention and ILO conventions.

### Secondary 1 — Containment Robustness vs. Site Universality

- **Improving:** Reliability (TRIZ #27) — mesocosm boundary integrity across operational lifecycle
- **Degrading:** Adaptability/Versatility (TRIZ #35) — deployability across geological site conditions
- **Applicable principles:** 3 (Local Quality), 10 (Preliminary Action), 11 (Beforehand Cushioning), 28 (Mechanics Substitution)
- **Statement:** Increasing containment reliability through validated membrane specifications requires geological conditions (clay substrate, low tidal variance) that directly constrain the range of coastal sites where the system can be deployed.

### Secondary 2 — Sensor Fidelity vs. Confidence Calibration

- **Improving:** Loss of Information (TRIZ #24, inverted) — higher fidelity ground truth in corroded, modified vessel interiors
- **Degrading:** Reliability (TRIZ #27) — reliability of confidence intervals in novel corrosion environments
- **Applicable principles:** 10 (Preliminary Action), 19 (Periodic Action), 24 (Intermediary), 32 (Color Changes / State Change Indicator)
- **Statement:** Pushing recon drone sensors to hardware limits in corroded vessel interiors causes confidence intervals to become unreliable precisely in the novel corrosion cases that matter most for safety-critical sequencing decisions.

---

## Solutions by Principle

### Primary Contradiction Solutions

**Principle 1 — Segmentation**

Decompose the decision sequence into two structurally separate streams: CLASP generates a continuous "intent log" of micro-decisions (cut sequence, flood order, hazmat extraction timing) at machine speed, while a parallel regulatory layer operates only on "phase boundaries" — discrete checkpoints where the system has paused and presented a human-readable state summary. Regulators never approve individual decisions; they approve transitions between defined phases (e.g., Phase 2: Hazmat Extraction Complete -> Phase 3: Structural Deconstruction Authorized). Autonomous adaptation runs freely within phases; human authority governs between phases.

**Principle 15 — Dynamics**

Replace the static pre-approved work plan (which cannot match an undocumented vessel) with a living regulatory instrument: a Continuous Compliance Record (CCR) that updates in real time as CLASP adapts. The CCR is a cryptographically signed, timestamped log that the regulator monitors as a live feed rather than approving in advance. Regulatory legitimacy shifts from pre-authorization of actions to post-auditable traceability of decisions. The Hong Kong Convention obligation is satisfied not by prior approval but by an unbroken chain of documented machine reasoning that any inspector can replay.

**Principle 35 — Parameter Changes**

Change the parameter being regulated. Instead of regulating the decision sequence (which must be adaptive and therefore unknowable in advance), regulators certify the constraint envelope: maximum allowable contamination flux at the mesocosm boundary, minimum structural integrity threshold before cutting, maximum rate of structural change per hour. CLASP can generate any sequence it chooses so long as it stays inside certified parameters. The regulatory object shifts from "what the system does" to "what the system cannot exceed."

**Principle 37 — Thermal Expansion / Differential Response**

Model the approval chain as a differential response mechanism rather than a gate. High-confidence CLASP decisions (novel corrosion pattern within previously mapped range, structural state within baseline variance) self-authorize at machine speed. Low-confidence decisions (corrosion morphology outside training distribution, structural response anomaly) automatically expand the approval requirement — they "thermally expand" into human review. The threshold for expansion is calibrated to the confidence interval output of the sensor fusion layer, creating a continuously variable human-in-the-loop that scales with actual uncertainty rather than applying uniform oversight to all decisions.

### Secondary 1 — Containment Solutions

**Principle 3 — Local Quality**

Rather than specifying a uniform membrane standard for the mesocosm floor, design the containment system as a spatially differentiated layer where membrane grade, thickness, and overlap geometry vary according to local geological survey data. A site with fractured basalt receives a different zone specification than a site with consolidated clay. The regulatory certification shifts from "approved membrane spec" to "approved site characterization methodology plus zone-to-spec mapping algorithm." Any geology can be addressed; the system adapts locally rather than deploying a single universal specification.

**Principle 10 — Preliminary Action**

Before any vessel enters the drydock, deploy a temporary mesocosm validation protocol: introduce a controlled tracer compound (non-toxic, detectable at parts-per-billion) at the drydock floor and monitor for 72 hours at the perimeter. This pre-certifies actual site containment performance under real geological conditions, not modeled ones. A site that fails tracer validation is remediated before the ship arrives. Containment robustness is decoupled from geological assumptions because it is empirically verified on each site before use.

**Principle 11 — Beforehand Cushioning**

Install a secondary containment annulus — a ring of sacrificial absorbent berm material surrounding the primary mesocosm perimeter — before drydock construction begins. If the primary membrane fails due to unanticipated geological shear or subsidence, the annulus captures the contamination pulse before it reaches groundwater. The berm material is selected for the specific contaminant suite of aged vessels (heavy metals, PCBs, asbestos particulate in water suspension). Site universality is preserved because the system compensates for geological variability with a physical buffer rather than requiring the geology to meet a specification.

**Principle 28 — Mechanics Substitution**

Replace the rigid, geology-dependent impermeable substrate with an active hydraulic containment field. A network of extraction wells installed at the drydock perimeter maintains an inward hydraulic gradient — groundwater and any leachate is continuously drawn toward the drydock interior rather than outward. Containment is achieved by fluid mechanics, not membrane integrity. The system works in fractured rock, sandy substrate, and clay alike, because the gradient is maintained by pumping power, not geological impermeability. The subterranean hazmat evacuation system already present in the design serves as the extraction infrastructure.

### Secondary 2 — Sensor Solutions

**Principle 10 — Preliminary Action**

Before deploying recon drones into an unknown vessel interior, introduce a known-state calibration object: a small reference panel fabricated from steel with precisely characterized corrosion stages (mill scale, surface rust, pitting at known depths, through-corrosion) attached to the drone chassis. Every sensor reading taken inside the vessel is simultaneously taken against the reference panel in the same electromagnetic and atmospheric environment. Sensor drift, interference, and environmental degradation are continuously corrected against a ground truth that travels with the drone.

**Principle 19 — Periodic Action**

Replace continuous sensor streaming with a periodic pulse-and-dwell protocol. The drone moves, stops, deploys all sensors simultaneously for a fixed dwell period, records a complete multimodal snapshot, then moves again. During dwell, the system runs an internal consistency check across sensor modalities — if ultrasonic thickness, electromagnetic induction, and visual morphology are mutually consistent, confidence is high; if they diverge, confidence is flagged low and the location is added to a re-survey queue. Continuous streaming masks the divergence signal; periodic snapshots make it visible and actionable.

**Principle 24 — Intermediary**

Insert a physically separate confidence-calibration drone whose sole function is to follow the primary recon drone through each compartment and independently re-measure a sample of the primary drone's readings using different sensor physics (e.g., primary uses ultrasonic; calibrator uses radiographic). The calibration drone produces no new spatial coverage — it only validates what the primary drone already measured. Confidence intervals are derived from the inter-drone agreement rate in that specific corrosion environment rather than from theoretical sensor performance curves.

**Principle 32 — Color Changes / State Change Indicator**

Apply a reactive chemical indicator coating to the interior surfaces of the vessel before the first recon pass. The coating changes color in the presence of specific hazmat compounds (asbestos fiber aerosol, PCB-laden condensate, heavy metal particulate) and also changes texture/reflectivity in response to structural stress. Recon drone cameras now receive a direct, unambiguous visual signal about hazmat presence and structural state that does not rely on inferential sensor processing of corroded steel. In the most degraded and novel corrosion cases — where sensor inference fails — the chemical indicator provides a binary, high-confidence ground truth that the drone's camera reads directly.

---

## Evaluation

### Structural Distinctness

**Primary Contradiction:** All four solutions are genuinely structurally distinct — they attack the contradiction at different joints.

- P1 operates on *temporal partitioning*: autonomy within phases, human authority between them. The system is still fundamentally approval-gated, just at coarser granularity.
- P15 operates on *audit substitution*: it dissolves the pre-authorization requirement entirely by making the reasoning stream inspectable after the fact. This redefines what "regulatory legitimacy" means at a philosophical level.
- P35 operates on *object substitution*: regulators stop governing actions and start governing a parameter space. A category shift, not an optimization.
- P37 operates on *continuous signal*: human involvement is itself an emergent property of runtime state — the only solution where human-in-loop is a real-valued dial driven by the system's own uncertainty output.

P15 and P1 conflict in interesting ways — P15 implies no pre-authorization is needed at all; P1 still requires it at phase boundaries. You cannot fully implement both.

**Secondary 1:** P3 and P28 are structurally opposed and both genuine. P3 accepts geological variability and matches containment *to* it. P28 refuses to accept geological substrate as a variable at all — replacing passive barrier with active field. P10 and P11 are less distinct (both compensatory buffers), though P11 is more structurally interesting because it is always active.

**Secondary 2:** P10 (reference panel) and P24 (calibrator drone) are structurally similar — both use known-state reference to correct for drift. P24 is more powerful because inter-agent agreement is more robust against shared-mode failures. P19 (pulse-and-dwell) is genuinely distinct — self-certifying rather than reference-certifying. P32 is categorically different from all three: it does not improve inference, it eliminates it.

### Direct Resolution vs. Sidestepping

- P1, P37: Address the contradiction directly — they restructure the human-machine boundary
- P15, P35: Sidestep the contradiction — they redefine what "regulatory approval" means
- P28: Sidesteps — eliminates geological dependence rather than resolving it
- P32: Sidesteps — eliminates inferential sensing rather than making it more reliable

### Most Surprising Element

**P32 (reactive chemical indicator coating) is the hardest to reach through conventional thinking.** Every other sensor solution tries to make the existing pipeline more reliable. P32 makes the pipeline unnecessary by *modifying the object being sensed* before sensing begins. The insight: treat the vessel interior as a substrate you can prepare, not a fixed unknown you must read. This is the kind of inversion that conventional engineering improvement cycles never surface — they optimize the sensor, not the sensed.

It also compounds: a reactive coating could simultaneously serve as a calibration reference for P10's reference panel, replacing machined steel standards with a distributed in-situ equivalent.

### High-Value Combinations

**P35 + P37** form a natural pair. P35 defines the constraint envelope (the certified operating space); P37 governs behavior *within* it by scaling human review to confidence. Together: regulators set the walls, the machine fills the space, escalating only when it brushes against them.

**P19 + P24** compound: pulse-and-dwell stops the primary drone for cross-modal internal checking; the calibrator drone arrives during that dwell and conducts inter-drone agreement measurement. The dwell is no longer dead time — it's the calibration window.

**P28 + P11** address failure modes at different scales. P28 (active hydraulic gradient) is primary containment; P11 (sacrificial annulus) catches any hydraulic transient that exceeds pump capacity. Active-plus-passive layering with no single point of failure.
