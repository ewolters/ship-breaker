# Pre-Mortem: Automated Ship Salvage via CLASP Drone Coordination

**Date:** 2026-05-02
**Technique:** Prospective Hindsight
**Perspectives:** Impact Investor (Series A lead), Chittagong Yard Owner (22-year incumbent), CLASP Chief Engineer (ex-military robotics)

---

## Failure Narratives

### The Impact Investor

*May 2027*

I remember the pitch deck slide that sold me. A cross-section of the drydock, the impermeable substrate glowing blue, everything else flowing from that single elegant constraint. "The boundary IS the intervention," Marcus said, and I believed him. I still think that principle was right. That's what makes this so hard to write.

We closed the Series A in February 2024 at a $34M valuation. I led the round. I called in two co-investors I'd worked with for a decade and told them this was the cleanest environmental infrastructure thesis I'd seen in fifteen years. They trusted me. That trust is gone now.

The first warning sign came in month seven, during the Bangladesh pilot authorization process. CLASP's adaptive guild-succession logic — the crown jewel of the architecture, the thing that was supposed to handle the fact that no decommissioned vessel matches its blueprints — required the onsite AI to make autonomous decisions about vertical segment sequencing based on real-time structural readings. The port authority wanted a printed sequence approval before any crane moved. The team said that defeated the entire design. The port authority said that was the regulation. The team asked for a waiver. That negotiation took eleven months.

We saw it then. I saw it. I told Marcus in a call that regulators don't grant waivers to systems they don't understand, and they don't understand systems where the machine decides the sequence. He said we'd demonstrate safety through the recon drone data, that the data would speak for itself. I let him talk me back into confidence. That was my failure.

The root cause was not the technology. The technology, largely, worked. The root cause was a foundational category error baked into the design thesis: the team built CLASP as an autonomous orchestrator for an industry where every lift, every cut, every crane movement exists inside a human approval chain going back to the ILO Conventions and the Hong Kong Convention. CLASP's core design principle — "orchestrates but never executes" — sounds clean in a slide deck. In practice, it meant the system produced instructions that no licensed marine engineer would sign off on, because the instructions came from an inference engine responding to sensor data, not from a certified structural assessment. You cannot interrupt a regulatory transmission chain the same way you interrupt a contamination transmission chain. The team conflated the two.

By month eighteen, we had spent $19M, completed zero full ship dissolutions, and had two partial pilots in Indonesia that were suspended pending review after a crane sequencing decision — correct, as it turned out, structurally sound — was made without a human co-signature. The incident wasn't a failure of the system. It was a failure of legitimacy. Same outcome.

The human cost is where I lose sleep. Dr. Aisha Okonkwo, the lead environmental engineer, spent four years building the subterranean hazmat evacuation system. It was genuinely beautiful work, published, peer-reviewed, cited. Her name is now attached to a cautionary tale rather than a breakthrough. She left the sector. Marcus and his co-founder haven't spoken since the bridge round collapsed in early 2026. The two co-investors I brought in have not returned my calls in six months. Not anger, exactly. Just the particular silence of people who trusted your judgment and won't again.

If I could go back, I would have funded a regulatory pathfinder before the technology build, not alongside it. Not a lobbyist. An actual regulatory co-designer — someone whose job was to make the approval chain legible to regulators before the first crane moved. The technology was solving the right problem. It was solving it in a language that the institutions gatekeeping ship demolition were structurally prohibited from accepting.

The boundary was the intervention. That was true. But there are two kinds of boundaries in this industry — physical containment and institutional legitimacy — and we only designed for one of them.

That's the story. That's where the money went.

---

### The Chittagong Yard Owner

*Spoken at the Chittagong Shipbreakers' Association dinner, November 2027*

They came in 2023 with laptops and confidence. A Dutch consortium, some American NGO money behind them, a Singaporean logistics firm as the respectable face. They called it CLASP. I called it a fantasy, but quietly, because my nephew works in government and I did not want trouble.

The pitch was elegant. A drydock with an impermeable floor. One ship at a time, fully sealed. Drones doing the reconnaissance, cranes doing the cutting, everything orchestrated by software that would know where every pocket of fuel oil was before a torch came near it. They showed us renderings. The drydock gleamed. There was no mud. There were no men.

The first warning sign appeared in late 2024, before a single hull was touched. CLASP's recon drones were mapping a retired Panamax bulk carrier to build their internal model of the ship. The ship had spent 31 years at sea and then four years laid up in Batam. The drones returned data. The data matched almost nothing in the original build documentation. Seventeen structural modifications, undocumented. Two entirely remade engine room bulkheads. Fuel tanks where cargo holds were supposed to be. The CLASP system, which was designed to orchestrate sequences — not improvise them — had no answer for this. The project managers wrote it up as a calibration issue. They adjusted parameters. They filed it and moved forward.

