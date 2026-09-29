# Reading guide

[Home](../README.md) · [Framework notes](FRAMEWORK.md)

This is a curated route through **12 works cited in the review**, organized around its scientific questions. It is a selective companion guide, not the full bibliography or a survey of all subsequent work. The bracketed reference numbers correspond to the supplied review manuscript.

## 1. Start with scenarios and human feedback

**Riahi, K., et al. (2017).** [The Shared Socioeconomic Pathways and their energy, land use, and greenhouse gas emissions implications: An overview](https://doi.org/10.1016/j.gloenvcha.2016.05.009). *Global Environmental Change*, 42, 153–168. **[29]**

Read for the socioeconomic pathways that underpin scenario-based climate research. Relates to Section 2 of the review.

**Beckage, B., Moore, F. C., and Lacasse, K. (2022).** [Incorporating human behaviour into Earth system modelling](https://doi.org/10.1038/s41562-022-01478-5). *Nature Human Behaviour*, 6, 1493–1502. **[35]**

Read for the existing foundations of behavioral feedback in Earth system modeling. Relates to the introduction and Section 4.

## 2. Understand what AI weather forecasting establishes

**Pathak, J., et al. (2022).** [FourCastNet: A Global Data-driven High-resolution Weather Model using Adaptive Fourier Neural Operators](https://arxiv.org/abs/2202.11214). *arXiv:2202.11214*. **[11]**

Read for the use of adaptive Fourier neural operators in global weather prediction.

**Lam, R., et al. (2023).** [Learning skillful medium-range global weather forecasting](https://doi.org/10.1126/science.adi2336). *Science*, 382, 1416–1421. **[12]**

Read for GraphCast and graph-based global weather prediction.

**Bi, K., et al. (2023).** [Accurate medium-range global weather forecasting with 3D neural networks](https://doi.org/10.1038/s41586-023-06185-3). *Nature*, 619, 533–538. **[13]**

Read for Pangu-Weather and the incorporation of Earth-specific structure into neural weather forecasting.

These three papers connect to Sections 1.2–1.3. When reading them, distinguish finite-lead weather skill from evidence about long-term climate statistics, changing forcing, or endogenous emissions.

## 3. Examine the transition to climate simulation

**Kochkov, D., et al. (2024).** [Neural general circulation models for weather and climate](https://doi.org/10.1038/s41586-024-07744-y). *Nature*, 632, 1060–1066. **[60]**

Read for a hybrid atmospheric model combining a differentiable dynamical core with learned components. Examine the evaluated climate conditions and the limits of extrapolation.

**Watt-Meyer, O., et al. (2025).** [ACE2: accurately learning subseasonal to decadal atmospheric variability and forced responses](https://doi.org/10.1038/s41612-025-01090-0). *npj Climate and Atmospheric Science*, 8, 205. **[23]**

Read for an atmospheric emulator evaluated for variability and responses to changing boundary conditions.

**Cresswell-Clay, N., et al. (2025).** [A Deep Learning Earth System Model for Efficient Simulation of the Observed Climate](https://doi.org/10.1029/2025AV001706). *AGU Advances*, 6, e2025AV001706. **[24]**

Read for DLESyM and coupled atmosphere–ocean-surface modeling of observed climate. Separate evidence about present-climate stability from claims about future forced climates.

These papers connect to Section 1.4. They provide possible foundations for a climate response component; their inclusion here does not imply an implemented behavior–emission–climate loop.

## 4. Follow the aerosol evidence chain

**Bellouin, N., et al. (2020).** [Bounding Global Aerosol Radiative Forcing of Climate Change](https://doi.org/10.1029/2019RG000660). *Reviews of Geophysics*, 58, e2019RG000660. **[10]**

Read for aerosol forcing and its uncertainty. Relates to Section 3.2.

**Zheng, B., et al. (2018).** [Trends in China's anthropogenic emissions since 2010 as the consequence of clean air actions](https://doi.org/10.5194/acp-18-14095-2018). *Atmospheric Chemistry and Physics*, 18, 14095–14111. **[73]**

Read for evidence connecting clean-air measures to changes in China's anthropogenic emissions. Relates to Sections 3.3 and 5.1.

The two papers address different links: emission changes and climate forcing. A coupled framework still needs to examine how those links fit together and how regional climate and behavior respond.

## 5. Add physical constraints and causal reasoning

**Beucler, T., et al. (2021).** [Enforcing Analytic Constraints in Neural Networks Emulating Physical Systems](https://doi.org/10.1103/PhysRevLett.126.098302). *Physical Review Letters*, 126, 098302. **[57]**

Read for enforcing physical constraints in learned emulators. Relates to Sections 1.3 and 4.2–4.3.

**Runge, J., et al. (2019).** [Inferring causation from time series in Earth system sciences](https://doi.org/10.1038/s41467-019-10105-3). *Nature Communications*, 10, 2553. **[83]**

Read for the assumptions and challenges of causal inference from Earth system time series. Relates to Sections 4–5.

## Reading questions

For each method, identify its inputs, outputs, time horizon, physical constraints, and evaluation conditions. For a claimed feedback, ask which link is observed, which is estimated, and which remains a modeling assumption.

For the complete bibliography, including work on climate uncertainty, integrated assessment, climate economics, parameterization, and Chinese regional studies, consult the review article.
