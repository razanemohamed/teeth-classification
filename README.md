# Teeth Classification

An end-to-end teeth-condition classification project from the Cellula internship.
The project trains a PyTorch CNN/EfficientNet model for seven classes and includes
a Streamlit inference demo.

## Repository contents

- `notebooks/Teeth_Classification_Notebook.ipynb` - training and evaluation notebook
- `notebooks/streamlit_app.py` - upload-and-predict demo
- `models/` - selected trained checkpoints and evaluation arrays
- `reports/Teeth_Classification_Report.pdf` - saved evaluation report

## Demonstration

The evaluation report contains representative test results and visualizations.
Raw teeth images are not republished from the training dataset.

## Dataset

The original `Teeth_Dataset` is intentionally not included. It is a large
third-party image dataset and should not be republished without confirming its
license and redistribution terms. Download it from the original source and
place it at:

```text
data/Teeth_Dataset/
```

The notebook expects the `Training`, `Validation`, and `Testing` folders below
that directory.

## Run the notebook

Install the notebook dependencies, then open and run the notebook from the
repository root:

```bash
pip install torch torchvision scikit-learn matplotlib seaborn tqdm pillow jupyter
jupyter notebook notebooks/Teeth_Classification_Notebook.ipynb
```

## Run the demo

```bash
pip install streamlit torch torchvision pillow
streamlit run notebooks/streamlit_app.py
```

The demo loads `models/efficientnet_b0_best.pth`.

## Scope

This repository is a cleaned standalone snapshot of the internship project.
The original combined repository remains the source of historical context.
