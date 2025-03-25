# mlq2project
ML Quarter 2 Project - Adaptive Decision Trees with Dynamic Depth Pruning for Uneven Data Distributions

Abstract:
Many machine learning datasets exhibit imbalanced distributions, with dense and sparse regions that challenge traditional decision tree models. Conventional decision trees tend to overfit in dense areas while underfitting in sparse regions, limiting their generalizability. This paper introduces an adaptive decision tree algorithm that dynamically adjusts its depth based on local data density. By incorporating a density-based pruning mechanism inspired by K-Nearest Neighbors (KNN), the proposed method prevents excessive branching in sparse regions while allowing deeper splits in dense areas, striking a balance between interpretability and adaptability. Experiments on a traffic accident prediction dataset demonstrate that our model achieves higher generalization performance compared to standard decision trees and pruned variants, with a 20% improvement in test accuracy and a 0.35 improvement in macro-averaged precision, recall, and F1-Score. These findings suggest that density-aware decision trees offer a promising approach for handling uneven data distributions in domains such as healthcare, finance, and autonomous systems.

Steps to run our code:
1. Download our repository
2. Use our preprocessed and discretized ```Traffic_Accident_Prediction.csv``` in the content folder
   a. This file has been preprocessed from the original ```Traffic_Accident_Prediction_InitialDataset.csv``` in the content folder by discretizing numerical attributes, removing and replacing missing values, and conducting a stratified train-test split (70-30 ratio) to preserve class distributions. All of the preprocessing steps are detailed in the "Dataset and Features" section of our report.
3. Run each of the individual cells in the python notebook file ```RohithYelisetty,AaravGupta_Q2Project.ipynb``` in order to run a default (control) decision tree on the traffic data in addition to our adaptive one on the data.
