# Awesome-HCC-AI

A curated collection of artificial intelligence studies for the early detection and diagnosis of hepatocellular carcinoma (HCC), accompanying our review on technological evolution and research advances.

## Review Article

**Artificial Intelligence for Early Detection and Diagnosis of Hepatocellular Carcinoma: Technological Evolution and Research Advances**

This repository provides the literature collection reviewed in our article and is intended to facilitate literature retrieval, comparison, and future research on artificial intelligence for the early detection and diagnosis of hepatocellular carcinoma.

---

## Scope

This review focuses on artificial intelligence methods for the **early detection and diagnosis of hepatocellular carcinoma (HCC)**, covering the technological evolution from conventional machine learning and radiomics to deep learning, attention mechanisms, Transformers, multimodal learning, and other emerging AI paradigms.

The included original studies are organized into seven major research tasks:

1. **Screening and early risk prediction**
2. **Detection and localization**
3. **Tumor and lesion segmentation**
4. **Classification and differential diagnosis**
5. **LI-RADS and risk stratification**
6. **Multimodal, multitask, and integrated diagnosis**
7. **Clinical validation and physician comparison**

Studies primarily focusing on treatment response prediction, recurrence prediction, survival analysis, or prognosis were not considered part of the main scope unless they were directly related to HCC early detection or diagnostic assessment.

---

## Literature Overview

The current review includes **164 publications published between 2020 and 2026**, consisting of:

- **20** reviews, systematic reviews, and meta-analyses
- **144** original research studies

The 144 original studies are distributed across seven major research categories:

| Research task | Number of studies |
|---|---:|
| Screening and early risk prediction | 20 |
| Detection and localization | 30 |
| Tumor / lesion segmentation | 32 |
| Classification and differential diagnosis | 26 |
| LI-RADS and risk stratification | 13 |
| Multimodal / multitask / integrated diagnosis | 12 |
| Clinical validation and physician comparison | 11 |
| **Total** | **144** |

The annual number of all 164 included publications is:

| Publication year | Number of publications |
|---|---:|
| 2020 | 5 |
| 2021 | 10 |
| 2022 | 7 |
| 2023 | 17 |
| 2024 | 29 |
| 2025 | 47 |
| 2026 | 49 |
| **Total** | **164** |

---

## Technological Evolution

The reviewed studies cover a broad range of artificial intelligence methodologies, including:

- Conventional machine learning
- Radiomics
- Convolutional neural networks
- Three-dimensional deep learning
- Object detection and segmentation networks
- Attention mechanisms
- Transformer-based architectures
- Multitask learning
- Multimodal learning
- Self-supervised learning
- Federated learning
- Generative models
- State-space models and other emerging AI architectures

These methodological developments reflect the transition of HCC-related AI from handcrafted feature engineering toward end-to-end representation learning, multimodal integration, and more generalizable and clinically oriented intelligent systems.

---

## Data Modalities

The reviewed literature includes studies using diverse clinical and biomedical data sources, including:

- Ultrasound
- Contrast-enhanced ultrasound (CEUS)
- Multiphasic computed tomography (CT)
- Multiparametric magnetic resonance imaging (MRI)
- Clinical and demographic variables
- Laboratory indicators
- Electronic health records
- Serum and plasma biomarkers
- Histopathology
- Radiomics
- Proteomics
- Transcriptomics
- Other molecular and omics data
- Multimodal combinations of imaging, clinical, pathological, and molecular information

It should be noted that **multiphasic CT** and **multisequence MRI** represent information integration within the same imaging modality and are not automatically considered heterogeneous multimodal learning.

In this review, multimodal learning mainly refers to the integration of different types of information, such as medical imaging, clinical variables, laboratory biomarkers, pathology, and molecular data.

---

## Evaluation and Validation

In addition to algorithmic performance, this review places particular emphasis on the strength and interpretation of validation evidence.

The reviewed studies involve different evaluation and validation strategies, including:

- Internal train-validation-test splits
- Cross-validation
- Temporal validation
- Cross-dataset evaluation
- Independent external validation
- Multicenter evaluation
- Reader studies
- Human-AI collaboration
- Prospective evaluation
- Clinical workflow assessment

Several important distinctions are considered throughout the review.

### Multicenter Study vs. Independent External Validation

The use of data from multiple institutions does not automatically indicate independent external validation.

