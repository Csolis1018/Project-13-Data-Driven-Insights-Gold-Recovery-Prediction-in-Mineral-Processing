# Data-Driven Insights: Gold Recovery Prediction in Mineral Processing

This project focuses on developing a machine learning prototype for Zyfra, a company that builds efficiency solutions for heavy industry. The goal is to predict gold recovery rates from gold ore at different stages of the technological process, supporting production optimization and the elimination of non-profitable parameters.

The analysis uses industrial extraction and purification data, covering the full processing pipeline from rougher flotation to final purification, and applies a custom evaluation metric (sMAPE) tailored to the problem domain.

# Objective

To test the following hypothesis:

Gold recovery rates at both the rougher and final stages can be accurately predicted using machine learning models, improving industrial decision-making when evaluated with a custom combined sMAPE metric.

# 🛠️ Technologies Used

Python: Pandas, NumPy, Scikit-learn

Matplotlib: Data visualization and exploratory analysis

Jupyter Notebook: Interactive environment for analysis and modeling

Industrial Datasets: Gold extraction and purification process data

# Key Steps
# Data Description

Loaded and examined three datasets:

Training dataset

Test dataset

Full source dataset

Reviewed time-based indexing and feature availability.

Identified target variables:

rougher.output.recovery

final.output.recovery

# Data Validation

Verified the correctness of gold recovery calculations using the provided recovery formula.

Calculated recovery values manually for the training set.

Measured the Mean Absolute Error (MAE) between calculated and provided recovery values to confirm data integrity.

# Data Preprocessing

Analyzed features unavailable in the test set and removed them from training data.

Identified feature types (input, output, state, calculation).

Handled missing values and ensured dataset consistency.

# Exploratory Data Analysis

Analyzed how metal concentrations (Au, Ag, Pb) change across processing stages.

Compared particle size distributions between training and test sets to validate model evaluation reliability.

Examined total substance concentrations at different stages.

Detected and removed anomalous values to improve model stability.

# Model Development

Implemented a custom function to compute the final sMAPE metric, combining rougher and final recovery predictions.

Trained multiple machine learning models.

Evaluated models using cross-validation.

Tuned hyperparameters to improve predictive performance.

# Model Evaluation

Selected the best-performing model based on cross-validation results.

Evaluated final performance on the test dataset using the combined sMAPE metric.

# Results

The analysis demonstrates that:

Gold recovery behavior can be effectively modeled using industrial process data.

Validating recovery calculations is essential for reliable modeling.

Removing unavailable features and anomalous values improves prediction quality.

The custom sMAPE metric provides a robust evaluation framework for this industrial problem.

The final model delivers stable and accurate predictions for both rougher and final recovery stages.

These results highlight the value of data-driven modeling for optimizing complex industrial mineral processing workflows.
