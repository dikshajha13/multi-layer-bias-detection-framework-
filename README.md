# Multi-Layer Bias Detection Framework (MLBDF)
This repository contains the official implementation of Multi-Layer Bias Detection Framework (MLBDF), an undergraduate research initiative focused on fairness in machine learning.

MLBDF proposes a novel approach to analyzing how algorithmic bias originates, manifests, and propagates through different stages of a deep learning pipeline. It introduces two core methodologies: Bias Residual Propagation (BRP) and Dual-Dataset Fairness Transfer (DDFT).

# 🔬 Core Methodology
MLBDF operates across multiple abstraction layers of the machine learning lifecycle to intercept and mitigate bias:

Dataset-Level Bias Analysis: Evaluates representation disparities and multi-attribute correlation in training data before modeling begins.

Bias Residual Propagation (BRP): Tracks how bias compounded in early neural network layers propagates downstream into final latent representations.

Dual-Dataset Fairness Transfer (DDFT): A transfer learning framework designed to enforce fairness constraints across distinct but distributionally related domains.

# 🚀 Key Features
Layer-Wise Bias Tracking: Analyze neural network layers individually using custom heatmaps and representation alignment metrics.

Baseline Benchmarking: Includes a robust Logistic Regression baseline for clear delta tracking between traditional and deep learning models.

Comprehensive Fairness Metrics: Evaluates models using standard quantitative fairness constraints:

* Demographic Parity ($\Delta DP$)
* Equal Opportunity ($\Delta EO$)

Multi-Attribute Evaluation: Moves beyond single-variable bias to evaluate intersections of multiple sensitive attributes simultaneously.

# 🛠️ Tech Stack & Dependencies
The framework is built using the standard Python scientific computing and deep learning ecosystem:

- Deep Learning: PyTorch

- Machine Learning & Baselines: Scikit-learn

- Data Manipulation: Pandas, NumPy

- Visualization: Matplotlib, Seaborn


# Supported Datasets
To run the full pipeline, download and structure the following datasets in your local environment:

CelebA Dataset (Celebrity Attributes)

UTKFace Dataset (Large-scale face dataset with age, gender, and ethnicity annotations)


# Framework 

 ## overall framework 
 The overall framework illustrates the complete pipeline of the proposed Multi-Layer Bias Detection Framework (MLBDF), from dataset preprocessing and bias analysis to model training, Bias Residual Propagation (BRP), fairness evaluation, and Dual-Dataset Fairness Transfer (DDFT) for bias mitigation. Diagram below helps to sum up the flow of the model:
 <img width="260" height="373" alt="image" src="https://github.com/user-attachments/assets/77a369ae-de84-41b5-bb41-3a2bd7905d7b" />

 
 ## workflow
 The Diagrams below represent the dynamic behavior of the system by showing the sequence of interactions between different components over time.
The process begins with the user uploading a dataset and configuring parameters. The system then performs preprocessing, followed by model training and feature extraction. The BRP module tracks bias propagation, and the DDFT module applies fairness improvements. Finally, the evaluation module generates results, which are displayed to the user.


 <img width="377" height="240" alt="image" src="https://github.com/user-attachments/assets/7c6aac7a-f57c-408c-be9a-2e62f0ccb58c" />
 

 <img width="493" height="149" alt="image" src="https://github.com/user-attachments/assets/ee1951e2-61a9-4816-8457-e006146f01fb" />


 # Current Status & Future Roadmap
 [!NOTE]

Research Prototype (Work in Progress): This repository currently reflects the first draft implementation of the framework. Active development is underway to refine core algorithms and expand experimental setups.

# 📄 Research Paper
The initial comprehensive write-up detailing the mathematical formulations of BRP and DDFT can be found in the research-paper/ directory:
 