When data from multiple centers are pooled before random splitting, the resulting test set should generally be considered an internal or multicenter test set rather than a completely independent external validation cohort.

Independent external validation requires that the external institution or cohort remain separate from model development and be used only for final evaluation.

### Public Dataset Evaluation vs. Clinical External Validation

Evaluation across different public datasets can provide useful evidence of cross-dataset robustness, but it should not be regarded as equivalent to independent clinical external validation performed at a separate hospital or institution.

### Statistical Units

Patients, examinations, lesions, images, slices, videos, and biological samples represent different statistical units.

The numbers reported using these units should therefore not be directly converted or compared.

### Performance Metrics

Different tasks require different evaluation metrics.

Commonly reported metrics include:

- AUC
- Accuracy
- Sensitivity
- Specificity
- Precision
- F1-score
- AUPRC
- C-index
- mAP
- FROC
- Dice coefficient
- IoU
- HD95

These metrics should be interpreted according to the corresponding research task, case spectrum, statistical unit, reference standard, and validation design rather than used for direct model ranking across heterogeneous studies.

---

## Clinical Evidence

The clinical relevance of AI models cannot be determined solely by high performance on internal datasets.

This review therefore distinguishes among:

- AI-alone performance
- Physician-alone performance
- AI-assisted physician performance
- Reader studies
- Workflow studies
- Independent external validation
- Prospective clinical evaluation

AI-assisted reader studies evaluate whether AI can improve physician performance, whereas workflow studies additionally examine practical outcomes such as reading time, false-positive burden, workload, and clinical efficiency.

The available evidence suggests substantial technical potential for AI in HCC early detection and diagnosis, while rigorous independent external validation and prospective clinical evidence remain comparatively limited.

---

## Repository Contents

The repository is intended to provide structured literature records supporting the review.

The main contents include or will include:

```text
Awesome-HCC-AI/
│
├── README.md
│
├── HCC_AI_Literature_List.xlsx
│
└── supplementary/
```

The literature spreadsheet is intended to summarize, where available:

- Publication information
- Publication year
- Research task
- Data modality
- Study population
- Dataset characteristics
- AI methodology
- Model architecture
- Evaluation metrics
- Reference standard
- Validation design
- Independent external validation
- Multicenter information
- Reader-study evidence
- Clinical or workflow evaluation

---

## Important Notes

Several methodological issues should be considered when interpreting the studies included in this repository:

1. **Early HCC, small HCC, and early detection are not equivalent concepts.**  
   Tumor size, clinical stage, and the temporal relationship between AI prediction and confirmed diagnosis should be interpreted separately.

2. **Multicenter data do not automatically indicate external validation.**  
   The independence of the external cohort from model development should be explicitly examined.

3. **Multiphasic or multisequence imaging is not automatically multimodal learning.**  
   True heterogeneous multimodal learning generally involves integration across different information sources.

4. **Public-dataset evaluation and independent clinical external validation represent different levels of evidence.**

5. **Statistical units should be preserved.**  
   Patient-level, lesion-level, examination-level, image-level, and slice-level sample sizes should not be treated as interchangeable.

6. **Performance values should not be compared without considering study design.**  
   Case spectrum, reference standard, prevalence, data partitioning, and validation strategy can substantially affect reported performance.

---

## Updates

This repository accompanies the review article and may be updated as the manuscript is revised or as additional relevant studies are identified.

The current literature collection primarily covers publications from **2020 to 2026**.

---

## Citation

If you find this literature collection useful, please cite the corresponding review article:

**Cai G, et al. Artificial Intelligence for Early Detection and Diagnosis of Hepatocellular Carcinoma: Technological Evolution and Research Advances. 2026.**

The complete bibliographic information will be updated after publication.

A BibTeX entry will also be provided after the article is formally published.

---

## Repository Link

https://github.com/CaiGuoHui123/Awesome-HCC-AI

---

## Contact

For questions, corrections, or suggestions regarding the literature collection, please open an issue in this repository.

---

## Disclaimer

This repository is intended for academic and research purposes.

The included literature reflects the scope and inclusion criteria of the corresponding review and should not be regarded as an exhaustive collection of all artificial intelligence studies related to liver cancer.

The repository does not provide medical advice, and the summarized AI methods should not be used independently for clinical diagnosis or treatment decisions.
