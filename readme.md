# AUV Hydrography
Hydrography involves the measurement and description of the physical features of oceans, seas, coastal areas, lakes, and rivers, as well as the prediction of their change over time, primarily for safety, navigation, and marine operations.

Autonomous Underwater Vehicles (AUVs) are particularly valuable in hydrography due to their unique capabilities and advantages over traditional methods. Here are several key aspects that make AUVs special in relation to hydrography:

1. Autonomous Operation
Unmanned and Autonomous: AUVs can operate without human intervention, navigating and conducting surveys autonomously. This capability is crucial for exploring hazardous or difficult-to-reach underwater environments where human presence is risky or impractical.

2. High Precision and Accuracy
Advanced Sensors: Equipped with state-of-the-art sensors, including sonar, cameras, and environmental sensors, AUVs can capture high-resolution and precise data about underwater topography, features, and conditions.
Consistent Data Quality: AUVs can maintain a consistent speed and trajectory, ensuring uniform data collection, which is vital for accurate mapping and analysis.

3. Flexibility and Adaptability
Variety of Missions: AUVs can be programmed for various hydrographic missions, such as bathymetric mapping, seabed characterization, and environmental monitoring. They can adapt their missions based on real-time data and pre-defined criteria.
Dynamic Environment Adaptation: Advanced algorithms and control systems allow AUVs to adapt to changing underwater conditions, such as currents and obstacles, ensuring continuous and reliable operation.

4. Cost-Effectiveness
Reduced Operational Costs: AUVs reduce the need for manned missions and large support vessels, lowering the overall cost of hydrographic surveys. Their autonomous nature allows for longer deployments with minimal human oversight.

# Papers

## General

