# Vanilla CNN and Fine-Tune VGG16

A cats vs dogs image classification project using two models:

- A vanilla convolutional neural network (CNN)
- A fine-tuned VGG16-based model

This repository contains the notebook, dataset folders, saved model weights, and dependency list needed to reproduce the training and evaluation workflow.

## Repository contents

- `Vanilla_CNN_And_Finetune.ipynb` — Jupyter notebook with the full training, validation, and evaluation pipeline
- `requirements.txt` — Python package list required to run the notebook
- `cnn_best.h5`, `cnn_best.keras`, `vgg_best.h5` — saved Keras model files
- `data/` — prepared dataset, separated into `train/`, `val/`, and `test/`
- `PetImages/` — original cats and dogs source images
- `venv/` — local Python virtual environment

## Dataset layout

The `data/` folder should contain the processed dataset split by class and usage:

- `data/train/cats/`
- `data/train/dogs/`
- `data/val/cats/`
- `data/val/dogs/`
- `data/test/cats/`
- `data/test/dogs/`

The `PetImages/` folder contains the original raw image source files for cats and dogs.

## Setup

1. Open a terminal in the repository root.
2. Activate the virtual environment:

   ```powershell
   .\venv\Scripts\Activate.ps1
   ```

3. Install dependencies if needed:

   ```powershell
   pip install -r requirements.txt
   ```

4. Launch the notebook with Jupyter Lab or Jupyter Notebook.

## Usage

- Run the notebook cells from top to bottom.
- The notebook includes data loading, model definition, training, evaluation, and model saving.
- Use the saved weights (`cnn_best.h5`, `cnn_best.keras`, `vgg_best.h5`) for inference or to resume training.

## Notes

- The repository includes the data folders and saved model files so the project can be reproduced locally.
- If you want a lighter repository, you can keep `data/`, `PetImages/`, and model weight files out of version control and regenerate them locally.

## Recommended workflow

1. Activate the environment.
2. Open `Vanilla_CNN_And_Finetune.ipynb`.
3. Test the training and evaluation pipeline.
4. Save model checkpoints and update the notebook as needed.

## Recommended `.gitignore`

Files to ignore for a cleaner repository:

```gitignore
venv/
__pycache__/
*.py[cod]
.ipynb_checkpoints/
.DS_Store
Thumbs.db
.vscode/
```
