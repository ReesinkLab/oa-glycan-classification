### Computational Reproducibility

All analyses were developed and tested on an Apple M4 chip. The computing environment was standardized using Conda with Python 3.10 and Jupyter desktop version 4.2.5. Key dependencies:

| Package | Version |
|---|---|
| Python | 3.10 |
| PyCaret | 3.3.2 |
| scikit-learn | 1.4.2 |
| imbalanced-learn | 0.12.3 |
| pandas | 2.1.4 |
| numpy | 1.26.4 |
| shap | 0.47.1 |
| matplotlib | 3.7.5|

#### To Reproduce

1. Install Miniconda: https://docs.anaconda.com/miniconda/

2. Create and activate environment:
```bash
conda create -n reviewer_env python=3.10
conda activate reviewer_env
```

3. Install packages:
```bash
pip install -r requirements.txt
```

4. Open `OA-pipeline-v3.ipynb` in your preferred IDE and select `reviewer_env` as your kernel

#### Files Provided
- `OAcombined.csv`
- `train_data.csv`
- `holdout_data.csv`
- `requirements.txt`
- `OA-pipeline.ipynb`

> **Note:** Start at Step 4 in the notebook — the train/holdout split is already saved in the CSVs.

### LOSO analysis

1. Requirements.txt is still identical to `OA-pipeline.ipynb` and will still run `LOSO.ipynb`

2. Open `LOSO.ipynb` in your preferred IDE and you can still use the same `reviewer_env` as your kernel

#### Files Provided

- `LOSO.ipynb`
- `train_data_loso.csv`
- `holdout_data_loso.csv`

> **Note:** Start at Step 4 in the notebook — the train/holdout split is already saved in the CSVs.
