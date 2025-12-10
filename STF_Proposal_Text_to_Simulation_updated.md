## 1. PROPOSAL TITLE

**LLM-Enhanced Smart Mobility Simulation Platform for Assessing Congestion Impacts of Ride-Hailing Policies in Hong Kong**

---

## 2. OBJECTIVES

This research project aims to develop an innovative Large Language Model (LLM)-based framework for intelligent traffic simulation in Hong Kong. The proposed system will democratize access to advanced traffic simulation tools by enabling users to generate, customize, and analyze complex urban mobility scenarios by interacting with fine-tuned LLMs, allowing users without high-level traffic simulation expertise to evaluate future traffic policies, development programs, or interventions and their impacts; ultimately reducing congestion, controlling traffic-related emissions, improving road network efficiency, and advancing driving safety in Hong Kong. A special focus is placed on **assessing congestion impacts of ride-hailing policies (e.g., licensing regime, vehicle caps, fare rules, data-sharing requirements to support evidence-based implementation.

---

## 3. RESEARCH CONTENTS

### 3.1 Multi-Source Traffic Data Integration and Intelligent Processing

We will establish a multi-source data fusion framework to integrate heterogeneous traffic data streams including video surveillance feeds (data.gov.hk),  (3d.map.gov.hk), road network data (www.td.gov.hk, www.openstreetmap.org), and textual traffic incident reports (data.gov.hk). Ride-hailing–related sources (platform trip logs where accessible, public consultation papers, licensing parameters, fare rules) will be incorporated to capture supply–demand dynamics that drive congestion. The framework could enable automated data preprocessing pipelines to extract critical traffic parameters such as flow rates, vehicle speeds, density distributions, incident locations, and temporal patterns, converting them into both structured formats (e.g., time-series matrices, spatial networks) and natural language descriptions that LLMs can comprehend and process.

The data fusion module will implement advanced anomaly detection algorithms leveraging LLM's contextual reasoning abilities to automatically identify irregular traffic patterns such as sudden congestion, accidents, special events, or infrastructure failures. The system will maintain a continuously updated digital representation of Hong Kong's transportation network, integrating data from transport department's traffic detectors, CCTV networks, public transport information, parking occupancy sensors, and ride-hailing operational signals (surge events, supply gaps). This multi-modal integration ensures scenarios reflect congestion responses to ride-hailing policy changes.

### 3.2 Multi-Agent Text-to-Simulation System Architecture and Platform Integration

This part will develop a scalable multi-agent text-to-simulation system that seamlessly integrates with established microscopic traffic simulation platforms such as SUMO (Simulation of Urban MObility). The system will feature a modular architecture with API integration layers, including Planner Agent (central orchestrator), Tool Layer (simulation utilities), and State Management (workflow coordination), to enable bidirectional communication between traffic simulation platforms and users. The Planner Agent, powered by state-of-the-art LLMs, will serve as an intelligent interface that translates natural language user inputs into structured simulation commands, automatically invoking appropriate tools in the correct sequence to generate complete traffic scenarios from high-level descriptions such as "simulate morning peak hour traffic in Central with 20% increase in ride-hailing vehicles" and "evaluate congestion if 10,000 licensed ride-hailing vehicles operate under a 5% fare cap."

### 3.3 Domain-Specific LLM Fine-Tuning for Traffic Simulation Modules

This part will develop specialized fine-tuning strategies to adapt LLMs for diverse traffic simulation generation tasks, recognizing that different simulation components require distinct reasoning capabilities and domain knowledge. The fine-tuning program will target five critical simulation generation modules, each augmented to capture ride-hailing congestion effects: 

(1) Road Network Generation - training LLMs to interpret OpenStreetMap data for Hong Kong, handle complex junction types, and generate network files with designated pick-up/drop-off (PUDO) areas and curb management rules relevant to ride-hailing. (2) Geographic Feature Generation - enabling LLMs to identify POIs/AOIs that drive ride-hailing hotspots (CBDs, rail stations, airports) to shape demand. (3) Travel Demand Generation - producing OD matrices and trip chains reflecting Hong Kong behavior plus ride-hailing demand elasticity under legalization, fare caps, and vehicle permit limits. (4) Traffic Assignment and Route Planning - generating route choice sets that include platform dispatch/rebalancing behaviors and tunnel/bridge constraints to study congestion redistribution. (5) Traffic Signal Control and Priority - designing intersection control and transit priority plans that mitigate added ride-hailing flows and evaluate time-of-day congestion relief.

### 3.4 Ride-Hailing Driver & Passenger Behavioral Survey

To construct the simulation platform that accurately reflects the impact of ride-hailing operations on urban traffic congestion, this project designed a questionnaire targeting both ride-hailing drivers and passengers. The primary objective of the questionnaire is to transform individual behavioral intentions and decision-making patterns into quantifiable input parameters for the simulation model. These parameters are categorized into two main types: the operational behavior of drivers on the supply side and the travel profiles of passengers on the demand side.

On the supply side, the driver survey focuses on five key dimensions: (1) response to ride-hailing legalization, including willingness to become a driver after legalization and current occupation, to estimate the increase in driver numbers post-legalization; (2) employment type (full-time or part-time) and current occupation (for part-time drivers only), to determine drivers' available service time windows; (3) operational elasticity, measured through scenario-based questions regarding temporal elasticity (service hours), spatial elasticity (operating areas), and income elasticity (service duration under varying income levels); (4) request matching and route choice preferences, encompassing preferences for long versus short trips, behavior in no-order states (cruising or waiting), and route selection strategies under congestion; and (5) decision-making mechanisms, primarily examining sensitivity to dynamic pricing, criteria for order rejection, and changes in work frequency under adverse external conditions. On the demand side, the passenger survey primarily covers: (1) trip characteristics, including trip purpose, usage frequency, and typical origin-destination types; (2) service selection preferences, such as temporal distribution of ride requests, tolerance for waiting time, and price sensitivity; and (3) alternative travel modes adopted when ride-hailing is unavailable or not the preferred option.

### 3.5 Simulation Validation and Evaluation

To ensure reliability and accuracy, we will implement a comprehensive validation process calibrating simulation outputs against real-world Hong Kong traffic data. Quantitative validation will compare simulated and observed metrics (travel times, speeds, density, congestion patterns). Qualitative validation through expert assessments will ensure behavioral realism and alignment with Hong Kong's unique characteristics. In the application of the simulation system, we will evaluate impacts of potential traffic policy interventions, future development programs, and emerging mobility services. Policy scenarios include congestion pricing, dynamic signal optimization, road space reallocation, and incident management. Development assessments will examine major infrastructure projects and their effects on regional traffic distribution. Emerging mobility evaluations will cover autonomous vehicles, ride-hailing expansion, and micro-mobility integration. For each scenario, the system will generate comparative metrics (travel time, density, VKT, emissions, accessibility) to conduct rapid iterative policy testing, supporting evidence-based transportation planning for more sustainable and efficient urban mobility in Hong Kong. 


1. PROPOSAL TITLE
LLM-Enhanced Smart Mobility Simulation Platform for Assessing Congestion Impacts of Ride-Hailing Policies in Hong Kong
 
2. OBJECTIVES
This research project aims to develop an innovative Large Language Model (LLM)-based framework for intelligent traffic simulation in Hong Kong. The proposed system will democratize access to advanced traffic simulation tools by enabling users to generate, customize, and analyze complex urban mobility scenarios by interacting with fine-tuned LLMs, allowing users without high-level traffic simulation expertise to evaluate future traffic policies, development programs, or interventions and their impacts; ultimately reducing congestion, controlling traffic-related emissions, improving road network efficiency, and advancing driving safety in Hong Kong. A special focus is placed on assessing congestion impacts of ride-hailing policies (e.g., licensing regime, vehicle caps, fare rules, data-sharing requirements to support evidence-based implementation.

3. RESEARCH CONTENTS
3.1 Multi-Source Traffic Data Integration and Intelligent Processing
We will establish a multi-source data fusion framework to integrate heterogeneous traffic data streams including video surveillance feeds (data.gov.hk), LiDAR point clouds (3d.map.gov.hk), road network data (www.td.gov.hk, www.openstreetmap.org), and textual traffic incident reports (data.gov.hk). Ride-hailing–related sources (platform trip logs where accessible, public consultation papers, licensing parameters, fare rules) will be incorporated to capture supply–demand dynamics that drive congestion. The framework could enable automated data preprocessing pipelines to extract critical traffic parameters such as flow rates, vehicle speeds, density distributions, incident locations, and temporal patterns, converting them into both structured formats (e.g., time-series matrices, spatial networks) and natural language descriptions that LLMs can comprehend and process.

The data fusion module will implement advanced anomaly detection algorithms leveraging LLM's contextual reasoning abilities to automatically identify irregular traffic patterns such as sudden congestion, accidents, special events, or infrastructure failures. The system will maintain a continuously updated digital representation of Hong Kong's transportation network, integrating data from transport department's traffic detectors, CCTV networks, public transport information, parking occupancy sensors, and ride-hailing operational signals (surge events, supply gaps). This multi-modal integration ensures scenarios reflect congestion responses to ride-hailing policy changes.

3.2 Multi-Agent Text-to-Simulation System Architecture and Platform Integration
This part will develop a scalable multi-agent text-to-simulation system that seamlessly integrates with established microscopic traffic simulation platforms such as SUMO (Simulation of Urban MObility). The system will feature a modular architecture with API integration layers, including Planner Agent (central orchestrator), Tool Layer (simulation utilities), and State Management (workflow coordination), to enable bidirectional communication between traffic simulation platforms and users. The Planner Agent, powered by state-of-the-art LLMs, will serve as an intelligent interface that translates natural language user inputs into structured simulation commands, automatically invoking appropriate tools in the correct sequence to generate complete traffic scenarios from high-level descriptions such as "simulate morning peak hour traffic in Central with 20% increase in ride-hailing vehicles" and "evaluate congestion if 10,000 licensed ride-hailing vehicles operate under a 5% fare cap."

3.3 Domain-Specific LLM Fine-Tuning for Traffic Simulation Modules
This part will develop specialized fine-tuning strategies to adapt LLMs for diverse traffic simulation generation tasks, recognizing that different simulation components require distinct reasoning capabilities and domain knowledge. The fine-tuning program will target five critical simulation generation modules, each augmented to capture ride-hailing congestion effects: 

(1) Road Network Generation - training LLMs to interpret OpenStreetMap data for Hong Kong, handle complex junction types, and generate network files with designated pick-up/drop-off areas and curb management rules relevant to ride-hailing. (2) Geographic Feature Generation - enabling LLMs to identify POIs/AOIs that drive ride-hailing hotspots (CBDs, rail stations, airports) to shape demand. (3) Travel Demand Generation - producing OD matrices and trip chains reflecting Hong Kong behavior plus ride-hailing demand elasticity under legalization, fare caps, and vehicle permit limits. (4) Traffic Assignment and Route Planning - generating route choice sets that include platform dispatch/rebalancing behaviors and tunnel/bridge constraints to study congestion redistribution. (5) Traffic Signal Control and Priority - designing intersection control and transit priority plans that mitigate added ride-hailing flows and evaluate time-of-day congestion relief.
3.4 Ride-Hailing Driver & Passenger Behavioral Survey
Cannot get the ride-hailing stops, on the Amap, seems like we can order vehicles anywhere. But the locations for taxi stands are available. 

网约车合法化对交通拥堵的影响遵循以下传导机制：网约车司机进入市场后，其行为会影响司机与乘客的出行决策（如出行方式选择、出行频率等），进而改变交通流量与道路车速。为避免仿真平台出现以下问题：1）偶然再现真实拥堵模式，却错误表征行为转变机制，导致政策情景模拟失效；2）无法辨识车速变化是否源于网约车合法化后大量司机涌入市场，我们设计了一个从行为转变监测到拥堵变化评估的双重验证框架，以检验仿真模型的有效性。该框架中，行为转变监测模块用于观察网约车合法化后司机行为是否加剧拥堵，监测指标包括在线时长、空驶距离和绕行距离的变化；拥堵变化评估模块则用于检测路段车速在政策实施后的变化。通过对比仿真输出与实际情况（出行行为变化及路段车速），我们可评估仿真平台的可靠性，并对模型参数进行校准与优化。在此基础上，本研究进一步推演网约车合法化后，不同规模的网约车司机进入市场对城市交通拥堵的影响。

为校准仿真平台并提供独立验证依据，我们在网约车合法化前后分别开展了两轮数据收集工作：一轮在政策实施前（事前），一轮在政策实施后（事后）。数据主要包括网约车司机与乘客的出行行为问卷，以及重点观测区域的路段车速数据（可结合车流量、出租车及网约车轨迹数据）。事前问卷用于获取仿真平台所需的决策函数（如乘客出行模式选择、拼车意愿、司机接单概率、巡游策略等）及个体特征分布参数（如等待时间容忍度、价格敏感度、激励响应时间、工作弹性等）。事后问卷则主要用于验证仿真结果的有效性（如能否准确估计乘客等待时间、出行模式转变、司机空驶率、绕行距离等），并据此对仿真参数进行校准与约束。此外，政策实施前收集的路段车速数据将作为基础输入参数导入仿真平台，而政策实施后收集的路段车速数据则用于检验仿真平台在拥堵估计方面的准确性。

To construct the simulation platform that accurately reflects the impact of ride-hailing operations on urban traffic congestion, this project designed a questionnaire targeting both ride-hailing drivers and passengers. The primary objective of the questionnaire is to transform individual behavioral intentions and decision-making patterns into quantifiable input parameters for the simulation model. These parameters are categorized into two main types: the operational behavior of drivers on the supply side and the travel profiles of passengers on the demand side.
On the supply side, the driver survey focuses on five key dimensions: (1) response to ride-hailing legalization, including willingness to become a driver after legalization and current occupation, to estimate the increase in driver numbers post-legalization; (2) employment type (full-time or part-time) and current occupation (for part-time drivers only), to determine drivers' available service time windows; (3) operational elasticity, measured through scenario-based questions regarding temporal elasticity (service hours), spatial elasticity (operating areas), and income elasticity (service duration under varying income levels); (4) request matching and route choice preferences, encompassing preferences for long versus short trips, behavior in no-order states (cruising or waiting), and route selection strategies under congestion; (5) decision-making mechanisms, primarily examining sensitivity to dynamic pricing, criteria for order rejection, and changes in work frequency under adverse external conditions, and (6) driver’s trips records: including pick-up and drop-off points, time, distance, price, and driving route (optional, used to record detours).. On the demand side, the passenger survey primarily covers: (1) trip characteristics, including trip purpose, usage frequency, and typical origin-destination types; (2) service selection preferences, such as temporal distribution of ride requests, tolerance for waiting time, and price sensitivity; (3) alternative travel modes adopted when ride-hailing is unavailable or not the preferred option; and (4) travel records, including the travel mode, travel origins and destinations, travel time, and prices. 

下表展示了如何讲问卷收集的数据转为仿真平台可输入的参数
Parameter 	描述	Calculation 
乘客端
等待时间容忍度	乘客在被动等待（等待配对/叫车）时愿意接受的最大等待时间（分钟
等待时间分布
价格敏感度	乘客对价格变化的响应	出行行为离散选择模型计算敏感度分布
U_im=β_price 〖Price〗_im+∑▒〖β_others Others〗+γX_i+ϵ_im
Normal(β_price, S.D. (β_price))
是否参与拼车决策函数	该乘客是否愿意接受拼车	p_share=(∑▒N_share )/N
p_share=f(x)
司机端
司机空驶里程比	司机在接单前的空驶里程占其营运总里程的比例	Deadheading=(∑▒〖Deadheading miles〗)/(∑▒〖(Deadheading miles+trip miles)〗)
Normal(mean, S.D)
无单时司机的巡游模式选择函数	司机在无单/待命时如何选择空间移动（驻点、巡游、回家待命等）	Pr(mode | influencing factors)
接单接受概率函数	司机在面对某次派单/请求时接受的概率	Pr(accept =1 | influencing factors)
其他，后续添加		

仿真平台输出和真实观测结果的主要比较指标
行为层面：
乘客等待时间分布（分布函数/空间分布）
乘客N次出行的模式占比
乘客出行时间分布
司机订单接受概率（接受/拒单比例）
司机空驶里程比（空驶时间 / 营运时间或空驶里程比例）
司机平均每日上线小时数
各个区域对的出行量占比（是否需要）

拥堵层面：
路段平均车速（km/h）

3.5 Simulation Validation and Evaluation
To ensure reliability and accuracy, we will implement a comprehensive validation process calibrating simulation outputs against real-world Hong Kong traffic data. Quantitative validation will compare simulated and observed metrics (travel times, speeds, density, congestion patterns). Qualitative validation through expert assessments will ensure behavioral realism and alignment with Hong Kongs unique characteristics. In the application of the simulation system, we will evaluate impacts of potential traffic policy interventions, future development programs, and emerging mobility services. Policy scenarios include congestion pricing, dynamic signal optimization, road space reallocation, and incident management. Development assessments will examine major infrastructure projects and their effects on regional traffic distribution. Emerging mobility evaluations will cover autonomous vehicles, ride-hailing expansion, and micro-mobility integration. For each scenario, the system will generate comparative metrics (travel time, density, emissions, accessibility) to conduct rapid iterative policy testing, supporting evidence-based transportation planning for more sustainable and efficient urban mobility in Hong Kong.