[Advancements in the field of autonomous underwater vehicle](https://www.sciencedirect.com/science/article/abs/pii/S0029801819301623)


## AUV Strategies

### Multiple AUVs

[Bearing, elevation, and depth difference passive inverted acoustic navigation for an AUV fleet](https://www.sciencedirect.com/science/article/abs/pii/S0141118724000191)

[Low-cost high-performance seafloor surveying by multiple autonomous underwater vehicles](https://www.sciencedirect.com/science/article/abs/pii/S0141118721002388)


### Avoidance Methods


#### Navigation Strategies of a Cruising AUV for Near-Bottom Survey of a Steep Terrain
https://www.sciencedirect.com/science/article/pii/S2405896316309880


#### Revolutionizing Underwater Navigation: A New Framework for AUV Obstacle Avoidance

In the quest to explore the vast and resource-rich oceans, the deployment of Autonomous Underwater Vehicles (AUVs) has become increasingly vital. These intelligent, unmanned vehicles are designed to replace humans in performing hazardous underwater tasks. A recent study by researchers from Tianjin University has made significant strides in enhancing the obstacle avoidance capabilities of AUVs using advanced reinforcement learning techniques.

**Intelligent Control for Complex Environments**
AUVs are pivotal in deep-sea exploration, capable of navigating autonomously and operating under extreme conditions. The study, led by Shoufu Liu, Chao Ma, and Rongshun Juan, proposes an innovative obstacle avoidance framework that leverages event-triggered reinforcement learning. This approach enables AUVs to effectively navigate through unknown static and dynamic obstacles while ensuring they reach their designated targets.

**Key Components of the Framework**
The research highlights several critical elements of the new framework:

* Environment Perception Model: The model is designed to assess the relative positions of the AUV, obstacles, and targets. It considers the limited detection range of AUVs and the need to handle both static and dynamic obstacles. The framework uses a soft actor-critic (SAC) algorithm with non-policy sampling to enhance decision-making under varying underwater conditions.

* Event-Triggered Mechanisms: To improve performance, two distinct event-triggered mechanisms were developed. These mechanisms tailor the state space and reward functions, ensuring that the AUV maintains a safe distance from obstacles while navigating towards its target. The integration of these mechanisms with the SAC algorithm allows the AUV to respond dynamically to the environment.

* Simulation and Experimentation: The framework was tested using the Gazebo simulation platform. Three sets of experiments were conducted: single obstacle avoidance, multiple obstacle avoidance, and dynamic obstacle avoidance. The results demonstrated that the proposed method could achieve higher rewards and successfully complete tasks, showcasing its robustness in complex underwater environments.

**Reinforcement Learning in AUV Control**
Reinforcement learning (RL) has emerged as a prominent method in machine learning, particularly for tasks involving continuous interaction with dynamic environments. Traditional AUV control methods, such as Proportional Integral Derivative (PID) and Model Predictive Control (MPC), often fall short due to their reliance on predefined parameters and accurate models. In contrast, RL offers a model-free approach, allowing AUVs to learn optimal actions through interaction and feedback from the environment. This adaptability makes RL particularly suited for the unpredictable nature of underwater navigation.

**Challenges and Innovations**
The study addresses several challenges inherent in AUV navigation:

* Dynamic Environment Adaptation: Traditional control methods struggle with the time-varying nature of hydrodynamic coefficients in real ocean settings. The proposed RL framework adapts to these changes, optimizing strategies through continuous learning.

* Obstacle Avoidance: Ensuring the safety of AUVs while navigating through unknown and dynamic obstacles is crucial. The event-triggered mechanisms and SAC algorithm work in tandem to enhance obstacle detection and avoidance, significantly improving the AUV's operational efficiency and safety.

**Future Prospects**
The integration of intelligent control algorithms into AUVs marks a significant leap forward in underwater exploration technology. This study not only demonstrates the feasibility of using advanced RL techniques for AUV navigation but also sets the stage for future research in autonomous marine systems. As ocean exploration continues to expand, the deployment of smarter, more adaptable AUVs will be essential in unlocking the mysteries of the deep sea and harnessing its resources for the benefit of humanity.

https://www.mdpi.com/2079-9292/13/11/2030


## Novel Positioning Methods
### Polarisation
#### Innovative Advances in Underwater Geolocalization with AI: Transforming Navigation Below the Surface

In a groundbreaking study published in Optics Express, researchers from the University of Illinois at Urbana-Champaign have unveiled a novel approach to underwater geolocalization, harnessing the power of advanced deep neural networks (DNNs) and polarization-based imaging. This innovative method addresses the long-standing challenge of accurately locating unmanned autonomous vehicles (AUVs) in underwater environments where GPS signals are ineffective.

**The Challenge of Underwater Navigation**

Traditionally, underwater navigation has relied on acoustic, inertial, and visual-based localization methods, each with its own limitations. Acoustic localization depends on pre-deployed base stations, limiting its spatial scale. Inertial localization suffers from error accumulation over time, leading to significant deviations. Visual-based localization, which relies on visible landmarks, is constrained in offshore scenarios. These limitations have driven the search for more reliable methods to ensure the success of underwater explorations and research.

**Polarization-Based Geolocalization: A Natural Inspiration**

Drawing inspiration from the natural world, where animals use sky polarization patterns for navigation, the research team focused on polarization-based underwater geolocalization. This approach leverages the unique patterns of sunlight polarization underwater to determine the position of AUVs. The process involves capturing sky polarization patterns with a polarization camera and estimating the sun's location (azimuth and elevation). From these sun locations, the system infers the geolocation (latitude and longitude) of the camera.

**Overcoming Previous Limitations**

Earlier methods, such as the physics-based parametric approach, faced challenges in accurately modeling sunlight propagation in turbid waters or under low sun elevation conditions. These methods also struggled with environmental noise and were not robust in real-world scenarios. The initial deep neural network (DNN) approach improved on these issues by utilizing an RI-ResNet backbone for single-frame sun localization and a recurrent denoising module (RDM) for modeling the sun's trajectory. However, this approach still faced significant performance drops in cross-site tasks, where training and testing data come from different geographic sites and seasons.

**Introducing the Sectoral Transformer**

To address these challenges, the researchers introduced a next-generation DNN model incorporating a Sectoral Transformer (SecTran) and an unscented Kalman filter (UKF). The SecTran, inspired by Transformer architectures used in natural language processing, enhances rotation invariance and temporal modeling. By dividing images into sectoral patches and applying masked image modeling (MIM) during training, the SecTran improves the model's robustness against unseen and noisy inputs.

**Impressive Results and Future Implications**

Extensive experiments and evaluations demonstrated that the new approach significantly outperforms traditional methods. The SecTran-based model showed a 28% improvement in cross-site geolocalization accuracy on average, with some tasks seeing up to a 60% boost. Additionally, the training and inference times were dramatically reduced, making the system more efficient and practical for real-world applications.

This research marks a significant step forward in developing reliable underwater geolocalization systems, potentially revolutionizing the way AUVs navigate and conduct missions in challenging underwater environments. The combination of advanced DNN methodologies and innovative use of polarization-based imaging opens new possibilities for exploration and research in previously inaccessible underwater realms.

https://opg.optica.org/oe/fulltext.cfm?uri=oe-32-12-20706&id=551049

# Analysis
The studies highlight significant advancements in AUV navigation and positioning:

Reinforcement Learning for AUV Navigation: By employing reinforcement learning, particularly the SAC algorithm, the proposed frameworks significantly improve AUVs' ability to navigate complex underwater environments. This model-free approach allows for dynamic adaptation, crucial for real-world applications.

Polarization-Based Geolocalization: The novel use of polarization patterns combined with advanced DNNs addresses traditional limitations in underwater navigation. The introduction of the Sectoral Transformer improves robustness and accuracy, paving the way for more reliable underwater geolocalization.

# Future Implications
The integration of these advanced technologies and methodologies into AUV systems represents a leap forward in underwater exploration. Smarter AUVs with enhanced navigation and positioning capabilities will be essential for deep-sea exploration, resource extraction, and scientific research, contributing to a better understanding and utilization of marine environments.

# Glossary

BEDD - Bearing, elevation and depth differece. 
piSSBL - Passive inverted super short baseline. 
