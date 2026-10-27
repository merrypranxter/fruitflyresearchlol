# Development roadmap for the artificial-life playground

**Research roadmap, not a statement of current repository implementation.** R03 describes a browser-based 6,203-neuron escape-related circuit, LIF model, left/right looming inputs and hybrid outputs from supplied context, not inspected source. Verify actual code in the implementation repository before touching it.

## Stage 0 — preserve and inventory
- Locate and inspect the real implementation repo; confirm branch, license, tested device, engine and build.
- Freeze an executable neural fixture and expected readout traces.
- Record graph/hash, neuron IDs, sign conventions, seed and known stimuli; write tests.
- Do not replace the model, regenerate the connectome, or throw away a working scene as “cleanup.”

## Stage 1 — expose causal wiring
- Label neural vs scripted vs random movement/output contributions.
- Show left/right stimulus, selected population activity, action selection and world feedback.
- Add replay/silence/disconnect toggles and synchronized capture.
- Test the “runs into a boundary and stays there” failure with closed-loop exploration, edge sensing and sensible recovery, *not* hidden choreography.
- Use [P01 Bilateral Contour Grazer](../research/protocols/P01-bilateral-contour-grazer.md) to check neural left/right information with frozen readout and matched controls before richer autonomous decisions.

## Stage 2 — first living-material loop
- Add one world with conservation-aware ingestion/deposition.
- Give the neural-derived controller limited actions and prices.
- Ensure the altered pixels/mass/geometry produce subsequent sensory changes.
- A **HANDS OFF** run must remain engaging without mouse/touch intervention.
- Implement and test [P02 Conserved Glitter Metabolism](../research/protocols/P02-conserved-glitter-metabolism.md) as one traced material cycle—not a cosmetic particle emitter.

## Stage 3 — build the plug-in racks
- Formalized `BrainAdapter`, `SenseAdapter`, `BodyAdapter`, `WorldAdapter`, `Material`, `Recorder`.
- Add organism/world selection, seed/experiment load/save, restart, time scaling and mobile-safe controls.
- Preserve previous experiment outcomes and configurations.

## Stage 4 — octopus + CHROMAVORE
- Eight simple independently reactive arms with elastic local physics; no need for perfect MuJoCo anatomical reproduction.
- Add pigment stomach/inventory, structured glitter/crystals, bounded geometry vomiting, material costs.
- Keep biologically validated triggers distinct from synthetic selectors.
- Use [P03 Eight-Arm Stirrer](../research/protocols/P03-eight-arm-stirrer.md) as the minimal functional arm-scene experiment; compare local-only reflexes against neural modulation.

## Stage 5 — persistent math/ecology
- Couple two or three material systems (pigment + contour + crystal initially).
- Add history, nutrient replenishment, waste/damage, multi-day accelerated playback and deterministic checkpoints.
- Introduce second organism only after single-agent loops are stable.
- Test [P04 Pigment Notebook](../research/protocols/P04-pigment-notebook.md): allow a mark/channel to carry information into the future; erase/swap traces and remove all hidden answer leakage.

## Stage 6 — learning and diversification
- Begin with controlled readout learning using a frozen neural graph.
- Separate immediate reward, long-term homeostatic drives, satiation, habituation, historical novelty and changing preferences.
- Validate retention, reversal, novel situations and ablations.
- Use [P05 Twin Taste Histories](../research/protocols/P05-twin-taste-histories.md) to distinguish retained learned differences from transient hunger, random drift, or different rendering. Treat mushroom-body-like synaptic plasticity as an independent validated research track.

## Stage 7 — advanced neural substrates
- Inspect larger circuits (pursuit, feeding, olfactory, mushroom body, visual processing), then MaleCNS/BANC as computationally warranted.
- Compare proper matched controls; profile CPU, sparse network storage, GPU use, mobile thermal load.
- Never claim full-brain, full-fidelity, real-time iPhone support on the basis of a neuron count alone.

## Art/export requirements throughout
- Vibrant/high-color workflows, including acid-neon palettes and large smooth contour-band/strata styles.
- Fine rendering at 1:1 and 9:16 minimum; high-resolution PNG and timed GIF/MP4 export when feasible.
- Exact reproducibility from seeds/checkpoints for science, alongside deliberate mutation/chaos controls for art.
- Separate preview FPS, simulation clock and export time.
- No Netlify deploys or GitHub Actions runs merely to edit research/docs. Avoid extra paid APIs.

## Definition of DONE for each delivered experiment
1. Accessible and visibly functional UI with independent body/world/brain controls where applicable.
2. Neural source and channel mapping documented.
3. Genuine feedback (action changes what is subsequently sensed) demonstrated or explicitly labeled absent.
4. Deterministic checkpoint + experiment log.
5. At least one meaningful counterfactual/baseline.
6. Mobile behavior and export claims measured rather than assumed.
7. No regression of prior working experiments.

## Longer-horizon body/world boundary research (R04)

R04 proposes external sensory organs/constructed signaling channels, evolving body compliance, environmental notebooks, limited local law editing and body-as-control-territory definitions. These belong **after** the first five controlled protocols and require instrumentation and provenance before claiming embodied learning.
