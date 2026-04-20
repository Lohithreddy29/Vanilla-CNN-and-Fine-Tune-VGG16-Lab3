# Vanilla CNN and Fine-Tune VGG16

A cats vs dogs image classification project using two models:

- A vanilla convolutional neural network (CNN)
- A fine-tuned VGG16-based model

This repository contains the main training notebook, dependency list, and configuration files for reproducible model development.

## Repository contents

- `Vanilla_CNN_And_Finetune.ipynb` — main Jupyter notebook with data loading, model definition, training, evaluation, and saving
- `requirements.txt` — Python package list required to run the notebook
- `README.md` — project documentation
- `.gitignore` — repository ignore rules for local files and large artifacts

> The dataset, model weight files, and local virtual environment are intentionally excluded from version control.

## Project data and models

This repository expects the following local paths when running the notebook:

- `data/` — processed dataset split into `train/`, `val/`, and `test/`
- `PetImages/` — original raw image source files for cats and dogs
- `cnn_best.h5`, `cnn_best.keras`, `vgg_best.h5` — optional saved model weight files for inference or resuming training

If you do not have these files locally, either regenerate them with the notebook or download them from a separate archive.

## Dataset layout

The processed dataset should be arranged as follows:

- `data/train/cats/`
- `data/train/dogs/`
- `data/val/cats/`
- `data/val/dogs/`
- `data/test/cats/`
- `data/test/dogs/`

The `PetImages/` folder should contain the original raw images in:

- `PetImages/Cat/`
- `PetImages/Dog/`

## Setup

1. Open a terminal in the repository root.
2. Create and activate a Python virtual environment if needed:

   ```powershell
   python -m venv venv
   .\venv\Scripts\Activate.ps1
   ```

3. Install dependencies:

   ```powershell
   pip install -r requirements.txt
   ```

4. Launch the notebook with Jupyter Lab or Jupyter Notebook.

## Usage

- Open `Vanilla_CNN_And_Finetune.ipynb`.
- Run the notebook cells in order.
- If model weights are available locally, use them for inference or fine-tuning.
- If not, train the models from scratch with the notebook.

## Notes

- Large files and folders such as `data/`, `PetImages/`, and model weights are excluded from Git using `.gitignore`.
- Keep the notebook and dependency list tracked in version control.
- Use the included `requirements.txt` to reproduce the environment on another machine.

## Recommended workflow

1. Prepare or download the dataset locally.
2. Activate the virtual environment.
3. Install required packages.
4. Open and run `Vanilla_CNN_And_Finetune.ipynb`.
5. Save trained weights locally if needed.

## `.gitignore`

This repository ignores local artifacts and large binary files:

```gitignore
venv/
__pycache__/
*.py[cod]
.ipynb_checkpoints/
.DS_Store
Thumbs.db
.vscode/
data/
PetImages/
*.h5
*.keras
```
