# Indicator Chemistry v2: Hard Ecological Safety Constraint

**Date:** 2026-05-02
**Status:** Replaces v1. Hard-constrained for human and ecological safety.
**Supersedes:** `reactive-coating-chemistry.md` (v1 had reagents that, while analytically established, are not acceptable for open-air spray application in a facility designed to prevent ecological harm)

---

## The Hard Constraint

**Everything sprayed must be something you would not mind breathing.**

This is not a softened version of v1. It is a different design philosophy. We are building a facility whose entire value proposition is preventing ecological and human harm. Spraying analytically useful but ecologically questionable chemicals inside that facility is a contradiction that undermines the concept at a foundational level.

**Acceptable:** FDA GRAS (Generally Recognized As Safe), food-grade, cosmetic-grade, medical-diagnostic-grade. Things that are put in food, in eyes, on skin, or inhaled during medical procedures.

**Not acceptable:** Laboratory-grade analytical reagents that are "low toxicity at working concentrations." If the safety data sheet says "avoid inhalation," it doesn't get sprayed from a drone inside an enclosed drydock.

---

## Design Shift: Camera Physics First, Safe Dyes to Enhance

v1 tried to make every contaminant detectable by a sprayed chemical. v2 inverts this: **use camera physics (UV, multispectral, thermal) as the primary detection method — no chemicals needed — and use food-safe dyes only where passive imaging is insufficient.**

This is actually a better design. Most of what we need to detect is already visible to the right camera at the right wavelength.

---

## Layer 0: Passive Multispectral Imaging (No Spray)

Before any dye is applied, fly the recon drone with a multispectral camera array. This alone detects two of the four contaminant classes with no chemicals whatsoever.

### Hydrocarbons — UV Autofluorescence
**Method:** Illuminate with 365nm UV, image with standard camera.
**Signal:** Petroleum hydrocarbons (fuel oil, lubricants, hydraulic fluid) autofluoresce blue-white to yellow-green under UV. This is a well-established technique used in environmental spill assessment, pipeline inspection, and forensic investigation.
**Chemicals required:** None. Zero. The oil itself is the indicator.
**Effectiveness:** High. Oil films on steel are strongly fluorescent against the non-fluorescent steel background.

### Thermal Anomalies — Infrared Imaging
**Method:** FLIR or radiometric thermal camera on recon drone.
**Signal:** Liquid-filled compartments, trapped gases, and areas with different thermal mass show as anomalies on the thermal image. A fuel tank retaining residual liquid reads differently from an empty void.
**Chemicals required:** None.
**Effectiveness:** Moderate. Does not identify *what* the material is, but identifies *where something is* that differs from empty steel. Flags zones for closer inspection.

---

## Layer 1: Hydrocarbon Enhancement — Fluorescein

For zones where UV autofluorescence is ambiguous (thin films, mixed surfaces), enhance with fluorescein.

**Chemical:** Fluorescein sodium (C.I. 45350), 0.01-0.1% aqueous solution
**Safety profile:**
- FDA-approved food colorant (FD&C Yellow No. 8 / D&C Yellow No. 7)
- Used in ophthalmology — literally applied directly into human eyes for corneal examination
- Used in municipal water tracing — deliberately released into drinking water systems
- GRAS. You can drink it. It is put in the Chicago River every St. Patrick's Day.

**Mechanism:** Fluorescein partitions into hydrocarbon films and dramatically amplifies fluorescence under 490nm blue excitation light. Clean steel shows no signal; oil-contaminated zones glow vivid green.
**Visual signal:** Brilliant green fluorescence under blue light (490nm excitation / 520nm emission).
**Reaction time:** Essentially instant — partition is physical, not chemical.
**Cost:** Fluorescein is extremely cheap. ~$0.50-2.00 per slice at working dilutions.

---

## Layer 2: Heavy Metals — Turmeric/Curcumin

**Chemical:** Curcumin (from turmeric), 0.1-0.5% in food-grade ethanol or aqueous suspension
**Safety profile:**
- Food ingredient consumed daily by hundreds of millions of people
- GRAS. FDA approved as food colorant, dietary supplement, and cosmetic ingredient.
- You eat it. In curry. Regularly.

