---
id: l016
title: "Near-Miss Color Asymmetry — Small Deviations Cost More Than Large Departures"
layer: L2
date: 2026-02-26
contributor: Stefan Kovalik
tags:
  - color-perception
  - near-miss-asymmetry
  - non-riemannian
  - OKLCH
  - design-tokens
  - bujack-2022
  - brainard-2022
source: PFD analysis of Schrödinger's color theory + Bujack et al. (2022, PNAS) + Brainard (2022, PNAS commentary)
---

# Learning 16: Near-Miss Color Asymmetry — Small Deviations Cost More Than Large Departures

**Insight:** Human color perception is non-additive: large color differences are perceived as *less* than the sum of their small-step components (Bujack et al., 2022 — "diminishing returns"). This means the perceptual cost curve is non-linear. A brand blue that's 3% off-target imposes *disproportionate* processing cost compared to a completely different color, because small deviations sit in the steep, high-sensitivity zone of the perceptual metric where prediction error is maximal. PFD's L2 heuristic "3-4 colors, consistent" is directionally correct but operates at the wrong level of abstraction: "consistent" in hex/RGB space ≠ consistent in perceptual space. Every CSS gradient, palette interpolation, and color scale built linear in hex is non-linear in perception — a systematic L2 fluency violation invisible to the designer. **Practical implication:** near-miss color deviations (slightly off-brand, almost-but-not-quite matching) are the highest-cost L2 violations, more disruptive than using a completely different color. Design-token linting that flags off-system values should weight near-misses as more severe than far-misses. **Framework connection:** the Feb 2026 Los Alamos finding (Bujack et al., 2025, *Computer Graphics Forum*) that hue, saturation, and lightness are intrinsic geometric properties of the color metric — not learned or cultural — confirms PFD's hardware/software distinction for the color channel specifically. Color *structure* is hardware (universal geometry). Color *meaning* is software (cultural, context-dependent). **Caveat:** the non-additivity finding rests on aggregate data collected online across subjects; Brainard (2022, PNAS commentary — "Proximity Matters") flags that aggregate non-Riemannian behavior could be a statistical artifact of averaging individually Riemannian observers with different parameters (cone ratios, lens yellowing). The design implication holds regardless — near-misses are costly whether the mechanism is geometric or statistical — but the theoretical claim ("color space is non-Riemannian") should be cited as a theoretical framework, not settled law. The Feb 2026 "Schrödinger's theory completed" headlines overstate an incremental mathematical contribution (formalizing one missing component, the neutral axis). Cite the non-additivity finding cautiously; don't cite the "completed" framing.
