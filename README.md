# Inverse Pass-Through Spectrum — 23 Points, 21 Orders of Magnitude (Data Companion Repo)

Data companion of:

> Qin, Chao (2026). *Nucleated Self-Excitation Pass-Through: The Exchange Account of Two Kinds of Motion and the Pass-Through Spectrum.* Zenodo. doi:10.5281/zenodo.23874617 (v1.2) · concept doi:10.5281/zenodo.23858235 (all versions) · CC-BY-4.0.

The same CSV ships with the Zenodo record; this repository makes it directly reusable (clone/fetch/csv-parse) and version-tracked.

## What this is

The **inverse pass-through spectrum**: 23 data points on a unified mean-free-path scale λ = 1/(nσ), covering six classes — gravitational waves (1; resonance-limit caliber, flagged off-scale in cross-class comparison), neutrinos (3), γ/X rays (5), visible light (4; fiber 0.20 dB/km), radio (4), and sound (2; end-of-spectrum control rows). The measured span is 2.1×10¹⁹ cm to 0.021 cm — **21 orders of magnitude**.

Three readings (paper §4): (1) class-level inversion holds strictly under the same-medium constraint; (2) the four crossings are readings, not counterexamples — pass-through is a three-place function of class × energy × medium; (3) the 21-order span is the empirical display of the interface permeability spectrum (attenuation as a first ontological parameter of media).

## File

`inverse_pass_through_spectrum_v0.1.csv` — 23 rows + header. Column glossary (header is in Chinese):

| Column | Meaning |
|---|---|
| 序号 | row id |
| 类 | wave class (引力波/中微子/γX/可见光/无线电/声) |
| 代表能量或频段 | representative energy or frequency band |
| 介质 | medium assumed (with density stated) |
| 原始数值 | source quantity (e.g. cross-section σ) |
| 原始口径 | source caliber of that quantity |
| 换算公式 | conversion formula used (λ=1/(nσ) with the density value) |
| λ_cm | mean free path in cm (unified scale) |
| λ_显示 | display-scale value (ly / km / cm) |
| 来源类型 | source type (direct paper read / table read / database) |
| 来源或DOI | source or DOI of the cross-section |
| 核验状态 | verification status (crossref pass / errata recorded) |
| 口径级 | caliber level (computed / direct read) |

Every cross-section carries a DOI; all DOIs passed crossref verification, with errata recorded in-file (verification column). Matter-density assumptions are explicit per row (paper Appendix A scale declaration).

## Related

- Protein companion paper (atomic-level chain): doi:10.5281/zenodo.23858233 (concept) — reasoning-chain repo: `vortex-QC/nucleated-self-excitation-chain`
- v1.2 adds §5 the speed spectrum (complex attenuation; superposition/coupled self-excitation dichotomy; v = c·cos²θ) — the rate axis is the conjugate reading of this magnitude axis.

## License

CC-BY-4.0 (as the source paper). Author: Chao Qin (ORCID 0009-0006-2000-5644).
