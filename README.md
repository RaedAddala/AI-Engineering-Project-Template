# Data Science Project Template

This repository represents a template for data science, machine learning, and deep learning projects focusing on version control and data versioning using DVC.

This Repository is intended to be be used as template by an AI Team to contain work from the data, serialized models, to the tools built and used by the team:

- data collection
- data visualization
- feature engineering
- model trainings
- model config files
- tests

## Folder Structure

- **`data/`**: Directory for all datasets (raw, processed).
- **`notebooks/`**: Jupyter notebooks for exploration and prototyping.
- **`src/`**: Source code for data processing, feature engineering, and model training.
  - **`data/`**: Scripts for loading and processing data.
  - **`features/`**: Scripts for creating and selecting features.
  - **`models/`**: Scripts for training and evaluating models.
  - **`utils/`**: Utility functions.
  - **`visualization/`**: Scripts for generating data visualizations.
- **`tests/`**: Unit tests for various modules.
- **`models/`**: Serialized models.
- **`config/`**: Store all configuration parameters in YAML files located in the `config/` directory instead of sending parameters as arguments, send config file:

  - `python src/models/model1/train.py --config config/train/model1/config1.py`.

## Data Versionning

`data/` and `models/` will be handled using ***DVC ( Data Version Control)*** to ensure good version control over huge files.

Azure Storage, AWS Storage, Google Drive etc can be used as remote storage for the DVC.

## Guide for Using DVC alongside Git
