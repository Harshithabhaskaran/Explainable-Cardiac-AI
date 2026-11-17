# Explainable Cardiac AI
### Echocardiography Segmentation, Ejection Fraction Estimation and Clinical Report Generation

## Overview

This project explores an AI-based pipeline for analyzing echocardiography videos, segmenting the Left Ventricle (LV), estimating cardiac Ejection Fraction (EF), and generating structured clinical summaries.

The research combines deep learning, image processing, explainable AI, and language-model-based report generation.

## Research Objectives

- Process echocardiography videos and extract relevant frames.
- Segment the Left Ventricle using deep learning.
- Identify end-diastolic (ED) and end-systolic (ES) frames.
- Estimate Ejection Fraction from ventricular measurements.
- Explore explainability techniques for model interpretation.
- Generate structured clinical summaries from extracted measurements.

## Methodology

1. **Data preprocessing:** Echocardiography video and frame preparation.
2. **LV segmentation:** U-Net-based segmentation experiments, including temporal modeling.
3. **EF estimation:** ED/ES identification and EF calculation.
4. **External evaluation:** Experiments using the CAMUS dataset.
5. **Explainability:** Grad-CAM-based model interpretation experiments.
6. **Report generation:** Prototype for generating structured summaries using extracted measurements and language-model techniques.

## Reported Research Results

The following are the results reported in the research manuscript and are subject to final verification against the saved experimental outputs.

| Metric | Reported result |
|---|---:|
| EF Mean Absolute Error | 6.16 percentage points |
| EF R² | 0.613 |
| Segmentation Dice | 0.94 |
| Segmentation IoU | 0.86 |
| Segmentation Accuracy | 0.986 |

These results should be interpreted in the context of the experimental datasets and evaluation protocols described in the manuscript.

## Technologies Used

- Python
- PyTorch
- TensorFlow / Keras
- OpenCV
- NumPy and Pandas
- Scikit-learn
- SciPy
- Matplotlib
- Albumentations
- Segmentation Models PyTorch
- Hugging Face Transformers

## Repository Structure

```text
Explainable-Cardiac-AI/
├── data/
│   └── README.md
├── docs/
│   ├── manuscript/
│   ├── thesis/
│   ├── literature_review/
│   ├── presentations/
│   └── project_documentation/
├── notebooks/
│   ├── 01_data_preprocessing/
│   ├── 02_lv_segmentation/
│   ├── 03_ef_estimation/
│   ├── 04_explainable_ai/
│   ├── 05_camus_experiments/
│   └── 06_llm_report_generation/
├── results/
├── src/
│   ├── preprocessing/
│   ├── segmentation/
│   ├── ef_estimation/
│   ├── explainability/
│   └── report_generation/
├── .gitignore
└── requirements.txt
```

## Dataset Information

This research uses EchoNet-Dynamic and CAMUS datasets.

The original datasets are not included in this repository. Users must obtain authorized access from the respective dataset providers and comply with their usage terms.

Refer to `data/README.md` for details.

## Reproducibility

The notebooks document the research experiments and development process.

The reusable Python modules and installation instructions are being organized. Exact package versions, model checkpoints, and execution instructions will be added after environment verification.

## Limitations

- EF estimation is an experimental research implementation and is not a substitute for clinical measurement.
- External dataset performance should be interpreted according to the corresponding evaluation protocol.
- Report generation is a research prototype, not a clinically validated reporting system.
- This project is intended for academic and research purposes, not clinical diagnosis.

## Future Work

- Improve temporal consistency in LV segmentation.
- Strengthen external validation and reproducibility.
- Refine explainability methods.
- Explore retrieval-augmented generation for evidence-grounded clinical summaries.
- Investigate deployment options for research demonstrations.

## Author

**B. Harshitha**  
M.Tech Computer Science and Engineering – AI & ML  
Vellore Institute of Technology, Vellore

GitHub: [Harshithabhaskaran](https://github.com/Harshithabhaskaran)

Portfolio: [Harshitha's Portfolio](https://harshithabhaskaran.github.io/Harshitha_Portfolio/)

---

*Academic research project in echocardiography analysis using artificial intelligence.*
