---
layout: page
title: Research Projects
---

## Isolated DC-DC Topologies (QAB)
[cite_start]During my research at the **University of Texas at Austin** and **University of Washington**, I successfully implemented a series connection of a novel isolated dc-dc topology: the Quadruple Active Bridge (QAB) converter[cite: 22, 23, 28]. [cite_start]This system was designed to support medium-voltage grids from PV sources[cite: 28].

### Performance & Experimental Results
[cite_start]Each module achieved a **96.5% efficiency** for rated conditions of 250 V dc input and 2 kW peak PV power[cite: 29].

![AC and DC Performance](/assets/images/AcandDC.png)
*Figure 1: Experimental waveforms showing AC and DC side performance of the QAB converter.*

### System Architecture
[cite_start]I developed a hierarchy of fully functional MPPT, dc-link, interleaving, and grid-forming ac-side controls[cite: 30].

![System Diagram](/assets/images/System_diagram.png)
*Figure 2: Control architecture and system-level diagram of the modular converter system.*

---

## Grid-Forming Inverters & Fault Ride-Through
[cite_start]At the **Indian Institute of Science (IISc)**, I developed a fault ride-through scheme for grid-forming micro-inverters to make them resilient to dead-short faults[cite: 32, 35].

### Frequency and Stability Analysis
[cite_start]Using an 1 kVA back-to-back hardware setup, I implemented a modified inner current-outer voltage architecture using impedance emulation[cite: 36].

![Frequency Excursion Analysis](/assets/images/FrequencyExcursion.png)
*Figure 3: Frequency excursion analysis demonstrating system stability during grid transients.*

---

## Experimental Hardware Setup
[cite_start]My research involves extensive hardware-in-the-loop (HIL) testing and physical prototype validation using tools like **MATLAB**, **PSCAD**, and **TI C2000 microcontrollers**[cite: 7, 11, 13].

![Hardware Setup](/assets/images/NewsetupPic.png)
*Figure 4: Laboratory testbench including the modular converter stacks and real-time control interface.*
