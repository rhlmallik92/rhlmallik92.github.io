---
layout: page
title: Research Projects
---
## Isolated DC-DC Topologies (QAB)
![System Diagram](/assets/images/System_diagram.png)
*Figure 1: Control architecture and system-level diagram of the modular converter system.*
During my research at the **University of Texas at Austin** and **University of Washington**, I developed control for a novel modular power conversion architecture using a Quadruple Active Bridge (QAB) topology to interface PV sources with medium-voltage (13.2kV) grids.

### Decentralized Control of Series-Connected Modules
* **Unified Control:** Designed an architecture for simultaneous MPPT, DC-link regulation, and AC-side power control.
* **Autonomous Synchronization:** Developed a communication-less power-sharing strategy for modular, series-connected grid interfaces.
* **Stability Analysis:** Leveraged **Singular Perturbation Theory** to decompose control timescales, providing a rigorous framework for parametric selection and ensuring multi-module stability.
  
### Experimental Setup and Key Results
* **Multi-Timescale Control (Fig. 3):** Confirms autonomous **MPPT** tracking for Module #1 while Modules #2 and #3 maintain stable DC power, validating the singular perturbation-based design.
* **AC/DC Performance (Fig. 3):** High-resolution waveforms demonstrate precise **dVOC** synchronization and stable regulation of three-phase currents across the series-connected modules.
* **Grid-Forming Resilience (Fig. 4):** Successfully maintains system stability during a sudden grid frequency excursion from 60 Hz to 59.4 Hz.
* **Autonomous Power Sharing (Fig. 4):** Modules #2 and #3 automatically increased power injection via droop laws in response to frequency changes, proving robust decentralized operation without centralized communication.
![AC and DC Performance](/assets/images/AcandDC.png)
*Figure 3: Experimental waveforms showing AC and DC side performance of the QAB converter.*
![Frequency Excursion Analysis](/assets/images/FrequencyExcursionver2.png)
*Figure 4: Frequency excursion analysis demonstrating system stability during grid transients.*

![Hardware Setup](/assets/images/NewsetupPic.png)
*Figure 2: Laboratory testbench including the modular converter stacks and real-time control interface.*
Each module achieved a peak **96.5% efficiency** for rated conditions of 250 V dc input and 1 kW peak PV power and a peak **97.1% efficiency** for 1kV dc input and 7.5 kW peak PV power.

---

