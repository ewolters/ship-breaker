# Inter-Plant Logistics: Operational Synthesis

**Date:** 2026-05-02
**Source Artifacts:** Cross-Domain Transfer (semiconductor, ER, kitchen, hydrology), Morphological Analysis (4,096 combinations)
**Status:** Concept-stage operational design — how material actually moves from ship to hub

---

## The Core Insight

All four transfer domains converged on the same principle: **segregate at the point of generation, never downstream.** Every meter a stream travels before classification increases separation cost and contamination risk. The morph then surfaced a second insight that amplifies the first: **convert liquid hazmat to solid at the point of generation, and the entire facility becomes a single-phase handling system.**

These two principles together define the logistics architecture.

---

## How a Slice Cycle Works

Each horizontal laminar slice follows this sequence. CLASP orchestrates; the physical infrastructure does the routing.

### Phase 0: Pre-Cut Survey (Score Before You Cut)

Before the full slice cut, the cutting gantry makes a **shallow scoring pass** across the exposed horizontal plane — the "parer au vif" technique from the kitchen transfer. This 10-20mm score:

- Allows any pressurized reservoirs (fuel tanks, hydraulic lines, sealed compartments) to **weep their contents toward the catch basin** in a controlled, low-energy release rather than a sudden high-volume breach
- The reactive chemical indicator coating (applied during recon) has already flagged hazmat zones — the score pass targets those zones first
- Liquid releases drain by gravity into the **full-width catch basin** beneath the active cut zone
- CLASP logs weep locations and volumes, updating the predictive model for this slice

This converts the stochastic liquid hazmat problem — the thing that caused the fictional "Gothenburg incident" in the premortem — into a **managed, low-pressure pre-release event.** The full cut never plunges into an unknown pocket.

### Phase 1: Full Cut and Intercept

The cutting gantry completes the horizontal slice. As material separates:

**Liquids** (fuel oil, lubricants, hydraulic fluid, bilge water):
- Drain by gravity into the full-width catch basin beneath the cut zone
- The catch basin has retractable bulkheads that were positioned before cutting based on the pre-cut survey
- At the basin floor: **absorbent granulate dispensers** automatically release granulate into liquid pools, converting liquid to a handleable semi-solid within minutes
- This eliminates the liquid phase from all downstream handling — no liquid conveyance, no spill risk in transit, no dual-phase infrastructure
- Granulate-laden containers are sealed and labeled at the basin (hazmat jurisdiction transfers at sealing)

**Clean steel:**
- Cut sections are lifted by overhead crane to the **dedicated steel conveyance line** (parallel run to hub)
- Automated XRF sensors at the exit gate classify alloy type and gate to the correct sorting lane
- Classification is sticky — rerouting requires CLASP supervisory override

**Contaminated steel:**
- Sections flagged by the reactive coating (or by the worst-case protocol for known hazmat zones) route to a **separate dedicated contaminated line**
- Direct to decontamination baths at hub
- No shared infrastructure with clean steel at any point

**Solid hazmat** (asbestos, PCBs, lead paint):
- Collected by vacuum hoods on the cutting gantry during the cut (negative-pressure extraction captures airborne particulates at source)
- Deposited into sealed hazmat drums at the gantry
- Drums transfer to **pneumatic tube system** for rapid transit to hub thermal destruction endpoint
- For bulk solid hazmat (large insulation sections), dedicated parallel conveyor

**Non-ferrous metals** (copper, aluminum, brass):
- Sorted at intercept by XRF sensor array
- Pneumatic tube for small-volume streams (fittings, wire bundles)
- Conventional conveyor for larger pieces
- Direct to hub metal sorting/refining

**Machinery and equipment** (engines, generators, pumps, winches):
- Flagged by CLASP during pre-cut survey (these are identifiable from the vessel model)
- Lifted by dedicated crane to **staging area** at drydock perimeter
- Assessed for refurbishment value vs. scrap
- Transported to hub by flatbed (too large for any automated conveyance)

### Phase 2: Basin Reset

- Absorbent granulate containers sealed and removed
- Retractable bulkheads repositioned for next slice based on CLASP's updated model
- Basin inspected for residual contamination (automated conductivity sweep)
- First-flush protocol: initial drainage from the next scoring pass is diverted to holding tank until sensors confirm the flow has cleared
- Next slice cycle begins

---

## The Physical Layout

