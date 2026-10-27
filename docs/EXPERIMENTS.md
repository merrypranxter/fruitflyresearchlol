# Experiment catalog — proposed, not implemented

This is a prioritized *research-to-build menu* distilled from R01/R02/R03/R04. Each entry describes a test, not a claim that the fly brain has mastered it. All experiments require an inspectable mapping from sensory data through neural activity to output actions.

| ID | Experiment | Neural → actuator idea | World/body | Smallest honest success criterion | Scope |
| --- | --- | --- | --- | --- | --- |
| E01 | Bilateral Pigment Navigator | left/right looming/readouts → biased local motion/deposition | 2D pigment field | Side-swapping cue predictably swaps action; controls differ | first |
| E02 | Pixel / Pigment Ruminant | neural ingestion gate → transfer sampled material to store | colored material grid | world mass + stored mass accounted; feedback changes later movement | first |
| E03 | Glitter Kidney | neural release timing → resource-limited particle/crystal formation | material inventory + particles | glitter cost, shape, and timing traceable to model | first |
| E04 | Escape → Fractal Emesis | identified escape-like event → bounded grammar parameters | L-system / DLA / Voronoi | same neural state + seed reproduces specific eruption | first |
| E05 | Eightfold Borrowed Body | bilateral outputs → grouped arm recoil/bending | planar eight-arm creature with local reflexes | arm patterns change with cue and not with neural replay replacement | next |
| E06 | Mathematical God Garden | neural output → local seeding, inhibition, forcing | coupled pigment, contour, crystal and wave fields | created states change later neural inputs; stable over long runs | next |
| E07 | Fordite Liver | deposition output → nested persistent pigment layers | deformable interface / phase separation | observable history retained as contour strata | next |
| E08 | Curvature Grazer | computed curvature encoded synthetically → steering | moving contour / ribbon world | distinguish concave/convex cues with matched contrast | research |
| E09 | Twin Biography | clone same initial state; diverging experiences | matched paired worlds | persistent divergence tied to history, not hidden seed differences | next |
| E10 | Taste & Preference Orchard | explicit reward + learned readout; optional separate MB study | repeated choice scenes | acquisition, retention, reversal, generalization and controls | research |
| E11 | Swarm-Bodied Fly | several neural outputs → swarm cohesion/field goals | boids / particles | state affects swarm macrodynamics; local rules logged | next |
| E12 | Split-Brain Octopus | two independent circuits drive opposing arm groups | shared soft body | interaction/coordination beyond single-controller matched budget | research |
| E13 | Two-Agent Pigment Ecology | two agents modify same persistent material | crystals, pigment, decay and scarcity | consequences of A affect sensory/action of B and vice versa | research |
| E14 | Optical / Cymatic Body | neural modulation → wave sources, diffraction or refractive fields | resonant/light instrument | later sensed wave/light state shifts subsequent actions | exploratory |
| E15 | Body Swap Clinic | one fixed neural core, multiple body decoders | ribbon, blob, particle, arms | explicit comparison of generalization and adaptation costs | research |

### Baselines for first experiments

Every scene should support: **intact**, **silenced**, **timing-shuffled/replayed**, **feedback disconnected**, and **simple scripted/random controller**. Save each condition from the same seed/checkpoint.

### CHROMAVORE end-state (R02)

A pigment-eating organism with: artificial metabolism and storage; neural-selected feeding/growth/secretion; emergent structured glitter; procedural geometry release; eight or variable numbers of independently locally controlled tentacles; synthetic color/curvature senses; optional externally defined reward and verified learned preferences; biologically derived features visible in action telemetry.

Separate its *brain*, *body*, *world*, *physiology*, *learning*, *rendering* and *evaluation*. A beautiful picture alone is not a behavioral success metric.

### Other brainstorm categories in original reports

- Alien senses: time, topology, knotting, fractal complexity, magnetic fields, novelty, neural self-view, other agents.
- Impossible bodies: peristaltic line, hypercube crawler, elastic ribbons, distributed skin patches, boundary-only creature, particle disassembly/regeneration.
- Worlds: quasicrystal fields, graph grammars, artificial chemistry, Cahn–Hilliard, Allen–Cahn, Gray–Scott, cellular automata, morphogenesis, elastic networks.
- Ecologies: symbiotic/competitive painters, spore banks, hoarding reefs, parasites that change perception, distributed colonies.
- Sound: resonance, FM/granular synthesis, audible territory, cymatic structures, spectrally feeding creatures.
- Evolution: morphology adapting *around* a frozen neural controller; independent evolutionary search on decoder/body; separate research tracking for synaptic modifications.

For all 100-item lists and specific novelty claims, inspect the unabridged source text, especially [R01](../research/raw-text/R01-connectome-artificial-life-exploration.txt) and [R03](../research/raw-text/R03-the-unlimited-body-perplexity.txt). R03's atlas is incomplete in the uploaded document.


## Five concrete R04 protocols — useful first research milestones

R04 goes beyond brainstorming by specifying experimental inputs, output channels, null controllers, measurements, failure cases and completion criteria. These protocols can be implemented **without immediately replacing the current described neural circuit**:

| Order | Source protocol | Related catalog entries | Main scientific claim to test |
| --- | --- | --- | --- |
| 1 | [P01 Bilateral Contour Grazer](../research/protocols/P01-bilateral-contour-grazer.md) | E01 / E08 | The neural circuit carries nontrivial left/right information, not merely a hard-coded turning bias |
| 2 | [P02 Conserved Glitter Metabolism](../research/protocols/P02-conserved-glitter-metabolism.md) | E02 / E03 | The agent sustains a measurable material cycle with neural-influenced action gating |
| 3 | [P03 Eight-Arm Stirrer](../research/protocols/P03-eight-arm-stirrer.md) | E05 | Neural modulation adds coordination beyond a local mechanical/reflex controller |
| 4 | [P04 Pigment Notebook](../research/protocols/P04-pigment-notebook.md) | New research protocol | Constructed environmental marks/routes provide real future information after transient memory reset |
| 5 | [P05 Twin Taste Histories](../research/protocols/P05-twin-taste-histories.md) | E09 / E10 | Different developmental histories produce retained, transferable, tested behavioral differences |

These protocols are **R04 proposals**, not implemented features or proven outcomes.

## R04's completed atlas and extra directions

Consult [R04 continuation guide](R04-CONTINUATION.md) for source-matched proposals #72–#100 and 20 additionally numbered experimental directions. **R03 and R04 constitute one continuous invention atlas**, while R01 contains another independently numbered set.
