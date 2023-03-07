# Linkit Beginner Challenge: Explainable ML using SHAP values

Repository for the Linkit Beginner Challengeon Explainable ML using SHAP values.

## Challenge Description

## Instructions

You can either develop locally by cloning the repo or work in a cloud environment like Google Colab.

### Google Colab (Recommended)

You can use Google Colab to run the notebook.

To get the data inside colab, use the following commands inside a cell (make sure to prefix the line with `!` as it is shown here):

```bash
!pip install dvc
!dvc get https://dagshub.com/MoritzM00/Linkit-Beginner-Challenge-Explainable-ML data/bank.csv -o data/bank.csv
```

This installs `dvc` and downloads the data from the repository.

You may have to install some missing dependencies, that are not pre-installed in the colab environment like `shap`.
with the following command:

```bash
!pip install shap
```

### Local Development

For local development, you can clone this repository locally and run the following commands to set up a virtual environment and install the required dependencies. You must have python installed on your machine.

You can use your preferred method of creating a virtual environment, but we recommend using the builtin `venv`:

```bash
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

Pull the data from the remote storage by running:

```bash
dvc pull
```

Optionally, install development dependencies and pre-commit hooks:

```bash
pip3 install -r requirements-dev.txt
pre-commit install
```

These hooks will run on every commit and will check for linting errors and formatting issues. Optionally, you can remove the output of all cells to make it easier for version control. This part is commented out at the moment.
