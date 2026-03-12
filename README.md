# agent-society-simulator
# Emergent Agent Society Simulator – Three-World Comparative Experiment & Knowledge Graph Analysis

This repository shares the outcomes of a long-running agent-based simulation experiment that explores how scientific knowledge (specifically a hypothetical gravity-modulation framework called MHM) emerges, spreads, and consolidates under different societal conditions.

The simulation is powered by a custom generative engine that creates autonomous agents with realistic emotional, logical, social, and creative behaviors. Agents live full simulated lives, form collaborations, debate ideas, publish findings, migrate during crises, and build cumulative knowledge over decades — all without hard-coded templates or scripted events. Every outcome emerges organically from agent interactions.

**Important**: This repo contains only the *results* and analysis — no simulation source code, no internal engine details, and no proprietary components are included.

## Overview of the Simulation Engine

The engine generates persistent, evolving societies of agents that:
- Exhibit human-like emotions, reasoning, planning, and social dynamics
- Form institutions, publish papers, conduct experiments, and reach consensus
- Respond to external shocks (wars, plagues, famines, funding suppression)
- Carry knowledge across generations and migrations
- Produce long-term coherent history (decades to centuries)

No templates or scripted narratives are used — all events, discoveries, migrations, deaths, and scientific progress arise from agent decisions and interactions.

## The Three-World Experiment (150 Simulated Years, Seed=7)

We ran the same starting conditions (2026 CE, initial physics knowledge) across three parallel worlds with different societal constraints:

1. **Open Science** (collaborative, no censorship)  
   - Fastest unification: full synthesis in **11 years**  
   - No major losses; clean consensus on all components

2. **Suppression** (censorship, funding blocks, IP wars)  
   - Delayed unification: **16 years**  
   - One migration event (knowledge rescued)  
   - Still succeeds, but with friction

3. **Collapse** (war, plague, famine, high scientist mortality)  
   - **Failed** — no full synthesis in 150 years  
   - 16 scientist deaths, 9 migrations, only partial knowledge preserved

Key tracked elements:
- Time to consensus
- Migration events (scientists fleeing with partial knowledge)
- Scientist deaths
- Bottleneck components (e.g., `decoupling_condition` repeatedly delayed)

**Narrative verdict summary**:
- Open Science wins cleanly.
- Suppression slows but does not kill progress.
- Collapse destroys cumulative science.

Full log excerpt: [mhm_three_worlds 2.txt](mhm_three_worlds%202.txt)

## Knowledge Graph Structural Analysis

For the successful **Open Science** world, we analyzed the discovery process as a directed dependency graph:

- 8 sequential steps (nodes) from initial measurements to full synthesis
- Critical path length: **11.8 years** (longest unavoidable chain)
- Main bottleneck: `full_static_eq` (2.1 years alone)
- 8 parallelizable waves (avg 1.4 nodes per wave)
- Consensus gate (requiring 3 independent measurements) adds ~3.5 years overhead

**Key findings**:
- Theoretical minimum time: 11.8 years
- Optimistic (higher precision/discovery rate): 7.2 years
- Pessimistic (half scientists, lower precision): 56.8 years
- Observed range in sim: 13–18 years (realistic human overhead)

Full graph analysis: [mhm_graph_analysis.txt](mhm_graph_analysis.txt)

## Real-World Industries & Applications

This type of generative simulation engine — where agents live full lives, build knowledge, and evolve societies — has broad potential beyond pure research:

- **Urban planning & smart cities**  
  Simulate decades of policy changes, migration, economic shifts, and infrastructure evolution to test resilience against crises.

- **Geopolitical & strategic forecasting**  
  Model how nations, alliances, and technologies interact over 50–200 years under different governance models.

- **Drug discovery & epidemiology**  
  Run long-term societal responses to pandemics, vaccine hesitancy, misinformation, and public health policies.

- **Corporate strategy & innovation labs**  
  Test how R&D teams, funding models, and IP strategies affect breakthrough timelines in competitive markets.

- **Game development & interactive storytelling**  
  Create living worlds (e.g., next-gen GTA-style cities) where NPCs evolve independent histories, remember player actions across generations, and generate infinite emergent narratives.

- **Education & history simulation**  
  Let students "enter" historical periods and interact with agents who live authentic lives shaped by real-era constraints.

- **Ethical AI & societal risk assessment**  
  Introduce emerging tech (AGI, longevity, climate fixes) → observe moral, political, and economic fallout over decades.

The data and insights in this repository come entirely from the engine's emergent behavior — no hard-coded templates, scripted events, or pre-written histories were used.

## Files in this Repository

- `mhm_three_worlds 2.txt` — Raw log of the three parallel worlds experiment (150 simulated years).
- `mhm_graph_analysis.txt` — Detailed knowledge-graph breakdown of the successful Open Science run, including critical path, bottlenecks, and waves.

## License

MIT License — feel free to use, adapt, and share the documents and analysis.

If you find this interesting or run similar simulations, open an issue or PR to discuss!

