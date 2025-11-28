## 1. PROPOSAL TITLE

**LLM-Enhanced Smart Mobility Simulation Platform for Assessing Congestion Impacts of Ride-Hailing Policies in Hong Kong**

---

## 2. OBJECTIVES

This research project aims to develop an innovative Large Language Model (LLM)-based framework for intelligent traffic simulation in Hong Kong. The proposed system will democratize access to advanced traffic simulation tools by enabling users to generate, customize, and analyze complex urban mobility scenarios by interacting with fine-tuned LLMs, allowing users without high-level traffic simulation expertise to evaluate future traffic policies, development programs, or interventions and their impacts; ultimately reducing congestion, controlling traffic-related emissions, improving road network efficiency, and advancing driving safety in Hong Kong. A special focus is placed on **assessing congestion impacts of ride-hailing policies (e.g., licensing regime, vehicle caps, fare rules, data-sharing requirements to support evidence-based implementation.

---

## 3. RESEARCH CONTENTS

### 3.1 Multi-Source Traffic Data Integration and Intelligent Processing

We will establish a multi-source data fusion framework to integrate heterogeneous traffic data streams including video surveillance feeds (data.gov.hk), LiDAR point clouds (3d.map.gov.hk), road network data (www.td.gov.hk, www.openstreetmap.org), and textual traffic incident reports (data.gov.hk). Ride-hailing–related sources (platform trip logs where accessible, public consultation papers, licensing parameters, fare rules) will be incorporated to capture supply–demand dynamics that drive congestion. The framework could enable automated data preprocessing pipelines to extract critical traffic parameters such as flow rates, vehicle speeds, density distributions, incident locations, and temporal patterns, converting them into both structured formats (e.g., time-series matrices, spatial networks) and natural language descriptions that LLMs can comprehend and process.

The data fusion module will implement advanced anomaly detection algorithms leveraging LLM's contextual reasoning abilities to automatically identify irregular traffic patterns such as sudden congestion, accidents, special events, or infrastructure failures. The system will maintain a continuously updated digital representation of Hong Kong's transportation network, integrating data from transport department's traffic detectors, CCTV networks, public transport information, parking occupancy sensors, and ride-hailing operational signals (surge events, supply gaps). This multi-modal integration ensures scenarios reflect congestion responses to ride-hailing policy changes.

### 3.2 Multi-Agent Text-to-Simulation System Architecture and Platform Integration

This part will develop a scalable multi-agent text-to-simulation system that seamlessly integrates with established microscopic traffic simulation platforms such as SUMO (Simulation of Urban MObility). The system will feature a modular architecture with API integration layers, including Planner Agent (central orchestrator), Tool Layer (simulation utilities), and State Management (workflow coordination), to enable bidirectional communication between traffic simulation platforms and users. The Planner Agent, powered by state-of-the-art LLMs, will serve as an intelligent interface that translates natural language user inputs into structured simulation commands, automatically invoking appropriate tools in the correct sequence to generate complete traffic scenarios from high-level descriptions such as "simulate morning peak hour traffic in Central with 20% increase in ride-hailing vehicles" and "evaluate congestion if 10,000 licensed ride-hailing vehicles operate under a 5% fare cap."

### 3.3 Domain-Specific LLM Fine-Tuning for Traffic Simulation Modules

This part will develop specialized fine-tuning strategies to adapt LLMs for diverse traffic simulation generation tasks, recognizing that different simulation components require distinct reasoning capabilities and domain knowledge. The fine-tuning program will target five critical simulation generation modules, each augmented to capture ride-hailing congestion effects: 

(1) Road Network Generation - training LLMs to interpret OpenStreetMap data for Hong Kong, handle complex junction types, and generate network files with designated pick-up/drop-off (PUDO) areas and curb management rules relevant to ride-hailing. (2) Geographic Feature Generation - enabling LLMs to identify POIs/AOIs that drive ride-hailing hotspots (CBDs, rail stations, airports) to shape demand. (3) Travel Demand Generation - producing OD matrices and trip chains reflecting Hong Kong behavior plus ride-hailing demand elasticity under legalization, fare caps, and vehicle permit limits. (4) Traffic Assignment and Route Planning - generating route choice sets that include platform dispatch/rebalancing behaviors and tunnel/bridge constraints to study congestion redistribution. (5) Traffic Signal Control and Priority - designing intersection control and transit priority plans that mitigate added ride-hailing flows and evaluate time-of-day congestion relief.

### 3.4 Ride-Hailing Driver & Passenger Behavioral Survey

Embed the project’s questionnaire to translate behavioral intentions into simulation parameters that influence congestion. Supply-side items quantify legalization-induced entry, full/part-time availability, spatial/temporal elasticity, route choice under congestion, and reactions to dynamic pricing—informing driver supply curves and repositioning patterns. Demand-side items capture trip purposes, usage frequency, waiting-time tolerance, price sensitivity, and mode-shift choices when ride-hailing is constrained, enabling congestion-sensitive demand modeling and counterfactuals for policy scenarios. 

### 3.5 Simulation Validation and Evaluation

To ensure reliability and accuracy, we will implement a comprehensive validation process calibrating simulation outputs against real-world Hong Kong traffic data. Quantitative validation will compare simulated and observed metrics (travel times, speeds, density, congestion patterns). Qualitative validation through expert assessments will ensure behavioral realism and alignment with Hong Kong's unique characteristics. In the application of the simulation system, we will evaluate impacts of potential traffic policy interventions, future development programs, and emerging mobility services. Policy scenarios include congestion pricing, dynamic signal optimization, road space reallocation, and incident management. Development assessments will examine major infrastructure projects and their effects on regional traffic distribution. Emerging mobility evaluations will cover autonomous vehicles, ride-hailing expansion, and micro-mobility integration. For each scenario, the system will generate comparative metrics (travel time, density, VKT, emissions, accessibility) to conduct rapid iterative policy testing, supporting evidence-based transportation planning for more sustainable and efficient urban mobility in Hong Kong. 
