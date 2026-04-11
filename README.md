# Inlet Aerodynamic Limitations and Thermal Failure Analysis of the HAL Tejas Mk1
## A First-Principles Investigation of the 2025 Dubai Airshow Incident

**Author:** Ayush Sreejith  
**Affiliation:** Independent Researcher, Palakkad, Kerala, India  
**Contact:** ayushsreejith.research@gmail.com  
**Date:** April 2026  
**Status:** Preprint — To be submitted to AIAA Journal of Propulsion and Power

---

### Dedication

*This paper is dedicated to the memory of Wing Commander Namansh Syal, Indian Air Force, who gave his life representing India at Dubai on November 21, 2025. He was 34 years old.*

---

### Abstract

On November 21, 2025, Wing Commander Namansh Syal of the Indian Air Force was killed when a HAL Tejas Mk1 light combat aircraft was lost during an aerobatic display at Al Maktoum International Airport, Dubai World Central. He did not eject. The aircraft impacted the ground at approximately 14:10 hrs local time following an unrecovered descent from a low-altitude negative-G maneuver. A Court of Inquiry was immediately ordered by the IAF.

This paper presents a first-principles aerodynamic and thermodynamic analysis of the Tejas Mk1 inlet system in response to that loss. Using published engine specifications, NASA exhaust survey data for the F404 family, flight timeline reconstruction from open-source footage, and corrected atmospheric conditions for the incident site, a cumulative thermal-aerodynamic failure chain is developed.

The analysis demonstrates that the lateral intake geometry, while adequate under standard operating conditions, exhibits compounded vulnerability under sustained high-G aerobatic maneuvering in hot, humid environments. The bifurcated side-inlet configuration imposes specific boundary-layer ingestion penalties under negative-G attitudes that a chin or diverterless supersonic inlet (DSI) geometry would not encounter. A flight-timeline-based thermal accumulation model shows that compressor stall margin was progressively eroded throughout the display sequence, with the final negative-G maneuver acting as a threshold event within an already degraded propulsion system rather than an isolated mechanical cause.

The analysis does not assert definitive causation — that determination requires access to flight recorder and telemetry data held by the Court of Inquiry — but establishes a physically consistent and evidence-supported pathway to compressor instability under the documented conditions. The paper concludes with proposed inlet redesign alternatives for the Tejas Mk2 and future LCA variants.

---

### Key Findings

- The Tejas Mk1 bifurcated lateral inlet configuration produces compounding DC60 distortion under high-AoA and negative-G conditions not adequately mitigated by the fixed-geometry splitter plate diverter
- A lumped-parameter thermal accumulation model, calibrated against NASA F404 exhaust data (TM-88273), demonstrates that the 1–4 s recovery intervals between aerobatic maneuvers are insufficient for thermal dissipation given the F404's 30–45 s thermal time constant
- Stall margin analysis using the reduced-order model shows threshold failure onset consistent with the documented flight profile
- The Mk1A's documented 3% pressure recovery improvement via the three-door AAID system constitutes implicit acknowledgment of a pre-existing Mk1 inlet performance deficit
- Three redesign alternatives are evaluated and ranked: DSI configuration, chin/ventral intake, and rear-shifted lateral intake

---

### Primary Sources

All analysis is conducted from publicly available data. No classified information is used or required.

| Source | Role in Analysis |
|--------|-----------------|
| NASA TM-88273 (Walton & Burcham, 1986) | F404-GE-400 exhaust temperature reference |
| NASA TM-104329 (Steenken et al., 1993) | F/A-18A HARV inlet distortion during high-AoA departed flight |
| NASA TM-100991 (Burcham & Fullerton, 1988) | F404 transient engine response and stall characteristics |
| SAE ARP1420C | Inlet-engine distortion compatibility standard |
| Triantafyllou et al., Aeronautical Journal, 2015 | Total pressure distortion at military aircraft AIP |
| Seddon & Goldsmith, Intake Aerodynamics (1999) | Inlet aerodynamic theory and modelling |
| Mattingly, Elements of Gas Turbine Propulsion (1996) | Compressor thermodynamic framework |
| GE Aerospace F404 Data Sheet | Engine specifications |
| HAL / IDRW — Mk1A AAID documentation | 3% pressure recovery improvement evidence |

---

### Repository Contents

```
tejas-inlet-analysis/
├── paper/
│   └── Sreejith_Tejas_Inlet_Thermal_Analysis_2026.pdf
├── figures/
│   ├── dc60.png
│   ├── massflow.png
│   ├── compressor.png
│   ├── stall_margin.png
│   ├── thermal_accumulation.png
│   ├── dsi_graphs/
│   │   ├── dsi_dc60.png
│   │   ├── dsi_mass.png
│   │   ├── dsi_stall.png
│   │   ├── dsi_thermal.png
│   │   └── dsi_compressor.png
│   ├── chin_graphs/
│   │   ├── chin_dc60.png
│   │   ├── chin_mass.png
│   │   ├── chin_stall.png
│   │   ├── chin_thermal.png
│   │   └── chin_compressor.png
│   └── rear_graphs/
│       ├── rear_dc60.png
│       ├── rear_mass.png
│       ├── rear_stall.png
│       ├── rear_thermal.png
│       └── rear_compressor.png
├── src/
│   └── AIAA_Tejas_Dubai_FINAL.tex
├── LICENSE
└── README.md
```

---

### Disclaimer

This analysis is based on publicly available data and reconstructed flight conditions. It does not represent an official accident determination. The analysis does not assert causation, but identifies a consistent mechanism through which inlet–engine interaction may reduce propulsion stability under the conditions documented at Dubai on November 21, 2025. The Court of Inquiry constituted by the Indian Air Force holds the flight recorder and telemetry data required for a definitive determination.

---

### Citation

```
Sreejith, A., "Inlet Aerodynamic Limitations and Thermal Failure Analysis of the
HAL Tejas Mk1: A First-Principles Investigation of the 2025 Dubai Airshow Incident,"
Independent Research Preprint, Palakkad, Kerala, India, April 2026.
Available: https://github.com/ayushsreejith/tejas-inlet-analysis
```

---

© 2026 Ayush Sreejith. All rights reserved. See LICENSE for terms.