```
                    ┌─────────────────────────────────────┐
                    │         HUB (Permanent)              │
                    │                                      │
                    │  ┌──────────┐  ┌──────────────────┐  │
                    │  │ Thermal  │  │  Fractionation    │  │
                    │  │ Destruct │  │  Lines            │  │
                    │  └────▲─────┘  └────▲─────────────┘  │
                    │       │             │                 │
                    │  ┌────▲─────┐  ┌────▲─────────────┐  │
                    │  │ Decontam │  │  Metal Sorting    │  │
                    │  │ Baths    │  │  & Refining       │  │
                    │  └────▲─────┘  └────▲─────────────┘  │
                    │       │             │                 │
                    │  ┌────▲─────────────▲─────────────┐  │
                    │  │    Storage / Staging             │  │
                    │  └────▲─────────────▲─────────────┘  │
                    └───────┼─────────────┼────────────────┘
                            │             │
              ══════════════╪═════════════╪══════════════
              PERIMETER     │  JURISDICTION│  TRANSFER
              ══════════════╪═════════════╪══════════════
                            │             │
        ┌───────────────────┼─────────────┼──────────────┐
        │   DRYDOCK (Spoke)  │             │              │
        │                    │             │              │
        │   ┌────────────────┴─────────────┴───────────┐ │
        │   │         INTERCEPT / EXIT GATES            │ │
        │   │  XRF sensors ─── classification ─── route │ │
        │   └────────────────▲─────────────────────────┘ │
        │                    │                            │
        │   ╔════════════════╧═══════════════════════╗   │
        │   ║     FULL-WIDTH CATCH BASIN              ║   │
        │   ║  retractable bulkheads │ granulate       ║   │
        │   ║  dispensers │ first-flush divert         ║   │
        │   ╚════════════════╤═══════════════════════╝   │
        │                    │                            │
        │   ┌────────────────┴───────────────────────┐   │
        │   │      ACTIVE CUT ZONE                    │   │
        │   │  scoring pass → full cut → crane lift    │   │
        │   │  vacuum hoods │ gantry │ reactive coat   │   │
        │   └────────────────┬───────────────────────┘   │
        │                    │                            │
        │              ══════╧══════                      │
        │              VESSEL (slicing                    │
        │              top → down)                        │
        │                                                 │
        └─────────────────────────────────────────────────┘
```

### Conveyance Runs (Drydock → Hub)

Six dedicated parallel runs, no shared infrastructure:

1. **Clean steel by alloy** → metal sorting/refining (conveyor)
2. **Contaminated steel** → decontamination baths (conveyor, separate)
3. **Granulated liquid hazmat** → thermal destruction / fractionation (sealed containers, flatbed or conveyor)
4. **Solid hazmat** → thermal destruction (pneumatic tube for particulate, conveyor for bulk)
5. **Non-ferrous metals** → metal sorting/refining (pneumatic + conveyor hybrid)
6. **Machinery/equipment** → staging/assessment (flatbed, as-needed)

---

## Scheduling: Stream-Selective Coupling

From the morph analysis, the optimal scheduling model is **stream-selective**:

- **Hazmat streams (liquid + solid): tightly coupled** to hub processing capacity. CLASP does not authorize a slice that will produce hazmat unless thermal destruction and fractionation confirm available capacity. This prevents hazmat accumulation at the drydock.
- **Steel streams: fully decoupled.** Buffer yard at drydock perimeter absorbs timing mismatch. Hub metal sorting processes steel on its own schedule. Steel is not time-sensitive and not a contamination risk in buffer.
- **Non-ferrous and machinery: decoupled.** Queue freely.

This gives the facility the throughput resilience of full decoupling for the high-volume, low-risk streams while maintaining contamination discipline on the streams that matter.

---

## Degraded Mode (Passive Fallback)

If automated sensors, pneumatics, or predictive scheduling fail, the facility falls back to **Combination 5 from the morph** — the passive configuration:

- Gravity-fed cascade (floor slope routes everything to collection gallery)
- Worst-case contamination protocol (all material from known hazmat zones treated as contaminated)
- Fixed sump tanks for liquid hazmat
- Stream-selective scheduling (hazmat tight, steel decoupled)
- Manual inspection at perimeter

The facility runs slower but never fails catastrophically. No automated system failure produces a contamination release. This is the defined safe state.

---

## Open Questions

1. **Absorbent granulate chemistry:** What granulate handles the full spectrum of marine hazmat (fuel oil, hydraulic fluid, bilge water with dissolved heavy metals)? What's the conversion time? What's the cost per tonne of liquid converted? Is the resulting solid classified as the same hazmat category or a different one?

2. **Catch basin sizing:** For a Panamax-beam (32.3m) slice, what's the maximum single-event liquid volume from a breached fuel tank? The basin + granulate must handle worst-case without overflow.

3. **Pneumatic tube capacity:** Can pneumatic systems handle the particulate loading from asbestos and PCB-containing solids at the volumes a single slice produces? What filtration is needed at the pneumatic terminus?

4. **First-flush diversion calibration:** What conductivity/pH thresholds distinguish "residual contamination from previous slice" from "new clean drainage"? How quickly do sensors stabilize?

5. **Granulate disposal classification:** If absorbent granulate containing fuel oil is classified as hazardous waste under RCRA, does it route to thermal destruction or to a different disposal pathway? This affects the hub's permitting.
