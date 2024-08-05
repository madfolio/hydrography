# Hydrography


# Papers

https://www.sciencedirect.com/science/article/abs/pii/S0029801819301623


## AUV Strategies

### Avoidance Methods
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


