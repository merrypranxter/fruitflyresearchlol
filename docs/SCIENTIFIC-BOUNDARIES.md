# Scientific boundaries & evidence labels

## The distinction we refuse to blur

`connectome data → dynamical equations → synthetic sensory input → neural activity → action decoder → body/world engine → next sensory input`

Each arrow can contain substantive engineering. Seeing realistic walking, expressive art, clever gameplay or a glitter explosion does **not** establish that a scanned fly understands its task, likes the outcome, or has been fully emulated.

### Labels for assertions (adopted from R03)

- **D — Demonstrated:** A specified published result or documented implementation supports the particular claim. A project video/README is *author report*, not independent replication.
- **F — Engineering-feasible:** Known computational pieces plausibly compose; behavioral results in this exact hybrid are still untested.
- **R — Research frontier:** Coherent but significant uncertainty in learning, stability, coordination, or biological validity.
- **S — Speculative:** Coherent hypothesis lacking validated implementation.
- **X — Major additions required:** The stated biological substrate lacks necessary machinery without engineering new modules.

Mark these per **claim**, not once per project. A neural octopus may have F-level actuation while adaptive dexterity remains R.

## What is established in the source documents (subject to primary-source verification)

- High-resolution connectome datasets provide structural connectivity for the adult fly brain and newer brain-plus-ventral-nerve-cord preparations.
- Simplified connectome-constrained models can generate informative predicted neural responses when specified populations are stimulated.
- Engineered systems can close neural → action → environment → neural loops.
- External trained policies can learn to use connectome-derived features for tasks unlike natural fly tasks.
- Some controlled comparisons suggest biological network structure can be useful for certain *trained* tasks; that does not generalize to all tasks or explain the entire behavior.

## NOT established

- Recovery of an individual fly's complete living state, learned history, identity, or consciousness.
- That the static graph alone spontaneously generates the natural complete fly behavioral repertoire.
- That crude LIF + synthetic “dopamine” automatically confers durable, useful associative learning.
- That an 8-armed octopus, glitter eater, mathematical god garden, etc. has already been validated as a biologically meaningful fly-brain organism.
- That aesthetic reward implies the network experiences beauty, pleasure, desire or suffering.
- That increasing neuron count automatically increases capability, scientific fidelity or GPU performance.
- That a beautiful image implies correct fluid/chemistry equations or correct attribution to neural topology.

## Attribution checklist for every experiment

Record:
1. Exact connectome dataset/version and included neuron subset; graph filters, connection thresholds, predicted transmitter signs, weights.
2. Simulated neural equations, time step, initial state, background drive and random seed.
3. Every sensory variable, encoder mapping, stimulated populations and whether mapping is naturalistic, pathway-bypassing or wholly synthetic.
4. Neural populations/latents read out; each neural vs scripted vs stochastic action contribution.
5. Trained parameter counts in encoder, neural core, decoder, body controller, and learned value system separately.
6. Local body physics, material conservation rules, numerical solver, timestep and resampling rates.
7. Whether the outcome is a one-off observation, a reproducible result, a tested preference or a validated task.
8. Appropriate control conditions: intact, silenced, replay, time-shuffled, disconnected feedback, rewired, conventional matched controller.
9. What changed after experience, where, and whether it persists after restart/reversal.
10. Known failures and negative tests (preserve them).

## A particularly important control distinction

**Acute dependence:** Hold a learned decoder fixed; silence/scramble its neural inputs. Does the current assembled controller rely on its current circuit?

**Architectural usefulness:** Retrain comparably sized decoders on intact, rewired, random and conventional substrates under equal budgets. Is the biological structure actually advantageous?

Failing the first after disruption is not proof of the second.

## Biological language hygiene

Say “computed curvature was encoded into an artificial neural input,” not “fly neurons naturally sense mathematical curvature.”

Say “artificial satiety/reward variables” instead of implying an original scanned fly's wants were recovered.

Say “neural-influenced pattern production” until a causal contribution and feedback loop are measured.
