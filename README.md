# Explainable Cardiac AI

**AI-Powered Echocardiography Analysis Using Deep Learning, Explainable AI and Large Language Models**

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" />
  <img src="https://img.shields.io/badge/Deep%20Learning-PyTorch-orange?logo=pytorch" />
  <img src="https://img.shields.io/badge/Computer%20Vision-OpenCV-green" />
  <img src="https://img.shields.io/badge/Healthcare-AI-red" />
  <img src="https://img.shields.io/badge/Research-Academic-purple" />
</p>

## Project Overview

Explainable Cardiac AI is an academic research project exploring automated echocardiography analysis using deep learning, computer vision, explainable AI and generative AI.

The project investigates Left Ventricle (LV) segmentation, cardiac cycle analysis, Ejection Fraction (EF) estimation, Grad-CAM-based explainability and Large Language Model (LLM)-based structured report generation.

The research uses EchoNet-Dynamic and CAMUS datasets to explore an integrated workflow for extracting and interpreting cardiac information from echocardiography images and videos.

## Project Demo

Watch the project demonstration:

https://github.com/user-attachments/assets/0829ffe6-8452-4bd3-a6b2-bbbd43cdea08

## Key Research Components

| Component | Description |
|---|---|
| Video Preprocessing | Echocardiography video processing and frame extraction |
| LV Segmentation | Deep learning-based Left Ventricle segmentation |
| Cardiac Cycle Analysis | End-Diastolic (ED) and End-Systolic (ES) frame identification |
| EF Estimation | Experimental cardiac measurement and EF estimation |
| Explainable AI | Grad-CAM-based model interpretation |
| LLM Report Generation | Structured report-generation prototype using Mistral-7B-Instruct |

## Research Workflow

1. Echocardiography video preprocessing
2. Frame extraction and preparation
3. Left Ventricle segmentation
4. Cardiac cycle analysis (ED/ES identification)
5. Cardiac measurements and EF estimation
6. Explainability using Grad-CAM
7. Structured report generation using Mistral-7B-Instruct

Individual components were investigated through separate research experiments and notebooks.

## Datasets

- **EchoNet-Dynamic:** Echocardiography video analysis and LV segmentation experiments.
- **CAMUS:** Additional echocardiographic image segmentation experiments.

Original datasets are not included in this repository. Users must obtain authorized access from the respective dataset providers and comply with their licensing and usage requirements.

Refer to `data/README.md` for dataset information.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Deep Learning | PyTorch, TensorFlow, Keras |
| Computer Vision | OpenCV, Pillow |
| Image Processing | Albumentations, Scikit-image |
| Data Processing | NumPy, Pandas, SciPy |
| Machine Learning | Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Architectures | U-Net, ResNet50-based segmentation, ConvLSTM |
| Explainability | Grad-CAM |
| Generative AI | Hugging Face Transformers, Mistral-7B-Instruct |
| Development | Jupyter Notebook, Git, GitHub |

## Repository Structure

```text
Explainable-Cardiac-AI/
│
├── data/
│   └── README.md
│
├── notebooks/
│   ├── 01_data_preprocessing/
│   ├── 02_lv_segmentation/
│   ├── 03_ef_estimation/
│   ├── 04_explainable_ai/
│   ├── 05_camus_experiments/
│   └── 06_llm_report_generation/
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

Clone the repository:

```bash
git clone https://github.com/Harshithabhaskaran/Explainable-Cardiac-AI.git
cd Explainable-Cardiac-AI
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Configure the dataset paths and experiment-specific settings before running individual notebooks.

## Research Scope and Limitations

- This repository contains academic research notebooks and experimental results, not a production-ready application.
- Different notebooks represent separate experimental approaches rather than one fully validated end-to-end pipeline.
- EF estimation results depend on the measurement approach and evaluation protocol.
- CAMUS experiments are exploratory and do not establish clinical generalization.
- Explainability visualizations do not establish clinical validity.
- LLM-generated reports require independent clinical verification.

**Medical Disclaimer:** This project is intended for academic research and educational purposes only. It is not a certified medical device and must not be used for clinical diagnosis or treatment decisions.

## Future Work

- Improve temporal consistency in cardiac segmentation.
- Strengthen quantitative evaluation and external validation.
- Investigate more robust cardiac measurement approaches.
- Improve explainability and model interpretation.
- Explore Retrieval-Augmented Generation (RAG) for evidence-grounded report generation.
- Develop a reproducible integrated research demonstration.

## Author

**B. Harshitha**  
M.Tech – Computer Science and Engineering (Artificial Intelligence and Machine Learning)  
Vellore Institute of Technology, Vellore

- **GitHub:** [Harshithabhaskaran](https://github.com/Harshithabhaskaran)
- **Portfolio:** [Harshitha's Portfolio](https://harshithabhaskaran.github.io/Harshitha_Portfolio/)

---

*Exploring the intersection of Artificial Intelligence, Medical Imaging and Healthcare Research.*
