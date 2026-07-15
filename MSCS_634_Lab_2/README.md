# Lab 2: Classification Using KNN and Radius Neighbors

**Name:** Malik Black  
**Course:** Big Data and Data Mining (MSCS-634-B01)

## Project Overview
This lab focuses on implementing and comparing two classification algorithms—K-Nearest Neighbors (KNN) and Radius Neighbors (RNN)—using the Wine dataset.

## Tools Used
* Python 3.11
* VS Code
* scikit-learn
* pandas
* matplotlib

## Observations
* **KNN Performance:** The model achieved a peak accuracy of approximately 0.86 at K=11. 
* **Radius Neighbors Performance:** The accuracy for the Radius Neighbors classifier peaked at 0.75, and showed a trend of stabilizing as the radius increased.
* **Comparison:** Based on the results, KNN proved to be more effective for this dataset as it better captured the local structure of the data compared to the fixed-radius approach.

## Challenges and Decisions
* **Environment Configuration:** A primary challenge was a `ModuleNotFoundError` for 'sklearn'. This was resolved by switching the VS Code kernel to match the Python environment where the libraries were installed (`~/.pyenv/versions/3.11.13/bin/python`).
* **Algorithm Clarification:** Initially, I investigated RNN as a Recurrent Neural Network, but clarified that for this lab, it refers to a Radius Neighbors Classifier, which was more appropriate for the static Wine dataset.
