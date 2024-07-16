# Traffic-Sign Detection and Classification (Vietnam Dataset)

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository provides a robust solution for detecting and classifying traffic signs within the unique context of Vietnamese roads. It features a custom-built dataset of traffic signs from Vietnam and explores the effectiveness of various object detection models in this specific environment, including their performance under challenging real-world conditions.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Models](#models)
- [Baseline Results](#baseline-results) 
- [Results and Evaluation](#results-and-evaluation)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

Accurately identifying traffic signs is crucial for both human drivers and autonomous vehicles. This project aims to address the challenges of traffic sign detection and classification in Vietnam, where road conditions and sign designs may differ from other regions. We specifically focus on evaluating model robustness under challenging conditions like blur, darkness, and noise.

## Features

- **Custom Vietnamese Traffic Sign Dataset:** A carefully curated collection of traffic sign images captured in various locations across Vietnam.
- **Diverse Model Exploration:**  Implementation and comparison of different object detection models to find the most suitable for Vietnamese traffic signs.
- **Robustness Testing:** Evaluation of models under challenging conditions (e.g., varying lighting, weather, blur) using image transformations.
- **Extensible Framework:** Designed for easy integration with other traffic sign datasets and additional model architectures.

## Dataset

Our dataset is a valuable resource for training and validating object detection models specifically tailored for Vietnamese traffic signs. It includes:

- **Variety:**  Diverse sign types (regulatory, warning, informational).
- **Annotations:**  Precise bounding boxes and class labels for each sign.
- **Real-World Data:** Images captured in different lighting and weather conditions.
- **Challenging Conditions:** Subsets of images with added blur, darkness, and noise.
- **Metadata:** Additional details for in-depth analysis (location, camera angle, etc.).

## Models

We've experimented with a range of object detection models:

- **YOLOv5:** Known for its speed and accuracy.
- **YOLOv8:** An improved version of YOLOv5.
- **Faster R-CNN:** Strong performance on diverse object types.

## Baseline Results

We established baseline performance on the unchallenged dataset (no blur, darkness, or noise) using mAP50 and mAP50:95 metrics. We then evaluated model performance under various challenging conditions and degrees of severity. 
We also analyzed the degradation in performance under severe challenges, particularly for YOLOv5, YOLOv8, and Faster R-CNN.  Overall, performance degradation ranged from 0.5% to 6%, with the highest variation observed in Faster R-CNN.

## Getting Started

1. **Clone the repository:** `git clone https://github.com/your-username/traffic-sign-detection-vietnam.git`
2. **Install dependencies:** `pip install -r requirements.txt`
3. **Train or test models:**  We will update later. 

## Usage

Provide examples of how to use the trained models to detect and classify traffic signs in new images or video streams.

## Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) guide for details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
