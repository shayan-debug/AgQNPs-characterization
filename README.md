# Ag@QNPs Characterization Data

[![DOI](https://img.shields.io/badge/DOI-10.1038%2Fs41598--025--96684--2-blue)](https://doi.org/10.1038/s41598-025-96684-2)
[![Python](https://img.shields.io/badge/Python-3.10-green)](https://www.python.org/)
[![Data source](https://img.shields.io/badge/Data-Scientific%20Reports%202025-orange)](https://doi.org/10.1038/s41598-025-96684-2)

Visualization and documentation of physicochemical characterization data for quercetin-loaded silver nanoparticles (Ag@QNPs) as urease inhibitors.

> **Data source:** All experimental values are from the published paper:
> Asadi, S. et al. *Enhanced urease inhibitory activity of quercetin via conjugation with silver nanoparticles: synthesis, characterization, and DFT study.* Scientific Reports 15, 11892 (2025). https://doi.org/10.1038/s41598-025-96684-2

---

## Repository Structure

```
AgQNPs-characterization/
├── notebooks/
│   └── characterization_analysis.ipynb   # Full visualization pipeline
├── data/
│   ├── characterization_summary.csv      # DLS, UV-Vis, zeta potential
│   ├── ic50_data.csv                     # Urease inhibition IC₅₀ values
│   ├── xrd_peaks.csv                     # XRD 2θ peak positions
│   └── summary_table.csv                 # Generated summary (output)
├── figures/                              # Generated plots (output)
│   ├── uvvis_peaks.png
│   ├── dls_zeta.png
│   ├── xrd_peaks.png
│   └── ic50_comparison.png
└── README.md
```

---

## Key Results

### Physicochemical Characterization

| Parameter | AgNPs | Ag@QNPs | Method |
|-----------|-------|---------|--------|
| UV-Vis SPR peak | 407 nm | 445 nm | UV-Vis (Jenway 6300) |
| Hydrodynamic diameter | 70.85 ± 9.68 nm | 104.5 ± 8.53 nm | DLS (Malvern ZEN3600) |
| Zeta potential | −23.5 ± 3.16 mV | −15.2 ± 2.3 mV | DLS |
| TEM size range | 59–69 nm | 57–77 nm | TEM (PHILIPS EM208s) |

The 38 nm red-shift in UV-Vis SPR peak and the increase in hydrodynamic diameter confirm successful quercetin loading onto AgNPs.

### XRD — Crystal Structure

| 2θ (°) | hkl | Assignment |
|--------|-----|------------|
| 38.10 | 111 | FCC Ag (JCPDS 087-0717) |
| 44.32 | 200 | FCC Ag |
| 64.44 | 220 | FCC Ag |
| 77.41 | 311 | FCC Ag |

Crystallite size calculated by Debye-Scherrer equation: **D = 0.62 nm**

### Urease Inhibitory Activity

| Compound | IC₅₀ (µg/mL) | Notes |
|----------|-------------|-------|
| Quercetin (free) | 9.581 ± 0.38 | — |
| **Ag@QNPs** | **0.473 ± 0.09** | ~20× more potent than free quercetin |
| Hydroxyurea | 7.6 | Positive control |

Ag@QNPs show ~20× greater potency than free quercetin on a 
total nanoparticle mass basis (IC₅₀: 0.473 vs 9.581 µg/mL). 
On a quercetin-equivalent basis (12% loading efficiency), 
the effective IC₅₀ of quercetin in Ag@QNPs is approximately 
0.057 µg/mL, representing ~170× improvement over free quercetin.

---

## How to Run

Open in Google Colab — no local installation required:

```
notebooks/characterization_analysis.ipynb
```

Dependencies: `pandas`, `matplotlib`, `numpy` (all pre-installed in Colab)

---

## Citation

If you use this data or notebook, please cite the original paper:

> Asadi, S. et al. *Enhanced urease inhibitory activity of quercetin via conjugation with silver nanoparticles: synthesis, characterization, and DFT study.* Scientific Reports 15, 11892 (2025). https://doi.org/10.1038/s41598-025-96684-2

---

## Author

**Shayan Asadi** — Medicinal Chemistry, Zanjan University of Medical Sciences  
GitHub: [@shayan-debug](https://github.com/shayan-debug)
