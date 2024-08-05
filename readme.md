# Hydrography


# Papers

https://www.sciencedirect.com/science/article/abs/pii/S0029801819301623





## Novel Positioning Methods
### Polarisation
Title: Innovative Advances in Underwater Geolocalization with AI: Transforming Navigation Below the Surface

In a groundbreaking study published in Optics Express, researchers from the University of Illinois at Urbana-Champaign have unveiled a novel approach to underwater geolocalization, harnessing the power of advanced deep neural networks (DNNs) and polarization-based imaging. This innovative method addresses the long-standing challenge of accurately locating unmanned autonomous vehicles (AUVs) in underwater environments where GPS signals are ineffective.

The Challenge of Underwater Navigation

Traditionally, underwater navigation has relied on acoustic, inertial, and visual-based localization methods, each with its own limitations. Acoustic localization depends on pre-deployed base stations, limiting its spatial scale. Inertial localization suffers from error accumulation over time, leading to significant deviations. Visual-based localization, which relies on visible landmarks, is constrained in offshore scenarios. These limitations have driven the search for more reliable methods to ensure the success of underwater explorations and research.

Polarization-Based Geolocalization: A Natural Inspiration

Drawing inspiration from the natural world, where animals use sky polarization patterns for navigation, the research team focused on polarization-based underwater geolocalization. This approach leverages the unique patterns of sunlight polarization underwater to determine the position of AUVs. The process involves capturing sky polarization patterns with a polarization camera and estimating the sun's location (azimuth and elevation). From these sun locations, the system infers the geolocation (latitude and longitude) of the camera.

Overcoming Previous Limitations

Earlier methods, such as the physics-based parametric approach, faced challenges in accurately modeling sunlight propagation in turbid waters or under low sun elevation conditions. These methods also struggled with environmental noise and were not robust in real-world scenarios. The initial deep neural network (DNN) approach improved on these issues by utilizing an RI-ResNet backbone for single-frame sun localization and a recurrent denoising module (RDM) for modeling the sun's trajectory. However, this approach still faced significant performance drops in cross-site tasks, where training and testing data come from different geographic sites and seasons.

Introducing the Sectoral Transformer

To address these challenges, the researchers introduced a next-generation DNN model incorporating a Sectoral Transformer (SecTran) and an unscented Kalman filter (UKF). The SecTran, inspired by Transformer architectures used in natural language processing, enhances rotation invariance and temporal modeling. By dividing images into sectoral patches and applying masked image modeling (MIM) during training, the SecTran improves the model's robustness against unseen and noisy inputs.

Impressive Results and Future Implications

Extensive experiments and evaluations demonstrated that the new approach significantly outperforms traditional methods. The SecTran-based model showed a 28% improvement in cross-site geolocalization accuracy on average, with some tasks seeing up to a 60% boost. Additionally, the training and inference times were dramatically reduced, making the system more efficient and practical for real-world applications.

This research marks a significant step forward in developing reliable underwater geolocalization systems, potentially revolutionizing the way AUVs navigate and conduct missions in challenging underwater environments. The combination of advanced DNN methodologies and innovative use of polarization-based imaging opens new possibilities for exploration and research in previously inaccessible underwater realms.
https://opg.optica.org/oe/fulltext.cfm?uri=oe-32-12-20706&id=551049


