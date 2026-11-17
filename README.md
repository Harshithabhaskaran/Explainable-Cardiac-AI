# Explainable Cardiac AI

### AI-Powered Echocardiography Analysis Using Deep Learning, Explainable AI and Large Language Models

\<p align="center">
&#x20; \<img src="[https://img.shields.io/badge/Python-3.x-blue?logo=python](https://img.shields.io/badge/Python-3.x-blue?logo=python)" alt="Python" />
&#x20; \<img src="[https://img.shields.io/badge/Deep%20Learning-PyTorch-orange?logo=pytorch](https://img.shields.io/badge/Deep%20Learning-PyTorch-orange?logo=pytorch)" alt="PyTorch" />
&#x20; \<img src="[https://img.shields.io/badge/Computer%20Vision-OpenCV-green](https://img.shields.io/badge/Computer%20Vision-OpenCV-green)" alt="OpenCV" />
&#x20; \<img src="[https://img.shields.io/badge/Domain-Healthcare%20AI-red](https://img.shields.io/badge/Domain-Healthcare%20AI-red)" alt="Healthcare AI" />
&#x20; \<img src="[https://img.shields.io/badge/Research-Academic-purple](https://img.shields.io/badge/Research-Academic-purple)" alt="Academic Research" />
\</p>

\<p align="center">
&#x20; \<b>An academic research project exploring automated cardiac analysis from echocardiography videos.\</b>
\</p>

---

## Project Overview

**Explainable Cardiac AI** is an academic research project focused on applying deep learning, computer vision, explainable AI and generative AI to echocardiography analysis.

The project investigates automated **Left Ventricle (LV) segmentation**, cardiac cycle analysis, **Ejection Fraction (EF) estimation**, model explainability and Large Language Model (LLM)-based structured report generation.

Using echocardiography datasets such as **EchoNet-Dynamic** and **CAMUS**, the research explores different approaches to extracting cardiac information from ultrasound images and videos.

The overall objective is to investigate an explainable AI-assisted workflow that connects image segmentation, cardiac measurements, visual interpretation and structured report generation.

## Project Demo

Explore the project demonstration:

[**▶ Watch the Echocardiography AI Project Demo**](results/segmentation/Recording%202026-11-17%20095822.mp4)

The demonstration showcases selected project outputs and segmentation results.

## Key Research Components

| Component                      | Description                                                      |
| ------------------------------ | ---------------------------------------------------------------- |
| Echocardiography preprocessing | Video processing and frame extraction                            |
| LV segmentation                | Deep learning-based Left Ventricle segmentation experiments      |
| Cardiac cycle analysis         | End-Diastolic (ED) and End-Systolic (ES) frame identification    |
| EF estimation                  | Experimental cardiac measurement and EF estimation approaches    |
| Explainable AI                 | Grad-CAM-based visualization of model predictions                |
| LLM report generation          | Structured report-generation prototype using Mistral-7B-Instruct |

## Research Workflow

The research is organized into six major stages:

```text
Echocardiography Videos
          |
          v
   Data Preprocessing
          |
          v
  Frame Extraction
          |
          v
  Left Ventricle Segmentation
          |
          v
  Cardiac Cycle Analysis
  (ED / ES Identification)
          |
          v
  Cardiac Measurements
  and EF Estimation
          |
          v
  Explainable AI
  (Grad-CAM Visualization)
          |
          v
  LLM-Based Report Generation
  (Mistral-7B-Instruct)
```

*The diagram represents the overall research direction. Individual components were investigated through separate experiments and notebooks.*

## Experimental Results and Visualizations

The following figures showcase selected outputs from the research experiments.

### 1. Left Ventricle Segmentation

The segmentation experiments investigate deep learning architectures for identifying the Left Ventricle in echocardiography images.

**U-Net Architecture**



**Input, Ground Truth and Segmentation Results**





### 2. Cardiac Cycle Analysis

The project explores cardiac phase identification and changes in ventricular measurements across echocardiography frames.

**End-Diastolic and End-Systolic Frames**



**Left Ventricular Ejection Fraction Visualization**



### 3. Ejection Fraction Estimation

Experimental EF estimation and evaluation visualizations:

**EF Prediction**



**Regression Analysis**



**Bland–Altman Analysis**



**EF Distribution**



### 4. Explainable AI

Grad-CAM-based experiments explore visual interpretation of deep learning predictions and model attention.

These visualizations are intended for research and model interpretation, not as clinical evidence.

### 5. LLM-Based Clinical Report Generation

A report-generation prototype explores the use of **Mistral-7B-Instruct** to generate structured summaries using extracted cardiac measurements.

**Left Ventricular Measurements Over Time**



**Generated Structured Report**



The generated report is an experimental research output and requires independent clinical verification.

## Datasets

This research uses the following echocardiography datasets:

