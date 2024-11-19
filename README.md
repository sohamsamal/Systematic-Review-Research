# Automation of Title and Abstract Screening for Clinical Systematic Reviews

This project focuses on automating the abstract screening process for systematic reviews (SRs) using high-sensitivity Natural Language Processing (NLP) methods. By leveraging state-of-the-art models, this work aims to expedite the SR process, which is critical for evidence-based clinical practice.

---

## Table of Contents
1. [Background](#background)
2. [Datasets](#datasets)
3. [Empirical Study of High-Sensitivity NLP Methods](#empirical-study-of-high-sensitivity-nlp-methods)
4. [Systematic Review as Question Answering](#systematic-review-as-question-answering)
5. [Conclusion](#conclusion)
6. [Acknowledgements](#acknowledgements)
7. [References](#references)

---

## Background

### What is a Systematic Review?
Systematic Reviews (SRs) synthesize evidence for clinical practice, forming the basis of clinical guidelines and health policy decisions.

### Objective
The goal is to automate the abstract screening step of SRs using advanced NLP-based techniques. Abstract screening, which involves deciding article inclusion/exclusion based on title and abstract, is a time-intensive and resource-demanding task.

---

## Datasets

### Overview
Experiments were conducted on six datasets:
- **Immune Checkpoint Inhibitors (ICI)**
- **Hormone Replacement Therapy (HRT)**
- **Cooking (COOK)**
- **Accelerometer (ACC)**
- **Acromegaly (ACRO)**
- **COVID**

All datasets were provided by Mayo Clinic. Most are skewed toward fewer positive instances, with ICI being the exception.

### Inclusion/Exclusion Criteria
Each dataset involves applying specific criteria to determine whether an article should be included or excluded.

---

## Empirical Study of High-Sensitivity NLP Methods

### Metrics
The study evaluates:
- **Precision**
- **Sensitivity**
- **F-Measure**

Emphasis is placed on performance for the positive class and generating Precision-Recall curves for high-sensitivity methods.

### Baseline Experiments
Baseline models include:
- **SVM**
- **GloVe**
- **BERT**
- **BioBERT**

---

## Systematic Review as Question Answering

### Reformulation
The SR process is reformulated as a **Question Answering (QA)** task to address limitations of binary classification models:
- **Utilizes inclusion/exclusion criteria**
- **Addresses low-resource data issues**

### Proposed QA Model
The QA model achieved an average **7.6% higher precision** than baseline methods at high-recall levels (~0.99).

---

## Conclusion

The QA-based approach addresses key limitations of traditional methods and demonstrates significant improvement in precision, especially for low-resource datasets. This work contributes toward effective automation for clinical systematic reviews.

---

## Acknowledgements

Special thanks to:
- **Dr. Chitta Baral** for mentorship and research opportunities.
- **Mihir Parmar** for guidance and motivation.
- **Mayo Clinic team**: Dr. Irbaz B. Riaz (MD) and Dr. M. Hassan Murad (MD) for providing high-quality datasets.

---

## References
1. Liberati, A., et al. (2009). *The PRISMA statement for reporting systematic reviews and meta-analyses.* Journal of Clinical Epidemiology, 62(10), e1-e34.
2. Allen, I. E., & Olkin, I. (1999). *Estimating time to conduct a meta-analysis from number of citations retrieved.* JAMA, 282(7), 634-635.
3. Bagheri, E., et al. (2018). *Improving the conduct of systematic reviews: A process mining perspective.* Journal of Clinical Epidemiology, 103, 101-111.
4. Morton, S., et al. (2011). *Finding what works in healthcare: Standards for systematic reviews.*

---

## Thank You!
