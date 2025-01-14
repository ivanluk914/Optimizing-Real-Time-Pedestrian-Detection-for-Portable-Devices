# Optimizing-Real-Time-Pedestrian-Detection-for-Portable-Devices

### Introduction
This repository is part of Team New Bee's efforts for the COMP9444 course at UNSW, focusing on the development and benchmarking of a real-time pedestrian detection system for autonomous vehicles. This project aims to improve the safety and functionality of autonomous navigation systems through advanced computer vision techniques.

### Background
The evolution of autonomous vehicle technology presents significant challenges in detecting pedestrians accurately and swiftly to prevent accidents. This project explores state-of-the-art machine learning models that can provide reliable pedestrian detection even in dynamic environments. By enhancing detection systems, we aim to contribute to safer autonomous driving technologies.

### Project Objectives
- **Model Comparison**: Conduct exhaustive performance analyses of several machine learning models, including Faster R-CNN, SSD, YOLOv5, and YOLOv8, focusing on their efficiency and accuracy in detecting pedestrians in real-time.
- **Model Enhancement**: Optimize the YOLOv8 model to improve detection accuracy while minimizing computational demands, facilitating deployment on devices with limited hardware capabilities.

### Challenges
- **Data Representation**: One of the main challenges was the adaptation of the `MS COCO 2017` dataset to better focus on pedestrian detection. The original 'person' category was too broad, encompassing non-pedestrian figures, which required custom filtering and redefinition.
- **Model Optimization**: Balancing speed and accuracy, especially in low-resource environments, was challenging. Enhancing YOLOv8 involved integrating lightweight architectures without compromising the model’s performance.

### Models Evaluated
- **Faster R-CNN**: Integrates a Region Proposal Network with a Fast R-CNN, known for its accuracy but higher computational cost.
- **SSD (Single Shot MultiBox Detector)**: Utilizes a single neural network for detection, providing a balance between speed and accuracy.
- **YOLOv5**: Stands out for its operational speed and efficiency, making it ideal for real-time applications.
- **Enhanced YOLOv8**: Our project’s flagship model, incorporating GhostNet architecture to reduce complexity and enhance performance.

### Dataset
Utilizing the MS COCO 2017 dataset, we applied modifications to better suit our needs for pedestrian detection. This involved refining the dataset to accurately categorize 'pedestrians' and exclude non-relevant entities.

### Experimental Setup
- **Hardware**: Utilized NVIDIA T4, RTX 2060, and RTX 3090 GPUs to conduct experiments.
- **Software**: Deployed using PyTorch and the Ultralytics YOLOv8 framework, adapted for our enhancements.
- **Evaluation Metrics**: Models were assessed based on Mean Average Precision (mAP), Inference Speed (FPS), and Intersection Over Union (IoU).

### Results
The enhanced YOLOv8 model demonstrated a robust balance between speed and accuracy, showing great promise for real-time pedestrian detection in autonomous vehicle systems.

### Project Report
For a detailed analysis and comprehensive results, refer to the "report.pdf" which is included in this repository. The report provides an in-depth review of the project's methodologies, data handling, and experimental outcomes.

### Installation and Usage
Detailed setup instructions, including environment configuration and model execution, are provided in the notebook.

### Contributing

| Name      | zID |
|-----------|-----|
| Ivan Luk  | z5463348 |
| Zhidi Wei | z5392805 |
| Junhua Liu| z5438356 |
| Qirui Ye  | z5337136 |
| Yi Jiang  | z5432865 |

We encourage contributions to improve the project.

### License
This project is licensed under the Apache-2.0 license. Full details can be found in `LICENSE.md`.

### Acknowledgments
- Special thanks to our course mentors and COMP9444 staff for their continuous support.
- Appreciation to the contributors of the MS COCO dataset and the developers of the machine learning models used.