| Dataset         | Research Application                                            |
| --------------- | --------------------------------------------------------------- |
| EchoNet-Dynamic | Echocardiography video analysis and LV segmentation experiments |
| CAMUS           | Additional echocardiographic image segmentation experiments     |

**Dataset access and usage**

- Original datasets are not included in this repository.
- Users must obtain the datasets from their respective official providers.
- All dataset licensing, access and usage restrictions must be followed.
- No patient-related dataset files are distributed through this repository.

Refer to [`data/README.md`](data/README.md) for dataset information.

## Technology Stack

| Category            | Technologies                                                               |
| ------------------- | -------------------------------------------------------------------------- |
| Programming         | Python                                                                     |
| Deep Learning       | PyTorch, TensorFlow, Keras                                                 |
| Computer Vision     | OpenCV, Pillow                                                             |
| Image Processing    | Albumentations, Scikit-image                                               |
| Data Processing     | NumPy, Pandas, SciPy                                                       |
| Machine Learning    | Scikit-learn                                                               |
| Visualization       | Matplotlib, Seaborn                                                        |
| Model Architectures | U-Net, ResNet50-based segmentation experiments, ConvLSTM-based experiments |
| Explainable AI      | Grad-CAM                                                                   |
| Generative AI       | Hugging Face Transformers, Mistral-7B-Instruct                             |
| Development Tools   | Jupyter Notebook, Git, GitHub                                              |

## Repository Structure

```text
Explainable-Cardiac-AI/
│
├── data/
│   └── README.md
│
├── notebooks/
│   ├── 01_data_preprocessing/
│   │   ├── echonet_dynamic_image_and_mask_extractor.ipynb
│   │   └── processing.ipynb
│   │
│   ├── 02_lv_segmentation/
│   │   ├── echo-unet-convlstm-kaggle.ipynb
│   │   ├── ecohnet-dynamic-segmentation-resnet50unet-imagenet.ipynb
│   │   ├── ecohnet_dynamic_segmentation_resnet50unet_imagenet.ipynb
│   │   ├── final.ipynb
│   │   ├── segmenatation.ipynb
│   │   └── segmentation-final.ipynb
│   │
│   ├── 03_ef_estimation/
│   │   └── ef-range.ipynb
│   │
│   ├── 04_explainable_ai/
│   │   └── cardiac-xai.ipynb
│   │
│   ├── 05_camus_experiments/
│   │   ├── camus-echocardiographic-image-segmentation.ipynb
│   │   └── camus-segmentation.ipynb
│   │
│   └── 06_llm_report_generation/
│       └── llm_report.ipynb
│
├── results/
│   ├── ef_estimation/
│   ├── report_generation/
│   └── segmentation/
│
├── .gitignore
├── README.md
└── requirements.txt
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Harshithabhaskaran/Explainable-Cardiac-AI.git
```

### 2. Navigate to the project directory

```bash
cd Explainable-Cardiac-AI
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the relevant notebook and configure the dataset paths and experiment-specific settings before execution.

**Note:** Individual notebooks may require different dataset paths, trained checkpoints, dependency versions and hardware configurations. GPU availability and framework compatibility should be configured according to the selected experiment. Original datasets and trained model weights are not distributed in this repository.

## Research Scope and Limitations

- This repository contains academic research notebooks and experimental visualizations, rather than a fully packaged production application.
- Different notebooks investigate different architectures and experimental approaches; they do not represent one fully validated end-to-end deployment pipeline.
- EF estimation performance depends on the measurement approach and evaluation protocol.
- CAMUS experiments are exploratory and do not independently establish clinical generalization.
- Grad-CAM visualizations provide model-interpretation insights but do not establish clinical validity.
- LLM-generated reports are experimental outputs and require independent clinical review.

**Medical Disclaimer:** This project is intended exclusively for academic research and educational purposes. It is not a certified medical device and must not be used for clinical diagnosis, treatment decisions or patient management.

## Future Work

- Improve temporal consistency in cardiac segmentation.
- Strengthen quantitative evaluation and external validation.
- Investigate more robust cardiac measurement and EF estimation approaches.
- Improve explainability and interpretation of model predictions.
- Explore Retrieval-Augmented Generation (RAG) for evidence-grounded report generation.
- Develop a more reproducible and integrated research demonstration.

## Author

**B. Harshitha**

M.Tech – Computer Science and Engineering (Artificial Intelligence and Machine Learning)
Vellore Institute of Technology, Vellore

- **GitHub:** [Harshithabhaskaran](https://github.com/Harshithabhaskaran)
- **Portfolio:** [Harshitha's Portfolio](https://harshithabhaskaran.github.io/Harshitha_Portfolio/)

---

\<p align="center">   \<b>Explainable Cardiac AI\</b>\<br/>   Exploring the intersection of Artificial Intelligence, Medical Imaging and Healthcare Research. \</p>
