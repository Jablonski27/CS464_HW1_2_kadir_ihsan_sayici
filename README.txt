QUESTION 2 AND 3: Amazon Review Classification - README

Overview

This project is focused on classifying Amazon product reviews using different machine learning models. The tasks are performed as part of Homework 1 for the CS464 course. The project includes solutions for Questions 2 and 3 which involve classification tasks using Multinomial and Bernoulli Document Models.

Prerequisites

Before running the code, ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- Required Python libraries: numpy, pandas, matplotlib

How to Execute the Code

Jupyter Notebook
1. Open Jupyter Notebook by running the following command in your terminal:
    ```bash
    jupyter notebook
    ```
2. Navigate to the folder containing the project files.
3. Open the provided notebook file named `Question 2 and 3 (Amazon Reviews Classification).ipynb`.
4. Run all the cells in the notebook sequentially to execute the code and obtain the results.

File Structure

- x_train.csv: Training data containing review features.
- y_train.csv: Training data containing review labels (0: Negative, 1: Neutral, 2: Positive).
- x_test.csv: Test data containing review features.
- y_test.csv: Test data containing review labels.
- Question 2 and 3 (Amazon Reviews Classification).ipynb**: Jupyter Notebook containing the full implementation.
- report.pdf: The final report containing the detailed solution.
- README.txt: This file, providing details on how to execute the program.

Parameters

1. Alpha: Smoothing parameter for the Multinomial and Bernoulli models. It defaults to 0 for no smoothing and can be set to 1 for Laplace smoothing.

Default Values

- The `alpha` parameter in the Multinomial model defaults to `alpha = 0`.
- The `alpha` parameter in the Bernoulli model defaults to `alpha = 1`.

How to Run the Models and Interpret the Outputs

1. Question 3.1: You can view the distributions of each class (Negative, Neutral, Positive) in the training and test datasets. The results are displayed as pie charts, indicating the percentage of each class.
   - **Output**: Pie charts showing class distributions are displayed.

2. Question 3.2 & 3.3: Trains a Multinomial Document Model without and with smoothing. The accuracy of the model is displayed for both cases.
   - Output: 
     - Accuracy without smoothing is approximately 0.581.
     - Accuracy with smoothing (alpha = 1) is approximately 0.649.

3. Question 3.4: Trains a Bernoulli Document Model with smoothing (alpha = 1). Displays the accuracy for this model.
   - Output: 
     - Accuracy with smoothing is approximately 0.641.

4. Performance Comparison: The notebook prints out the relative accuracy values compared to the expected results mentioned in the homework document.

5. Runtime: The final cell of the notebook displays the total runtime for executing all tasks, which should be around 22 seconds.

Outputs

- Pie charts indicating the class distribution of the reviews in both training and test datasets.
- Accuracy scores for the Multinomial and Bernoulli models, both with and without smoothing.
- Log ratio values for occurrences of words 'good' and 'bad' in the positive class.