I heard this from a Bangladeshi engineer who had been hired as a local liaison. He told me over tea. He said the project engineers were not lying — they genuinely believed they had corrected for it. But they had written the system to execute a known sequence adaptively, not to reason from scratch when the sequence itself was wrong. There is a difference. A very important difference. A foreman knows this. Software, it turns out, did not.

The drydock itself was the second failure, slower and more expensive. Subterranean hazmat evacuation requires a substrate that does not shift. Chittagong's beachfront is not that substrate. The impermeable membrane they installed in the pilot site at Bhatiary developed stress fractures within eight months of installation, before the first ship entered. They repaired it. It fractured again. The entire design principle — containment first, everything else plugs in — was sound in theory, but the theory assumed geology that does not exist here. They had tested the membrane in the Netherlands. In clay. Not in tidal sand.

By mid-2025, the consortium was spending twice the projected budget and had not yet processed a single ship. The NGO backers began asking questions. The Singaporeans began making calls. The Dutch engineers began fighting among themselves about whether the adaptive guild-succession logic in CLASP — the part meant to handle exactly the problem of ships not matching their blueprints — could be rebuilt in time to save the project. It could not. Not because the idea was wrong, but because it had been specified as a feature to be added after launch rather than the foundational capability the whole system required. They had built the house and then remembered they needed a foundation.

The human cost is the part that does not appear in the NGO reports. The Bangladeshi engineer who warned them in 2024 was passed over for a permanent position with the consortium. He is back in Dhaka now. Three young Dutch engineers who had staked their early careers on this project have scattered — one into consulting, one into academia, one I have not heard of since. The Singaporean firm's local director, a man named Adrian Toh who had believed in this genuinely and said so publicly, lost a significant client relationship because he had vouched for the project. These people are not in the final report. They never are.

What would I have done differently? I would have spent six months in this yard first. Not studying. Working. I would have watched what happens when a ship that was built in 1987 to one specification arrives in 2024 having become something entirely else. I would have understood that the gap between blueprint and reality is not an edge case to be calibrated away. It is the central condition of this work.

The sea changes everything it touches. We have always known this. They did not.

---

### The CLASP Chief Engineer

*Recorded May 2027, eighteen months after the Gothenburg incident*

I will tell you exactly what happened, because I watched it happen and did not stop it.

We broke ground on the Gothenburg facility in early 2024 with genuine conviction. The design was sound — I still believe that. The closed mesocosm boundary as the primary intervention, CLASP as pure coordinator never touching steel, the guild-succession logic that let the system respond to what ships actually were rather than what their paperwork said. On paper, and in simulation, it was elegant.

The first warning sign came eight months in, during integration testing with the crane subsystem. CLASP was issuing segment-lift commands based on recon drone telemetry, and the cranes were acknowledging receipt — but the acknowledgment protocol was a simple handshake. It confirmed message delivery, not physical readiness. The cranes were saying "heard you" when they should have been saying "ready to act." Our firmware lead, Marta Henriksen, flagged this in writing on September 14th, 2024. I read the flag. I categorized it as a latency issue, not an architecture issue, because we were behind schedule and I wanted it to be a latency issue. That was the decision that broke everything.

The second warning came from the hazmat team. The subterranean evacuation channels were designed around flow models built from tanker blueprints — clean, idealized internal volumes. But the first full-scale test ship, a decommissioned Panamax bulk carrier, had three decades of informal modifications: welded bulkheads, sealed compartments no blueprint reflected. The contamination modeling was off by a significant margin. The evacuation timing was wrong. We recalibrated and told ourselves it was a one-ship anomaly.

It was not an anomaly. It was the system telling us that guild-succession logic requires ground truth about internal state that recon drones, in 2024 hardware, simply could not reliably provide. We had designed for adaptive response to unknown ship state, but we had not fully reckoned with how unknown "unknown" could be. The recon data had gaps we were filling with confidence intervals that were, in retrospect, optimistic by a factor that embarrasses me.

The Gothenburg incident — I won't call it an accident, because accidents imply bad luck — happened on November 3rd, 2025. CLASP issued a segment-lift sequence on a section of hull that the recon drones had assessed as clear. The assessment was based on sensor readings that, we later determined, had been partially occluded by a corroded internal structure that scattered the LIDAR return in a pattern our classification model had never encountered in training. The crane executed. The section was not clear. The resulting failure cascaded into the hazmat containment layer because the timing assumption in the evacuation sequence was built on the earlier, miscalibrated flow model we thought we had fixed.

