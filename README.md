# Classification-Models-for-Exercise-Science
Model Scripts created in Python Jupyter's Lab (V. 4.2.5).
Code produced by Ayden McCarthy.
Manuscript Title: "Strength, Jump Height, Landing, and Mobility Characteristics Predicts High and Low Performers of a Military Fire and Move Assessment: A Machine Learning Approach".
Program of Study: PhD.
Institution: Macquarie University.
Year: 2025.
# Model Suite

This repository contains three classification models developed as part of a scientific manuscript. Each model is designed to predict binary outcomes (i.e., high or low performers) using logistic regression, random forest, and multilayer perceptron scripts. Each notebook follows a logical order and structure, providing reproducible and transparent data analysis for researchers and practitioners. This suite supports performance modelling, prediction, and cross-validation applications for various populations.

## Table of Contents

- [Installation](#installation)
- [Models](#models)
  - [Notebook Structure](#notebook-structure)
- [Usage](#usage)
  - [Running the Notebooks](#running-the-notebooks)
  - [Parameter Tuning](#parameter-tuning)
  - [Cross-validation](#cross-validation)
- [Output Files](#output-files)
- [Contributions](#contributions)
- [License](#license)

## Installation

To get started, clone this repository and install the required Python packages. Ensure that you have installed Python 3 and that JupyterLab is set up. Use the following commands:

```bash
git clone https://github.com/AydenMQ/Machine_Learning_Models.git
cd Machine_Learning_Models
pip install -r requirements.txt
```

Download the `requirements.txt` file. If not, create a `requirements.txt` file with the following content:

```text
pandas==2.2.2
numpy==1.26.4
scikit-learn==1.5.1
matplotlib==3.9.2
seaborn==0.13.2
scipy==1.13.1
```

```text
pip install -r requirements.txt
```

This ensures compatibility with the specific package versions used in your notebooks.

## Models

This repository includes three predictive classification models, each in a separate Jupyter Notebook (.ipynb). Each notebook forms descriptive statistics of the outcome variable, splits data into high and low performers, splits data further into training and testing sets, and handles training, hyperparameter tuning, and output generation on an unseen testing data set.
The Three Classifications Models Include: Logistic Regression, Random Forest, and Multilayer Perceptron Model.

### Notebook Structure

Each model notebook follows the same logical flow:

1. **Data Import**: Load the dataset, containing predictor metrics, and outcome metrics.
2. **Pre-processing**: Standardises the data set and split the data into 80/20 training and testing datasets, respectively.
3. **Model Training**: Train the specified model with a randomised Gridsearch to tune hyperparameters.
4. **Validation**: Cross-validation (if applicable) to validate the model's performance and generalization capabilities.
5. **Results Output**: Save the results, including confusion matrices, accuracy, recall, precision, and other relevant metrics, to CSV or JSON for reporting.

## Usage

### Running the Notebooks

Open each notebook in JupyterLab and run the cells sequentially. Each cell contains code blocks that need to be executed in order to train and evaluate the model.

1. Start JupyterLab:

   ```bash
   jupyter lab
   ```

2. Open the desired notebook (e.g., `MLP_Model.ipynb`), and run all cells or step through cells to review intermediate results. **Note:** Make sure you have the training and testing set correctly spelled as .csv files.

### Parameter Tuning

Each model can be tuned for optimal performance using scikit-learn’s GridSearchCV or manual adjustment within the notebook. Refer to the hyperparameters section to adjust the parameters. For example, `solver': ['sgd', 'adam']` for optimisers.

### Cross-validation

Each notebook incorporates cross-validation to ensure model robustness on unseen data (testing phase). Results include cross-validated accuracy, recall, and precisions for consistent performance evaluation.

## Output Files

The notebooks generate output files that include:

- **Predictor Influence**: Shows what features are the most influential in reducing the error.
- **Performance Metrics**: Metrics such as Accuracy.
- **Prediction Outputs**: Predicted vs. actual performance values for the test dataset.

## Contributions

Contributions are welcome. If you have suggestions for model improvements, feature requests, or bug fixes, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
