# Framework notes

[Home](../README.md) · [Reading guide](READING_GUIDE.md)

These companion notes summarize Sections 2–5 of the [review article](https://doi.org/10.12006/j.issn.1673-1719.2026.146). The module descriptions are conceptual interfaces for future research. They do not specify an implemented model, a validated benchmark, or a committed software roadmap.

## 1. The scientific question

Many climate projection experiments prescribe emission or concentration pathways and simulate the physical response. The review asks how climate impacts could also shape the behavioral and policy processes that generate those pathways.

The resulting loop connects climate conditions and risk signals, social responses, changing emissions and forcing, and the physical climate response. Existing Earth system models, integrated assessment models, and social-climate models provide complementary foundations. AI methods can support the data integration and computational interfaces between them.

## 2. Module interfaces

| Module | Inputs discussed in the review | Outputs or interface variables | Central evaluation question |
| --- | --- | --- | --- |
| Climate state and risk representation | Temperature, precipitation, extremes, air quality, health risk, exposure | Climate pressure and risk signals that can enter behavior models | Are signals stable and representative across regions and scales? |
| Behavior and policy response | Risk signals, economic conditions, energy systems, institutional context | Policy intensity, energy substitution, adaptation investment, pollution control | Are response direction, magnitude, delay, and regional differences credible? |
| Emissions and forcing response | Activity levels, energy mix, policy variables, land-use change | Emissions, concentrations, aerosol optical depth, radiative forcing | Are the mappings consistent with inventories, observations, and physical constraints? |
| Physical climate core | Forcing or boundary conditions appropriate to the selected model | Temperature, precipitation, radiation, circulation, extremes | Does the model preserve climate statistics and respond appropriately to forcing? |
| Constraints and interpretation | Module outputs, physical budgets, causal assumptions, ensembles | Consistency diagnostics, uncertainty estimates, sensitivity and counterfactual analyses | Can errors and uncertainty be traced to identifiable processes? |

Emission fluxes, concentration fields, aerosol optical depth, and effective radiative forcing are distinct interface quantities. Their use depends on whether the receiving component is an Earth system model, a chemical transport model, a simplified climate model, or a learned emulator. Coupling requires compatible variables, units, spatial support, time resolution, and boundary conditions.

## 3. Roles for AI methods

| Method family | Role in the proposed framework | Key requirement |
| --- | --- | --- |
| Representation learning and sequence models | Align heterogeneous observations and characterize delayed responses | Track sampling differences, temporal alignment, and observation bias |
| Causal inference | Estimate effects of climate pressures or policy interventions and construct counterfactuals | State identification assumptions and address confounding |
| Bayesian hierarchical models | Represent regional and sectoral heterogeneity and parameter uncertainty | Assess identifiability and posterior uncertainty |
| Reinforcement learning | Explore sequential policy pathways with delayed outcomes and constraints | Distinguish a chosen policy objective from a prediction of actual behavior |
| Neural operators and climate emulators | Accelerate repeated simulations of forcing-to-response mappings | Evaluate long integrations and generalization across forcing conditions |
| Physics-constrained and hybrid models | Incorporate conservation, dynamics, and boundary consistency | Measure budget errors and stability alongside predictive accuracy |

These methods address different tasks. Their inclusion in the review does not imply that they have already been combined or empirically validated in one end-to-end system. Reinforcement learning is discussed as a tool for simulated policy-path exploration, including offline or model-based approaches.

## 4. Evaluation principles

The review distinguishes several dimensions of credibility:

| Dimension | Evidence to examine |
| --- | --- |
| Physical climate fidelity | Mean climate, variability, variance spectra, extremes, regional biases, and responses to forcing |
| Long-term consistency | Drift, energy and water closure, mass conservation, radiation budgets, and compatible boundary conditions |
| Behavioral credibility | Response direction, strength, lag, regional heterogeneity, and consistency with historical evidence |
| Causal interpretation | Identification assumptions, confounders, policy-shock evidence, and counterfactual consistency |
| Uncertainty and policy sensitivity | Internal variability, model structure, behavior, policy pathways, and parameter uncertainty |

Short-range forecast accuracy alone does not establish long-term climate credibility. Historical reconstruction, policy-shock natural experiments, counterfactual analyses, and comparisons across regional cases are discussed as complementary evaluation routes. The review does not report a new numerical benchmark or a quantitative decomposition of uncertainty contributions.

## 5. Aerosols and the China case

Aerosols offer a tractable entry point because they respond quickly to changes in activity and pollution control, exhibit regional structure, and influence climate through radiation and cloud interactions. China's clean-air actions provide a context for examining policy interventions alongside emissions, air quality, satellite observations, and climate variables.

Section 5.1 discusses three levels of evaluation:

1. **Behavior and policy:** explain regional differences in pollution-control intensity and emission changes.
2. **Emissions and forcing:** relate changes in relevant pollutants and precursors to aerosol optical depth, air quality, and radiative forcing.
3. **Physical climate response:** examine the associated temperature, precipitation, radiation, and monsoon responses.

Evidence for an individual link does not by itself validate the full feedback loop. Aerosol studies also do not replace the treatment of long-lived greenhouse gases, land-use change, or other climate processes.

## 6. Open research questions

- How can behavioral response functions be identified from observations while accounting for economic and institutional confounders?
- How should policy and social responses at monthly or annual scales be coupled to climate dynamics across longer time scales?
- How can emissions inventories, policy text, remote sensing, and socioeconomic statistics be aligned without concealing measurement bias?
- Which diagnostics can identify whether failures originate in the behavior module, emissions mapping, climate core, or their coupling?
- How can a model separate predictions of what people may do from policy objectives about what they should do?

These are research directions discussed in the review. No future code release or implementation schedule is implied.
