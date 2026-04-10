# Vanilla CNN and Fine-Tune VGG16

This repository contains a complete image classification project for cats vs dogs using a vanilla CNN and a fine-tuned VGG16 model.

## What is included

- Vanilla_CNN_And_Finetune.ipynb: Jupyter notebook with the full training, validation, and evaluation pipeline.
- README.md: This project documentation file.
- equirements.txt: Exact Python dependencies needed to run the notebook and reproduce results.
- env/: Included Python virtual environment with all installed packages.
- data/: Prepared dataset split into training, validation, and test folders.
- PetImages/: Original source image dataset for cats and dogs.
- cnn_best.h5, cnn_best.keras, gg_best.h5: Saved Keras model weights.

## Repository structure

`
Vanilla-CNN-and-Fine-Tune-VGG16-Lab3/
+-- README.md
+-- requirements.txt
+-- Vanilla_CNN_And_Finetune.ipynb
+-- cnn_best.h5
+-- cnn_best.keras
+-- vgg_best.h5
+-- data/
¦   +-- train/
¦   ¦   +-- cats/
¦   ¦   +-- dogs/
¦   +-- val/
¦   ¦   +-- cats/
¦   ¦   +-- dogs/
¦   +-- test/
¦       +-- cats/
¦       +-- dogs/
+-- PetImages/
¦   +-- Cat/
¦   +-- Dog/
+-- venv/
    +-- Scripts/
    +-- Lib/
    +-- ...
`

## Setup instructions

1. Open a terminal in the repository root.
2. Activate the virtual environment:
   `powershell
   .\venv\Scripts\Activate.ps1
   `
3. Install dependencies if needed:
   `powershell
   pip install -r requirements.txt
   `
4. Open Vanilla_CNN_And_Finetune.ipynb in Jupyter Notebook or JupyterLab.

## Notes

- env/, data/, and PetImages/ are included in this repository so the project is fully reproducible.
- equirements.txt captures the environment packages used for this project.
- The model weight files are included so you can run inference or resume training.

## Recommended workflow

- Make changes in Vanilla_CNN_And_Finetune.ipynb.
- Keep the datasets and models in place.
- Use the included equirements.txt to recreate the environment on another machine.
