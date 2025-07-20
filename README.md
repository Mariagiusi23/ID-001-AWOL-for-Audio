# 🌀 AWOL for Audio — Language-to-Sound Generation via Parametric Synthesis

**DLAI 2024/2025 Project — ID001**  
_Author: Mariagiusi23 • Based on CLAP + RealNVP + FM Synthesis_

This project explores generating sound from text descriptions by adapting the AWOL (Analysis Without synthesis using Language) framework from 3D to the audio domain. The system learns to map natural language prompts to the parameters of a procedural FM synthesizer using MLP and RealNVP models.

---

## 🎯 Objective

Translate the AWOL framework from 3D geometry to sound generation by:

- Using CLAP embeddings from textual prompts,
- Mapping embeddings to synthesis parameters via learnable models,
- Rendering semantically coherent and controllable audio,
- Exploring interpolation/extrapolation in latent space.

---

## 📁 Repository Structure

All notebooks are in the `notebook/` folder. You can run them directly on Google Colab:

| Notebook | Description | Open in Colab |
|----------|-------------|----------------|
| `01_BaselineClapEmbeddingToFmSynthesis.ipynb` | Baseline pipeline CLAP → MLP → FM synth (no training). | [🔗 Open](https://colab.research.google.com/github/Mariagiusi23/ID-001-AWOL-for-Audio/blob/main/notebook/01_BaselineClapEmbeddingToFmSynthesis.ipynb) |
| `02_AWOL_SupervisedMapping.ipynb` | Supervised training of the MLP model on a manual dataset. | [🔗 Open](https://colab.research.google.com/github/Mariagiusi23/ID-001-AWOL-for-Audio/blob/main/notebook/02_AWOL_SupervisedMapping.ipynb) |
| `03_AWOL_RealnvpMapping.ipynb` | RealNVP implementation for semantic → audio parameter mapping. | [🔗 Open](https://colab.research.google.com/github/Mariagiusi23/ID-001-AWOL-for-Audio/blob/main/notebook/03_AWOL_RealnvpMapping.ipynb) |
| `04_AWOL_LatentSpaceExploration.ipynb` | Latent space interpolation, baseline comparison, Gradio demo. | [🔗 Open](https://colab.research.google.com/github/Mariagiusi23/ID-001-AWOL-for-Audio/blob/main/notebook/04_AWOL_LatentSpaceExploration.ipynb) |


---

