# Morphological Analysis: Inter-Plant Logistics

**Date:** 2026-05-02
**Technique:** Morphological Analysis (Zwicky Box)

---

## Morphological Box

| Dimension | A | B | C | D |
|-----------|---|---|---|---|
| **1. Intercept Geometry** | Drip-pan trays indexed with cutting head | Full-width catch basin + retractable bulkheads | Vacuum hoods on gantry (negative pressure) | Sacrificial absorbent mat, peeled after each slice |
| **2. Conveyance Topology** | Single trunk spine, timing-window separation | Fully dedicated parallel runs, no shared infra | Gravity-fed cascade, graded floor into gallery | Pneumatic tube + conveyor hybrid |
| **3. Stream ID Protocol** | Human inspector + handheld scanner | Automated sensor array (XRF, conductivity, optical) | Pre-classification by vessel model (route by location) | Worst-case contamination protocol (conservative collapse) |
| **4. Liquid Hazmat Buffering** | Fixed sump tanks (2x safety factor) | Flexible bladder reservoirs | Absorbent granulate (convert liquid to solid) | Real-time continuous pumping, small surge pocket |
| **5. Scheduling Coupling** | Fully decoupled (buffer queue) | Takt-locked (slice gated by hub readiness) | Stream-selective (hazmat tight, steel decoupled) | Predictive pre-scheduling from vessel model |
| **6. Hazmat Jurisdiction** | Transfer at perimeter fence | Transfer when container sealed/labeled | Single integrated team (no transfer) | Third-party inspection checkpoint |

**Total design space:** 4,096 combinations

---

## Random Combinations Evaluated

### Combination 1
Mat / Pneumatic hybrid / Automated sensors / Flexible bladders / Takt-locked / Sealed-container transfer

**Feasible:** No. Mat produces bulky solid waste incompatible with pneumatic conveyance. Mat's batch cycle (stop-peel-replace) fights takt-locking's continuous-flow discipline.

**Interesting:** Flexible bladders + takt-locking is worth isolating — bladders pre-sized to takt interval's expected yield volume could meter variable liquid generation into predictable release.

### Combination 2
Catch basin / Single trunk / Pre-classification / Continuous pumping / Decoupled / Third-party checkpoint

**Feasible:** Marginal. Pre-classification dangerous for liquid hazmat where surprises are the rule. Single trunk creates serialization bottleneck. Fix: upgrade to automated sensors for liquid hazmat only.

**Interesting:** Third-party checkpoint + fully decoupled creates a latent inventory build — who controls dwell time when the inspector isn't there?

### Combination 3
Catch basin / Pneumatic hybrid / Automated sensors / Absorbent granulate / Predictive pre-schedule / Sealed-container transfer

**Feasible:** Yes. No modification needed.

**Interesting:** The standout combination. Absorbent granulate converting liquid to solid is not merely a buffering choice — it is a **topology simplification**. Once liquids become solids, the entire facility is a solid-handling system with one managed conversion zone. Pneumatic hybrid becomes viable because granulate-filled containers are tractable. Predictive pre-scheduling gains leverage because granulate throughput is deterministic. This combination quietly eliminates the stochastic element of liquid hazmat by changing its physical state early, cascading favorably through every downstream dimension.

### Combination 4
Catch basin / Pneumatic hybrid / Automated sensors / Absorbent granulate / Decoupled / Perimeter fence transfer

**Feasible:** Yes. Variant of Combination 3 trading coordination overhead for operational simplicity.

**Interesting:** Perimeter fence transfer is regulatory-exposure-heavy but operationally faster. Cost/compliance tradeoff variant of Combination 3.

### Combination 5
Mat / Gravity cascade / Worst-case protocol / Fixed sumps / Stream-selective / Perimeter fence transfer

**Feasible:** Yes, with caveats (floor-slope audit needed).

