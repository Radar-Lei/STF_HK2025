## 1. PROPOSAL TITLE

**Text to Simulation: Large Language Model for AI-based Urban Mobility Simulation in Hong Kong**

---

## 2. OBJECTIVES

This research project aims to develop an innovative Large Language Model (LLM)-based framework for intelligent traffic simulation in Hong Kong. The proposed system will democratize access to advanced traffic simulation tools by enabling users to generate, customize, and analyze complex urban mobility scenarios by interacting with fine-tuned LLMs, allowing users without high-level traffic simulation expertise to evaluate future traffic policies, development programs, or interventions and their impacts; ultimately reducing congestion, controlling traffic-related emissions, improving road network efficiency, and advancing driving safety in Hong Kong.

### 2.1 Primary Objectives

**Objective 1: Develop an LLM-Integrated Traffic Simulation Framework**
Create a novel AI-powered system that integrates state-of-the-art Large Language Models with microscopic traffic simulation platforms, enabling natural language scenario generation that lowers the specialized simulation expertise and setup barriers required for generating diverse traffic simulation scenarios.

**Objective 2: Enhance Accessibility and User-Friendliness for Hong Kong Transportation Planning**
Lower the barrier to entry for transportation planners, policymakers, and researchers in Hong Kong by delivering an interface that supports multi-language and real-time conversational scenario edits, enabling rapid iterative policy testing without prior simulation expertise.

**Objective 3: Improve Traffic Management and Decision-Making Capabilities**
Fuse multi-source data such as video, LiDAR, GPS traces, and textual traffic reports into the simulator while equipping AI agents to autonomously generate, optimize, and flag anomalies in traffic scenarios, enabling robust evaluation of traffic or policy-related interventions such as congestion pricing, road closures, signal plans, and emerging mobility services such as autonomous vehicles and ride-sharing.


---

## 3. RESEARCH CONTENTS

### 3.1 Multi-Source Traffic Data Integration and Intelligent Processing

We will establish a multi-source data fusion framework to integrate heterogeneous traffic data streams including video surveillance feeds, LiDAR point clouds, GPS trajectory data, and textual traffic incident reports from Hong Kong's existing ITS infrastructure. The framework could enable automated data preprocessing pipelines to extract critical traffic parameters such as flow rates, vehicle speeds, density distributions, incident locations, and temporal patterns, converting them into both structured formats (e.g., time-series matrices, spatial networks) and natural language descriptions that LLMs can comprehend and process.

The data fusion module will implement advanced anomaly detection algorithms leveraging LLM's contextual reasoning abilities to automatically identify irregular traffic patterns such as sudden congestion, accidents, special events, or infrastructure failures. The system will maintain a continuously updated digital representation of Hong Kong's transportation network, integrating data from transport department's traffic detectors, CCTV networks, public transport information, parking occupancy sensors. This multi-modal data integration will provide a high-fidelity foundation for the LLM-driven simulation system, ensuring that generated simulation scenarios accurately reflect real-world Hong Kong traffic characteristics including the unique geographical features and high-density mixed traffic patterns typical of the city.

### 3.2 Multi-Agent Text-to-Simulation System Architecture and Platform Integration

This part will develop a scalable multi-agent text-to-simulation system that seamlessly integrates with established microscopic traffic simulation platforms such as SUMO (Simulation of Urban MObility). The system will feature a modular architecture comprising a Planner Agent (central orchestrator), Tool Layer (simulation utilities), and State Management (workflow coordination). The Planner Agent, powered by state-of-the-art LLMs, will serve as an intelligent interface that translates natural language user inputs into structured simulation commands, automatically invoking appropriate tools in the correct sequence to generate complete traffic scenarios from high-level descriptions such as "simulate morning peak hour traffic in Central with 20% increase in ride-hailing vehicles."

The system will implement comprehensive API integration layers that enable bidirectional communication with traffic simulation platforms, handling data format conversions (XML configuration files, route definitions, network topology), parameter passing, simulation execution, and results retrieval. The architecture will support three operational modes: (1) Fully automated pipeline where LLM agents autonomously construct scenarios from natural language to execution; (2) Interactive mode enabling iterative refinement through conversational exchanges; and (3) Batch processing mode for policy comparison experiments. Critical technical components include a Translation Engine that converts LLM natural language outputs into simulation-ready formats, a Query Builder that constructs structured prompts from user intentions, and a Verification Module that validates generated scenarios for feasibility and consistency before execution, ensuring reliable simulation results for Hong Kong transportation planning applications.

### 3.3 Domain-Specific LLM Fine-Tuning for Traffic Simulation Components

This part will develop specialized fine-tuning strategies to adapt LLMs for diverse traffic simulation generation tasks, recognizing that different simulation components require distinct reasoning capabilities and domain knowledge. The fine-tuning program will target five critical simulation generation modules: (1) Road Network Generation - training LLMs to accurately interpret OpenStreetMap data for Hong Kong, handle complex junction types (roundabouts, slip roads, multi-level interchanges), and generate valid network files with appropriate lane configurations and connectivity; (2) Geographic Feature Generation - enabling LLMs to identify and instantiate Points of Interest (POI) such as shopping centers, offices, schools, and Areas of Interest (AOI) including residential zones, business districts, and industrial areas, serving as the origin and destination (OD) points of trips and ensuring realistic spatial activity distributions; (3) Travel Demand Generation - fine-tuning agents to produce human-like origin-destination matrices, daily activity patterns, and trip chains that reflect Hong Kong's unique travel behavior characteristics derived from household travel surveys and mobile signaling data.

The fine-tuning approach will employ a combination of techniques including supervised fine-tuning on domain-specific datasets (e.g., historical traffic scenarios, expert-designed simulation configurations), Low-Rank Adaptation (LoRA) for parameter-efficient training, and Retrieval-Augmented Generation (RAG) for incorporating traffic engineering knowledge bases. For route planning and traffic assignment, LLMs will be trained to apply established principles (e.g., user equilibrium, stochastic route choice) while adapting to real-time conditions. Critically, for signal intersection timing optimization, the system will fine-tune LLMs to validate and generate signal control schemes based on Webster's method, green wave coordination principles, and adaptive signal control logic, ensuring that generated timing plans are both theoretically sound and practically implementable. Each specialized LLM will undergo rigorous validation against ground-truth scenarios and expert-designed benchmarks to ensure high fidelity simulation outputs for Hong Kong's transportation simulation applications.

### 3.4 Policy Evaluation for Hong Kong's Ride-Hailing Service Regulation

This part will use the established LLM-driven simulation framework to evaluate the impact of various potential/future traffic policy interventions, strateges, and new development programs. As Hong Kong prepares to introduce a licensing regime for ride-hailing platforms, vehicles, and drivers, critical questions remain regarding the optimal number of ride-hailing vehicle permits (with proposals ranging from 10,000+ vehicles), their impact on existing taxi operations, and effects on overall traffic conditions. The simulation system will enable rapid scenario generation to evaluate multiple permit quota configurations and their potential impacts on network-wide traffic flow, congestion levels, travel times, emissions, and public transport ridership across different Hong Kong districts during peak and off-peak periods. We could also evaluate the performance of potential interventions for ride-hailing services using the simulation system. For example, we could evaluate the impact of dynamic congestion pricing in core business districts (Central, Admiralty, Wan Chai), designated ride-hailing pickup/drop-off zones to reduce cruising behavior, preferential treatment for electric ride-hailing vehicles, integration with public transport hubs, and time-of-day operational restrictions.