**Mechanism:** Curcumin is a well-documented chelator that forms colored complexes with lead and boron. In the presence of lead-containing paint, curcumin shifts from yellow to red-brown. The "Rosocyanine reaction" (curcumin + boron) is a classic analytical chemistry test adapted here for surface application. Lead detection via curcumin color shift has been published in food safety and environmental monitoring literature.
**Visual signal:** Yellow (clean surface) → red-brown (lead present). Visible light imaging. The color shift is dramatic and camera-resolvable.
**Reaction time:** 5-10 minutes for full color development on dried surfaces.
**Limitations:**
- Specific to lead and boron. Does not detect cadmium or chromium directly.
- Lead is the primary heavy metal of concern in marine paint (red lead, white lead primers were standard in shipbuilding). Cadmium and chromium are secondary.
- For cadmium/chromium: flag zones where curcumin shows lead, and treat the entire paint system as heavy-metal-contaminated. Conservative but safe.

**Cost:** Turmeric extract is inexpensive. ~$2-5 per slice.

---

## Layer 3: Asbestos Fiber — Food-Dye Differential Uptake

**Chemical:** Food-grade methylene blue (C.I. 52015), 0.05% aqueous
**Safety profile:**
- FDA-approved pharmaceutical (used IV and orally for methemoglobinemia treatment)
- Used in medical procedures — injected into patients and swallowed for diagnostic purposes
- USP grade available. Medical professionals administer this to humans routinely.

**Mechanism:** Methylene blue is a cationic dye that is preferentially adsorbed by mineral fiber surfaces (chrysotile, amphibole) versus organic paint matrices. Mineral fibers have high surface charge density and surface area, causing disproportionate dye uptake. After brief rinse (water spray from same drone), fiber-containing zones retain blue stain while organic surfaces wash clean.
**Visual signal:** Persistent blue stain on fiber-containing zones against neutral background. Visible light imaging.
**Reaction time:** 3-5 minute dwell, then water rinse pass.
**Limitations:**
- Detects exposed mineral fiber surfaces only. Does not detect encapsulated asbestos beneath intact paint.
- This is acceptable: laminar slicing exposes fresh surfaces with each cut. Encapsulated asbestos in the remaining hull will be detected when its layer is reached.

**Cost:** Medical-grade methylene blue is inexpensive. ~$3-8 per slice.

---

## Layer 4: PCBs / Chlorinated Organics — The Honest Gap

**There is no food-safe spray indicator for PCBs.**

This is the one contaminant class where v1's analytical chemistry (NBP) was genuinely useful, and where the safety constraint creates a real gap. PCB detection requires either solvent extraction or instrumental analysis — neither is achievable with a food-safe spray.

### Mitigation Options (not spray-based):

**Option A: Conservative zone protocol.** PCB-containing materials in ships are concentrated in specific locations: caulk/sealant joints, electrical insulation, capacitor housings, and some paint systems (primarily pre-1979 vessels). For vessels built before 1979, treat ALL caulk joints, electrical insulation, and capacitor locations as PCB-positive. This is the "worst-case contamination protocol" from the logistics morph — conservative but zero false negatives.

**Option B: Handheld XRF on flagged zones.** After the spray protocol identifies heavy-metal and hydrocarbon zones, dispatch a ground drone with a mounted handheld XRF analyzer to zones where chlorine signature would indicate PCB presence. XRF detects elemental chlorine in the PCB matrix. This is the "calibration drone pair" concept from the TRIZ analysis — different sensor physics for the contaminant that spray chemistry can't reach.

**Option C: Pre-cut wipe sampling.** Before each slice, a ground drone takes wipe samples from accessible surfaces at the cut line. Samples analyzed by immunoassay test kit (PCB RaPID Assay or equivalent) — 15-minute turnaround, no spray needed. This is the score-before-cut protocol applied to PCB detection specifically.

**Recommended:** Option A as default (conservative zone protocol for all pre-1979 vessels), with Option B (XRF drone) for ambiguous zones on post-1979 vessels.

---

## Revised Application Protocol

