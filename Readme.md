# Protein Subcellular Localization with Diffusion-Augmented Training

This repository explores the use of diffusion-generated synthetic data for improving multi-label classification of protein subcellular localization.

## 📂 Project Structure

- `Baselines/`: Standard supervised models using ResNet and Transformer backbones with different loss functions (BCE, Focal, ArcFace).
- `Diffusion_mix/`: Notebooks related to image generation (DDPM), synthetic data mixing strategies (MixLoss, MixRepresentation), and final submission scripts.

## 🧪 Datasets

This project uses the [Human Protein Atlas Kaggle Dataset](https://www.kaggle.com/competitions/human-protein-atlas-image-classification/).

To obtain train/test data, please follow Kaggle's rules and download from the official source. Generated synthetic images (~10k) are available at:

🔗 [\[Google Drive link here\]](https://drive.google.com/drive/folders/1tSOZjYSljlmgKWhwMwY25soZMLnzRE-1?usp=sharing)

## 📊 Key Findings

- MixModels with feature-level mixing improved validation scores, but failed to generalize to Kaggle test sets.
- Simplified DDPM successfully generated label-consistent synthetic images but exhibited distribution mismatch with real samples.

<!-- See full results in our [final report (PDF)](link-to-your-pdf-if-applicable). -->

## 💻 Environment

- Google Colab Pro+ (A100 GPU)
- Python 3.10
- Key dependencies: `torch`, `transformers`, `tqdm`, `scikit-learn`

<!-- ## 📜 Citation

If you use or reference this work, please cite: -->
