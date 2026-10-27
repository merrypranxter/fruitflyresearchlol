# Research index — 2026-10-27

Three uploaded reports form the initial research collection. **Their claims are not uniformly verified.** The notes below describe *what the reports say*, not independent confirmation of every citation, project, benchmark, numerical claim, or demonstration.

| ID | Uploaded PDF | Pages | Main contribution | Limitations |
| --- | --- | ---: | --- | --- |
| R01 | Connectome Artificial Life Exploration.pdf | 26 | Broad speculative design atlas: 100 concepts, neural octopus, pixel/glitter metabolism, mathematics as a body, research roadmap | A large invention list mixes feasibility with science claims; many examples are proposals, not established implementations. |
| R02 | The Unlimited Body_ Everything a Simulated Fly Brain Could Possibly Control.pdf | 30 | Detailed scientific distinction between connectome and neural controller; Digital Sphinx warning; CHROMAVORE specification; aesthetics, experiments and baselines | Its source list mixes peer-reviewed work and community demonstrations. |
| R03 | The Unlimited Body.pdf | 48 | More conservative source audit; evidence levels; named inputs/outputs; memory/performance guidance; three implementation blueprints; another proposed invention atlas | **Truncated around atlas entry 72.** Reports that it could not inspect the implementation repository; relies on supplied project details. |

Browse full extracted text:
- [R01](../research/raw-text/R01-connectome-artificial-life-exploration.txt)
- [R02](../research/raw-text/R02-everything-a-simulated-fly-brain-could-control.txt)
- [R03](../research/raw-text/R03-the-unlimited-body-perplexity.txt)

Original PDFs: see [source manifest](../research/manifest.json) and [PDF status](../research/pdfs/README.md). Extracted text may scramble equations and tables. Do not cite a malformed equation from the text transcription without checking the PDF.

## Recurring findings across the reports

1. **Anatomy ≠ executable behavior.** FlyWire/FAFB, MaleCNS, BANC and related datasets supply wiring/anatomy; LIF or other neuron dynamics, inputs, output translation, and embodiment must be provided.
2. **The body is interchangeable in an engineering sense.** A low-dimensional readout can select movements, transitions and goals; a soft-body/physics/local-controller layer handles thousands of degrees of freedom. That does not demonstrate natural octopus intelligence or fly intent.
3. **Closed loops matter.** Altered world state must alter subsequent sensory input; otherwise the system is an art visualizer with neural modulation, not an embodied agent.
4. **Learned preference needs a learning locus.** Separate sensory-encoder learning, motor-decoder learning, external-memory policy and synaptic plasticity; changing weights or making different pictures does not prove learned taste.
5. **Causality requires controls.** Intact circuit, scrambled or degree-preserving rewires, fixed replay, removed sensory feedback, matched conventional network and decoder-only baselines each test different things.
6. **Autonomy needs engineered physiology.** Hunger, stored pigment, damage, satiety, curiosity, exploration, or reproduction must be explicitly modeled rather than attributed to the real fly without evidence.
7. **Computational scope is a real constraint.** R03 recommends retaining the small established circuit for browser-first development, profiling neural time separately from display frame rate, and adding larger models only after measured benefits.
8. **Emergent art can be genuine within an engineered world.** Explicit chemistry/material rules + neural actions + persistent consequences make unplanned but reproducible visual outcomes possible.

## Named research / tooling leads in the reports

These are *reported leads*, not endorsements: FlyWire/FAFB; MaleCNS; BANC; MANC; FlyWire Codex; neuPrint; Shiu et al. brain simulation; flyvis; NeuroMechFly / FlyGym; Eon embodied fly; FlyGM; Digital Sphinx; DOOMFLY; Fly64; FlyPong; curated Awesome Fly repositories. For publications and URLs, consult the source report footnotes/bibliographies before reusing them.

## Overlap and differences

- R01 is the broadest in imaginative scope and more optimistic on WebGPU/full-connectome mobile scaling.
- R02 emphasizes why realistic-looking behavior may be driven by an expressive artificial decoder, plus carefully testable functional preferences.
- R03 is the most cautious on performance, auditability, and limitations of the current 6,203-neuron escape-related model.
- They contain **multiple distinct “100 ideas” catalogs**. Do not merge them as though there were a single authoritative numbered atlas. R03's list is incomplete in the uploaded PDF.
- Source numerical totals may refer to neurons, anatomical synaptic contacts, or unique neuron-pair edges; never interchange units.

See [scientific boundaries](SCIENTIFIC-BOUNDARIES.md), [experiment catalog](EXPERIMENTS.md) and [open questions](OPEN-QUESTIONS.md).
