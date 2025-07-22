# 🎧 AWOL for Audio — Language-to-Sound Generation via Parametric Synthesis

**DLAI 2024/2025 Project — ID001**  
**Author**: Mariagiusi Nicodemo  
*Based on CLAP + RealNVP + FM Synthesis*

This project explores generating sound from text descriptions by adapting the AWOL (Analysis Without synthesis using Language) framework from 3D to the audio domain. The system learns to map natural language prompts to the parameters of a procedural FM synthesizer using MLP and RealNVP models.

---

## 🎯 Objective

Translate the AWOL framework from 3D geometry to sound generation by:

- Using CLAP embeddings from textual prompts,  
- Mapping embeddings to synthesis parameters via learnable models,  
- Rendering semantically coherent and controllable audio,  
- Exploring interpolation/extrapolation in latent space.

---

## 🧱 Repository Structure

All notebooks are in the `notebook/` folder and runnable on Google Colab.

| Notebook                                  | Description                                                                | Open in Colab |
|------------------------------------------|----------------------------------------------------------------------------|----------------|
| `01_BaselineClapEmbeddingToFmSynthesis.ipynb` | Baseline pipeline CLAP → MLP → FM synth (no training).                    | [▶️ Open](...) |
| `02_AWOL_SupervisedMapping.ipynb`        | Supervised training of the MLP model on a manual dataset.                 | [▶️ Open](...) |
| `03_AWOL_RealNvpMapping.ipynb`           | RealNVP implementation for semantic → audio parameter mapping.           | [▶️ Open](...) |
| `04_AWOL_LatentSpaceExploration.ipynb`   | Latent space interpolation, baseline comparison, Gradio demo.            | [▶️ Open](...) |

> Replace `(...)` with actual Colab links if you want them clickable from the README.

---

## ⚙️ Setup

You can run the project in a new environment or in Google Colab.

### 🔧 Local

1. Clone the repository:
   ```bash
   git clone https://github.com/Mariagiusi23/ID-001-AWOL-for-Audio.git
   cd ID-001-AWOL-for-Audio


