# Biomedical Machine Translation with M2M-100

This project explores a two-stage fine-tuning approach to domain adaptation for machine translation, using the M2M-100 multilingual model as the baseline. The goal is to enhance translation quality in the biomedical domain, particularly for Vietnamese.

## 🔧 Methodology

### Stage 1: General-Domain Fine-tuning
- Fine-tuned M2M-100 on general-domain Vietnamese-English parallel datasets: **MTet** and **PhoMT**.
- Objective: Provide a strong foundational translation ability across general language usage.

### Stage 2: Biomedical Domain Adaptation
- Further fine-tuned the model on biomedical datasets:
  - **MedEV** (Vietnamese-English biomedical dataset)
  - **MIMIC-III** (clinical English dataset) with **back-translation** into Vietnamese.
- Goal: Enhance the model's accuracy and fluency for domain-specific (medical) language.

## 🧠 Additional Techniques

- ✅ **Domain Vocabulary Injection**: Constructed a specialized medical term dictionary and appended it to the training data to help the model learn biomedical terminology. This improves domain coverage and supports better domain adaptation.
- ⏳ **Homograph Disambiguation (Planned)**: Developing methods to handle ambiguous terms with multiple meanings.
- ⏳ **Ensemble Learning (Planned)**: Exploring model ensemble strategies to boost final translation performance.

## 📈 Outcomes
- Noticeable improvement in translation quality within the biomedical domain, particularly in handling terminology and maintaining contextual accuracy.
- Domain vocabulary injection increased term coverage in validation samples.

## 📁 Note
This repository is private due to ongoing research and unpublished data. A demo or more information can be provided upon request.

