Online News Popularity Prediction using Logistic Regression
Faculty Submission Details 
id : https://github.com/complexiota
  Field                      Details
  Student Name               Sanskar Santosh Randive
College                    Zeal College of Engineering, Narhe, Pune
Branch                     Artificial Intelligence and Data Science (AI&DS)
Academic Year / Class      Third Year B.Tech
Subject                    RCA
Practical / Activity No.   RCA Activity 2
1. Project Title
Online News Popularity Prediction using Logistic Regression
2. Aim
To build a Logistic Regression classification model that predicts
whether an online news article is popular or not based on the article's
available features.
3. Objective
- Load and explore the Online News Popularity dataset.
- Check the dataset information, descriptive statistics, missing
  values, and duplicate records.
- Create a binary target variable named popularity.
- Split the dataset into training and testing sets.
- Scale the input features.
- Train a Logistic Regression model.
- Evaluate the model using classification metrics and visualizations.
- Test predictions using a sample record.
4. Dataset
- Dataset file: OnlineNewsPopularity.csv
- Target source column: shares
- Target variable created: popularity
- Input features: Dataset columns except url, shares, and
  popularity.
The notebook defines popularity as follows:
- 1 -- Popular article (shares >= 1400)
- 0 -- Not popular (shares < 1400)
Place OnlineNewsPopularity.csv in the same working directory as the
notebook, or update the CSV path in the loading cell.
5. Technologies and Libraries
- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
6. Methodology / Steps Performed
1. Import the required Python libraries.
2. Load the CSV dataset using Pandas.
3. Inspect dataset dimensions, data types, and statistical information.
4. Check missing values and duplicate rows.
5. Remove extra spaces from column names.
6. Create the binary popularity target using the 1400 shares
   threshold.
7. Visualize the popularity class distribution.
8. Separate input features (X) and target (y).
9. Split the data into 80% training and 20% testing sets using
   random_state=42 and stratification.
10. Apply StandardScaler to scale the features.
11. Plot the sigmoid function.
12. Train the Logistic Regression model with max_iter=1000.
13. Generate predicted classes and probabilities.
14. Evaluate the model using a confusion matrix, accuracy, precision,
    recall, specificity, F1-score, classification report, and ROC-AUC.
15. Compare model accuracy with a majority-class baseline.
16. Compare classification results at thresholds 0.3, 0.5, and 0.7.
17. Visualize predicted probabilities and make a prediction for a sample
    record.
7. Evaluation Metrics
  Metric                              Purpose
  Accuracy                            Proportion of all predictions that
are correct

  Precision                           Proportion of predicted popular
articles that are actually popular

  Recall                              Proportion of actual popular
articles correctly identified

  Specificity                         Proportion of actual not-popular
articles correctly identified

  F1-score                            Harmonic mean of precision and
recall

  Confusion Matrix                    Shows true positives, true
negatives, false positives, and
false negatives
ROC-AUC                             Measures the model's ability to
distinguish between the two classes
The notebook calculates these values when its cells are executed. Refer
to the notebook output for the actual metric values.
8. Visualizations
The notebook includes: - News popularity distribution bar chart -
Sigmoid function plot - Confusion matrix - ROC curve - Predicted
probability scatter plot
9. How to Run
1. Open ActivityRCA2.ipynb in Google Colab or Jupyter Notebook.
2. Upload OnlineNewsPopularity.csv to the notebook environment.
3. Confirm that the CSV path in the data-loading cell is correct. The
   current notebook uses /content/OnlineNewsPopularity.csv.
4. Run all cells from top to bottom.
5. Review the printed evaluation metrics, prediction table, and plots.
10. Expected Outcome
The Logistic Regression model classifies news articles into Popular
(1) and Not Popular (0) based on the selected dataset features.
The notebook reports evaluation metrics and displays visualizations to
assess the classifier. Actual performance values depend on the dataset
and execution results.
11. Files Included
- ActivityRCA2.ipynb -- Python notebook containing the complete
  implementation.
- OnlineNewsPopularity.csv -- Dataset required to execute the
  notebook.
- README.md -- Project description and faculty submission
  information.
12. Conclusion
A Logistic Regression classification workflow was implemented for
predicting online news popularity. The dataset was explored, the target
variable was created using a shares threshold of 1400, and the features
were split and scaled before model training. The model was evaluated
using multiple classification metrics and plots.
Submitted by: Sanskar Santosh Randive
Branch: AI&DS
College: Zeal College of Engineering, Narhe, Pune