**Interesting:** The most **passive** combination — no pneumatics, no bladders, no predictive logic. Everything runs on physical geometry and conservative classification. Lowest technology dependency, highest tolerance for sensor/software failure. Degrades gracefully, never fails catastrophically. Serious consideration as first-facility configuration or defined degraded-mode fallback.

### Combination 6
Mat / Dedicated parallel / Pre-classification / Fixed sumps / Predictive pre-schedule / Sealed-container transfer

**Feasible:** Yes.

**Interesting:** High-ceiling, high-variance. When vessel model is accurate, extremely smooth — schedule built before first cut. When manifest has errors (sealed compartments, undocumented retrofits), whole schedule must be replanned mid-slice.

### Combination 7
Mat / Single trunk / Pre-classification / Flexible bladders / Takt-locked / Sealed-container transfer

**Feasible:** No. Mat-plus-takt conflict again. Single trunk with takt-locking means any delay gates all six streams.

**Interesting:** Flexible bladders + takt-locking pairing worth isolating despite combination infeasibility.

### Combination 8
Mat / Dedicated parallel / Automated sensors / Fixed sumps / Decoupled / Perimeter fence transfer

**Feasible:** Yes.

**Interesting:** The **brute-force** solution. Dedicated parallel runs + full decoupling = most throughput-robust configuration. No stream can block another, no hub delay gates cutting head. Mat's batch character absorbed by buffer queue. High infrastructure cost, low operational complexity. Operational confidence base to build from.

---

## Most Promising

### 1. Combination 3 — The Phase-State Simplifier
Catch basin / Pneumatic hybrid / Automated sensors / Absorbent granulate / Predictive pre-schedule / Sealed-container transfer

Physical-state conversion of liquid to solid via absorbent granulate is a topology simplification. The entire facility becomes a solid-handling system with one conversion zone rather than a dual-phase system with separate liquid infrastructure. Predictive scheduling gains traction because granulate throughput is deterministic. Sealed-container transfer closes jurisdictional loop cleanly. Coherent from intercept through handoff.

### 2. Combination 8 — The Robust Baseline
Mat / Dedicated parallel / Automated sensors / Fixed sumps / Decoupled / Perimeter fence transfer

Most failure-tolerant configuration. No single stream failure propagates. Hub absorbs variability without stalling cutting head. Not elegant, but operationally confident. Strong candidate for first-facility proving ground.

### 3. Combination 5 — The Passive Fallback
Mat / Gravity cascade / Worst-case protocol / Fixed sumps / Stream-selective / Perimeter fence transfer

Entirely passive physics — gravity, conservative classification, fixed sumps. Runs on geometry rather than automation. Degrades gracefully under sensor/software failure. Candidate for primary configuration in developing-market spokes or as defined degraded-mode fallback for automated primary design.

---

## Unexpected Dimension Interactions

### Liquid Buffering Pre-Selects Conveyance
Absorbent granulate (4C) unlocks pneumatic hybrid conveyance (2D) by eliminating the liquid phase entirely. Flexible bladders (4B) are incompatible with pneumatic systems and require dedicated parallel or trunk infrastructure, which cascades into scheduling constraints. **The buffering choice is effectively a conveyance pre-selection.** Treating these as independent will produce conflicts.

### Mat Intercept Fights Takt Scheduling
Sacrificial mats (1D) impose a physical batch cycle: cut, peel, replace, resume. Takt-locking (5B) penalizes any unscheduled pause. The mat replacement cycle must be modeled into the takt interval or the facility runs chronically behind. Combinations 1 and 7 both carry this conflict. Scheduling and intercept geometry share the cutting head as a common resource.

### Stream ID and Hazmat Jurisdiction Are Liability-Coupled
Worst-case contamination protocol (3D) simplifies jurisdictional handoff — if everything is treated as hazmat, transfer is paperwork not real-time classification. Pre-classification (3C) + perimeter fence transfer (6A) creates classification dispute risk at the boundary. **Protocol and jurisdiction must be co-designed, not selected independently.**
