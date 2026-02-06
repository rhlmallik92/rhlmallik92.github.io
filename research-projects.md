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
## Three-Phase Grid-Forming (GFM) Inverter Design
I designed and built the  5 kVA three-phase two-level inverter at the **University of Texas at Austin**. Using these inverters, I demonstrated the design and interoperability of grid-forming inverters using heterogeneous control laws (dVOC, Droop, and VSM) to ensure grid stability and seamless power sharing. The PCB files and design documnets are here: [unifi link](https://github.com/unifi-consortium/ThreePhaseGFM_C2000).

### Hardware Development & Specifications
* **High-Efficiency Design:** Designed and manufactured a **400 Vdc, 5 kVA three-phase 2-level inverter** featuring SiC MOSFETs for high-frequency operation and power density.
* **Embedded Control:** Fully implemented on the **TI C2000 (F28379D) MCU**, managing high-speed current and voltage loops alongside advanced synchronization algorithms ([codes](https://github.com/unifi-consortium/ThreePhaseGFM_C2000)).
* **Passive Filtering:** Integrated L-C-L filter stages ($L_f, C_f, L_g$) optimized for grid-interactive operation and harmonic suppression. 

### Interoperability & Grid-Forming Control
* **Heterogeneous Control Integration:** Demonstrated stable parallel operation of multiple inverters using a mix of **Dispatchable Virtual Oscillator Control (dVOC)**, **Droop**, and **Virtual Synchronous Machine (VSM)** controllers.
* **Decentralized Synchronization:** Verified autonomous frequency and phase synchronization at the Point of Common Coupling (PCC) without the need for inter-inverter communication.
* **Dynamic Response Validation:** Experimental results confirm high-fidelity tracking of three-phase currents and voltages, maintaining load balance even during sudden grid transients or setpoint changes.

![Grid-Forming Interoperability Results](/assets/images/HW_3phinv.png)
*Figure 6: Experimental waveforms showing the interoperability of VSM, Droop, and dVOC controllers on a common grid.*