```
T+0:00  Expose new horizontal plane (slice lifted clear)

        ─── PASSIVE IMAGING (no spray) ───
T+0:02  UV autofluorescence pass (365nm) → preliminary hydrocarbon map
T+0:05  Thermal imaging pass (FLIR) → anomaly/liquid detection map
T+0:08  Visible-light high-res photo → baseline documentation

        ─── SAFE DYE ENHANCEMENT ───
T+0:10  Layer 1: Fluorescein spray (hydrocarbon enhancement) — instant
T+0:12  Image under 490nm blue light → confirmed hydrocarbon map
T+0:15  Layer 2: Curcumin spray (heavy metals) — 5-10 min dwell
T+0:25  Image visible light → lead detection map (yellow→red-brown)
T+0:28  Layer 3: Methylene blue spray (asbestos fiber) — 3-5 min dwell
T+0:33  Water rinse spray (same drone, clean tank)
T+0:35  Image visible light → fiber retention map (blue zones)

        ─── INSTRUMENTAL (flagged zones only) ───
T+0:38  XRF drone dispatched to PCB-suspect zones (if post-1979 vessel)
T+0:45  PCB zone confirmation

T+0:50  Composite hazmat map generated by CLASP
T+0:55  Score-before-cut protocol begins on flagged zones
```

**Total characterization time: ~55 minutes** (same as v1, but now safe enough to breathe).

---

## Revised Cost Estimate per Slice

| Item | Cost | Safety |
|------|------|--------|
| Fluorescein 0.01% (~10L) | ~$0.50-2.00 | FDA food/ophthalmic |
| Curcumin 0.1% (~15L) | ~$2-5 | GRAS food ingredient |
| Methylene blue 0.05% (~15L) | ~$3-8 | FDA pharmaceutical |
| Water rinse (~20L) | ~$0.10 | Water |
| **Total reagent cost per slice** | **~$6-15** | **All food/medical grade** |
| **Cost per ship (~30-50 slices)** | **~$200-750** | |

**v2 is 6x cheaper than v1** ($200-750 vs $1,500-4,000) because food-grade dyes are commodity chemicals, not analytical-grade reagents.

---

## Reagent Summary Table (v2)

| Target | Reagent | Safety Grade | Signal | Method | Spray? |
|--------|---------|-------------|--------|--------|--------|
| Hydrocarbons (prelim) | None | N/A | UV autofluorescence | 365nm UV camera | No |
| Hydrocarbons (confirmed) | Fluorescein sodium | FDA food/ophthalmic | Green fluorescence | 490nm excitation | Yes |
| Thermal anomalies | None | N/A | Temp differential | FLIR camera | No |
| Lead (primary heavy metal) | Curcumin (turmeric) | GRAS food ingredient | Yellow → red-brown | Visible camera | Yes |
| Asbestos fiber | Methylene blue | FDA pharmaceutical | Blue stain retention | Visible camera | Yes |
| PCBs | N/A (no safe spray) | N/A | Chlorine signature | XRF instrument | No (drone-mounted XRF) |

---

## What Changed from v1

| Dimension | v1 | v2 |
|-----------|----|----|
| Philosophy | Analytical chemistry adapted to spray | Camera physics first, food-safe enhancement |
| Asbestos indicator | Malachite Green (lab dye) | Methylene blue (FDA pharmaceutical) |
| PCB indicator | NBP (analytical reagent) | No spray — XRF drone or conservative zone protocol |
| Heavy metal indicator | Sodium rhodizonate + DPC | Curcumin (turmeric) |
| Hydrocarbon indicator | Sudan IV (histological dye) | Fluorescein (FDA food/ophthalmic) + UV autofluorescence |
| Safety standard | "Low toxicity at working concentration" | "Would not mind breathing it" |
| Cost per ship | $1,500-4,000 | $200-750 |
| PCB detection | Spray-based (NBP) | Instrumental (XRF) or conservative zone protocol |

The v2 protocol is **safer, cheaper, and more honest** about the PCB gap. The gap is real — but the mitigation (conservative zone protocol + XRF) is operationally sound and doesn't compromise the ecology-first positioning.
