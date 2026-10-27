# The impossible vivarium — modular reference architecture

This is a proposed **design blueprint**, not a claim that the modules already exist in the app.

## Minimum closed-loop system

```text
      persistent world W(t) + body B(t) + artificial physiology H(t)
                      |
           observation / sampling
                      |
          sensory encoder E(sense)
                      |
       connectome-derived dynamics N(t)
                      |
      logged neural feature bottleneck z(t)
                      |
         small action decoder D(z,H)
                      |
      local body controllers + world physics P
                      |
       body/world state W(t+1), B(t+1)
                      +-------- feedback to sampling
```

### Separately replaceable layers

1. **Neural substrate:** frozen 6,203-cell verified escape-related subcircuit initially; later separately validated pursuit, feeding, mushroom body or full-CNS configurations.
2. **Sense rack:** vision/looming, contact, odor-like gradient, pigment density, stress, curvature, waves, sparkle, novelty, topology, other organisms. Log which mappings are genuinely biologically motivated and which are invented.
3. **Neural feature bridge:** identifiable left/right neural readouts, firing rates, timing and chosen latency, *not only* one global “neural energy” scalar.
4. **Actuator vocabulary:** approach, avoid, turn, withdraw, reach, eat, secrete, nucleate, deposit, stir, repair, attach, emit, reproduce, wait. Every action has costs and limits.
5. **Body shop:** octopus/soft arms; pixel-eating shape; particle swarm; ribbon/spline; colony; distributed pigment patches; no localized body, only controllable field parameters.
6. **World forge:** Cahn–Hilliard; Allen–Cahn; Gray–Scott; fluid flow; cellular automata; crystals/DLA; waves/cymatics; optical/light fields; fractals, graph rewriting; coupled materials.
7. **Physiology/biography:** hunger/energy, pigment inventories, satiety, damage, metabolic precursor, explored locations, memory and persistent learned state.
8. **Rendering/export:** vivid high-quality compositing, optional flat neon/contour-band rendering, deterministic high-res rerender from checkpoints and event logs.
9. **Experiment console:** intervention tools, telemetry, snapshots, split-screen controls, seeds, causal comparisons, report exports.

## Modes

- **HANDS OFF:** agent/world keep evolving without user gestures. The code should clearly expose whether exploratory movement is driven by biological neural activity, a synthetic baseline, a safety controller or randomness.
- **INTERVENE:** add obstacles/food/field perturbations, stimulate or silence channels, switch materials, inject physics events.
- **EXPERIMENT:** same starting seed with multiple controller conditions, matched budgets, plots/metrics, and playback.

## Prototype fidelity order

**First:** preserve current working neural kernel; modest coupled 2D world; independent render FPS; low-dimensional verified neural outputs; deterministic checkpoints.

**Next:** add body/environment plugins through interfaces without modifying the model.

**Later:** validated readout adaptation, mushroom-body experiments, multi-agent ecology, novel senses and growing morphology.

**Finally (if justified):** larger MaleCNS/BANC/full-brain tests and dedicated performance backends.

## Recommended data contracts (proposed)

```text
NeuralObservation { timestamp, population_id, mean_rate, spike_count, metadata }
SyntheticSense    { name, unit, raw_value, encoder_version, target_population }
ActionProposal    { time, source: neural|adapter|script|random, action, amount, target, cost }
WorldEvent        { time, location, material_before, material_after, cause, seed }
ExperimentRecord  { model_version, circuit_hash, decoder_version, body_id, world_id,
                    seed, clock_rates, control_condition, checkpoints, metrics }
```

Use typed/validated structures and deterministic ordering; the exact implementation language is open.

## Materials do the visual work

The neural system chooses **what, when, where, intensity, and budget**. A local simulator handles fluid trajectories, sparkles, rod bending, crystal microstructure, collision resolution and fractal expansion. That is legitimate hierarchical embodiment **provided the contribution from each part stays visible**.

For a glitter-eater, eating must transfer material from the world to an inventory, and emission must cost stored precursors; indiscriminate pixel deletion + random particle spawning is a visual effect, not a tracked metabolism.

## Performance/export notes

- Keep neural integration, sensory sampling, action decoding, physics, material evolution, rendering and wall-clock playback as distinct clocks.
- A 60 FPS display does **not** imply real-time full-brain millisecond neural integration.
- Profile sparse event traffic, model memory, CPU/GPU transfer, battery/thermals on actual hardware before committing to “mobile real time.”
- Export should capture world/geometry/seeds/checkpoints; rerender at higher resolution with appropriate antialiasing/shading rather than merely scaling a tiny screenshot.
- Prefer no paid APIs, no unnecessary deployment, and independent local operation for interactive art experiments.
