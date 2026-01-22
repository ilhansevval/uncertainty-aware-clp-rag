# Uncertainty-Aware Multimodal RAG for Safe Medical Question-Answering in Cleft Lip and Palate Assessment

<p align="center">
  <img src="https://img.shields.io/badge/IEEE-Access-blue?style=for-the-badge&logo=ieee" alt="IEEE Access">
  <img src="https://img.shields.io/badge/Python-3.9+-green?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/PyTorch-2.0+-red?style=for-the-badge&logo=pytorch" alt="PyTorch">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="License">
</p>

<p align="center">
  <b>🔬 Official implementation of our IEEE Access 2026 paper</b>
</p>

---

## 📢 Code Availability Notice

> **⚠️ The source code will be released upon paper publication.**
>
> We are currently in the peer review process. Once the paper is officially published in IEEE Access, the complete codebase including training scripts, model weights, and evaluation pipelines will be made publicly available.
>
> **Expected release: After publication acceptance**

---

## 📄 Paper

**Uncertainty-Aware Multimodal RAG for Safe Medical Question-Answering in Cleft Lip and Palate Assessment**

*Sevval Ilhan<sup>1,2</sup>, Ilhan Aytutuldu<sup>2</sup>, and Yusuf Sinan Akgul<sup>2</sup>*

<sup>1</sup>Department of Information Systems and Technology, Okan University, Istanbul, Turkey  
<sup>2</sup>Department of Computer Engineering, Gebze Technical University, Kocaeli, Turkey

---

## 🎯 Abstract

Medical question–answering systems that integrate multimodal perception with large language models are particularly prone to hallucinations under high predictive uncertainty. This work proposes an **uncertainty-aware multimodal retrieval-augmented generation (RAG) framework** for cleft lip and palate (CL/P) assessment that explicitly propagates classification confidence through both evidence retrieval and response generation.

### Key Contributions

- 🔹 **Multimodal CL/P Classification**: Combining ultrasound tongue imaging (UTI) and acoustic features with curriculum-guided learning
- 🔹 **Uncertainty-Aware RAG**: Confidence-weighted retrieval and generation for safer medical QA
- 🔹 **Hospital AI Simulation**: Persona-driven evaluation framework for behavioral safety assessment
- 🔹 **Clinical Decision Support**: Responsible AI design that communicates uncertainty and recommends specialist referral

---

## 🖥️ System Interface

<p align="center">
  <img src="images/Interface.png" alt="AI Medical Consultation Interface" width="100%">
</p>

*Figure: The AI Medical Consultation platform showing real-time multimodal analysis with uncertainty-aware RAG-based clinical responses.*

---

## 📊 Data Modalities

### Mel Spectrogram Features
<p align="center">
  <img src="images/mel_spectrogram.png" alt="Mel Spectrogram Visualization" width="600">
</p>

*Mel spectrogram representations capturing acoustic patterns related to resonance and hypernasality in CL/P speech.*

### Ultrasound Tongue Imaging (UTI)
<p align="center">
  <img src="images/uti.png" alt="Ultrasound Tongue Image" width="500">
</p>

*Midsagittal ultrasound tongue image showing articulatory dynamics for speech analysis.*

---

## 🏗️ Framework Architecture

<p align="center">
  <img src="images/framework_arch.png" alt="AI Medical Consultation Interface" width="100%">
</p>

## 📈 Key Results

### Classification Performance (Audio-only with Curriculum Learning)

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| CNN+LSTM | **0.89** | 0.87 | 0.90 | **0.89** |
| Vision Transformer | 0.86 | 0.85 | 0.85 | 0.85 |
| ResNet3D + Attention | 0.85 | 0.83 | 0.81 | 0.81 |

### RAG Performance Comparison

| Approach | Context Precision | Faithfulness | Joint F1 |
|----------|------------------|--------------|----------|
| Naive RAG | 0.71 | 0.81 | 0.34 |
| Adaptive RAG | 0.75 | 0.84 | 0.44 |
| Classification-Aware | 0.81 | 0.87 | 0.47 |
| **Uncertainty-Aware** | **0.86** | **0.90** | **0.49** |

---

## 📚 Dataset

This work uses the **UltraSuite CLEFT** dataset:

> Eshky, A., et al. "UltraSuite: A repository of ultrasound and acoustic data from child speech therapy sessions." *arXiv preprint arXiv:1907.00835*, 2019.

**Dataset Access:** [UltraSuite Repository](https://ultrasuite.github.io/)

---

## 🤝 Authors

<table>
  <tr>
    <td align="center">
      <b>Sevval Ilhan</b><br>
      <sub>Okan University & GTU</sub><br>
      <a href="mailto:sevval.ilhan@okan.edu.tr">📧 Email</a>
    </td>
    <td align="center">
      <b>Ilhan Aytutuldu</b><br>
      <sub>Gebze Technical University</sub><br>
      <a href="mailto:iaytutuldu@gtu.edu.tr">📧 Email</a>
    </td>
    <td align="center">
      <b>Yusuf Sinan Akgul</b><br>
      <sub>Gebze Technical University</sub><br>
      <a href="mailto:akgul@gtu.edu.tr">📧 Email</a>
    </td>
  </tr>
</table>

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- [UltraSuite](https://ultrasuite.github.io/) for providing the CLEFT dataset

---

<p align="center">
  <b>⭐ Star this repository if you find it helpful!</b>
</p>

<p align="center">
  <i>For questions and collaboration inquiries, please contact the authors.</i>
</p>