No one died. I want to be precise about that, because in the months afterward people implied otherwise. But three workers were hospitalized. The facility was condemned. And the regulatory consequence was total: the entire class of semi-automated maritime deconstruction systems was placed under a moratorium that is still in effect as I write this.

The human cost is harder to quantify. Marta Henriksen's career in industrial robotics is functionally over — her name is on the firmware that sent the faulty acknowledgment, even though she flagged the flaw before we shipped. That is not justice. My co-founder Pietersen has not spoken to me since March 2026. The consortium of port authorities who backed us lost not just capital but institutional credibility for backing an unproven system over their own engineers' objections.

What I would do differently: I would have treated the handshake protocol failure as an architecture review trigger, not a patch ticket. I would have required physical-readiness confirmation — a state assertion, not a message receipt — before any lift sequence could execute. CLASP was designed on the principle that coordination never executes. But I forgot that coordination commands execution, and commands require verified preconditions, not assumed ones.

The system failed where all coordination systems fail: at the boundary between the model and the world. I built a very good model. The world was not consulted.

---

## Pattern Analysis

### Common Failure Themes (2+ narratives — high robustness)

**The blueprint-reality gap as a foundational condition, not an edge case.** All three narratives converge. The yard owner states it most cleanly, but the chief engineer's hazmat flow model built on tanker blueprints and the investor's crane sequence decision both trace to the same source: the system was designed against documentation, and the physical world had moved on. Independent convergence across financial, operational, and engineering perspectives makes this the most robust finding.

**Guild-succession logic was deferred, not designed.** Two narratives (yard owner, chief engineer) explicitly identify adaptive sequencing as a capability specified for post-launch rather than built as the foundation. The investor's crane-sequence legitimacy crisis is the institutional expression of the same gap. The system assumed it could be calibrated into a working state from a stable baseline — there was no stable baseline.

**Human warnings were dismissed and the humans paid the cost.** All three narratives name a specific person who flagged a specific problem early, was overruled, and had their career damaged or ended: the Bangladeshi engineer, the firmware lead, and the environmental engineer. The pattern of warning, dismissal, and subsequent vindication-by-disaster appears in every account.

### Unique Risks (blind spots only one perspective caught)

**Regulatory legitimacy as a distinct transmission chain** (investor only). No other narrative engages with the ILO/Hong Kong Convention approval chain or institutional legitimacy as a parallel system to physical containment. The other two treat the failure as technical. The investor is the only one who identified that "orchestrates but never executes" has a legal meaning, not just an operational one.

**Firmware confirmation semantics** (chief engineer only). Message delivery confirmed as physical readiness — this specific integration failure, traceable to a single protocol design decision, is invisible to both other narrators. It is the proximate cause of the November incident but absent from the financial and operational accounts.

**Geology and membrane failure** (yard owner only). The impermeable membrane failing in Chittagong's tidal sand is a site-specific civil engineering failure not mentioned elsewhere. The mesocosm boundary as physical containment was a design principle; its failure mode in non-Dutch soil conditions was not tested.

### Earliest Warning Signs (the canary)

The crane acknowledgment protocol flaw, flagged in writing before launch, is the earliest documented canary. It preceded the November incident by a substantial period and was reclassified as a latency issue under schedule pressure. The membrane stress fractures appeared within eight months of operation. The regulatory waiver negotiation began in month seven. All early warnings were present before any full dissolution was attempted.

### Root Cause Consensus / Divergence

**The narratives do not agree.** The investor assigns root cause to a category error about institutional legitimacy. The yard owner assigns it to premature launch without foundational adaptive capability. The chief engineer assigns it to a specific integration flaw and optimistic confidence intervals in sensor classification. This disagreement is itself a finding: each narrator's domain produced a different root cause, which means the failure was **over-determined**. Any single fix would have left the other two causes intact.

### Assumptions Challenged

- That "orchestrates but never executes" is a neutral architectural description rather than a claim about legal and institutional authority
- That adaptive logic can be retrofitted onto a working system rather than being the precondition for the system working at all
- That recon drone sensor fidelity in current hardware is sufficient to establish ground truth in a 30-year-old vessel with undocumented modifications
- That a containment system validated in one geology transfers to another
- That the gap between blueprint and actual ship state is quantifiable variance rather than a categorical unknown
