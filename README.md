🇫🇷 README – Maintenance Prédictive avec l’Intelligence Artificielle
🎯 Objectif du projet
Ce projet a pour but de mettre en œuvre des modèles de maintenance prédictive à l’aide de l’intelligence artificielle. À partir de données industrielles simulées, nous cherchons à :

Prédire si une machine tombera en panne dans les 14 prochains jours.

Identifier quel composant est susceptible d'être en cause.

Estimer le nombre de jours restants avant cette panne.

📁 Structure du dépôt
/
├── 1_data_cleaning.ipynb              # Nettoyage et création des features
├── 2_prediction_panne_14d.ipynb       # Modélisation classification binaire (panne ou non)
├── 3_prediction-composant-panne.ipynb # Modélisation classification multi-classes (composant)
├── 4_prediction-tbf.ipynb             # Modélisation régression (temps avant panne)
├── requirements.txt                   # Bibliothèques Python nécessaires
├── dataset/
│   ├── PdM_telemetry.csv
│   ├── PdM_errors.csv
│   ├── PdM_maint.csv
│   ├── PdM_failures.csv
│   ├── PdM_machines.csv
│   └── dataset_cleaned/
│       ├── df_machine_failure.csv     # Pour modèle 1
│       ├── df_comp_failure.csv        # Pour modèle 2
│       ├── df_time_failure.csv        # Pour modèle 3

⚙️ Prérequis
Python 3.10+

Jupyter Notebook

Scikit-learn, LightGBM, XGBoost, Pandas, Numpy, etc.

Installez les dépendances avec :

pip install -r requirements.txt

🧠 Méthodologie
Feature engineering (variables dérivées, moyennes mobiles, deltas, etc.)

Entraînement des modèles avec optimisation d’hyperparamètres via RandomizedSearchCV

Évaluation : F1-score, matrice de confusion, MAE/RMSE (régression)

📊 Résultats
Précision des modèles de classification supérieure à 95 % avec LightGBM & XGBoost

Estimation du temps avant panne avec MAE ≈ 0.37 jours

🔍 Auteur
Projet réalisé par Marie-Ange Dieng, étudiante en Intelligence Artificielle.
Encadré dans le cadre d’un projet académique sur le développement durable.


🇬🇧 README – Predictive Maintenance with Artificial Intelligence
🎯 Project Goal
This project implements predictive maintenance models using artificial intelligence. From industrial time series data, the goal is to:

Predict whether a machine will fail within the next 14 days.

Identify which component will likely fail.

Estimate how many days remain before the failure.

📁 Repository Structure

/
├── 1_data_cleaning.ipynb              # Data cleaning and feature creation
├── 2_prediction_panne_14d.ipynb       # Binary classification model (failure or not)
├── 3_prediction-composant-panne.ipynb # Multi-class classification model (component)
├── 4_prediction-tbf.ipynb             # Regression model (time before failure)
├── requirements.txt                   # Required Python packages
├── dataset/
│   ├── PdM_telemetry.csv
│   ├── PdM_errors.csv
│   ├── PdM_maint.csv
│   ├── PdM_failures.csv
│   ├── PdM_machines.csv
│   └── dataset_cleaned/
│       ├── df_machine_failure.csv     # Used for model 1
│       ├── df_comp_failure.csv        # Used for model 2
│       ├── df_time_failure.csv        # Used for model 3

⚙️ Requirements
Python 3.10+

Jupyter Notebook

Scikit-learn, LightGBM, CatBoost, Pandas, Numpy, etc.

Install dependencies with:

pip install -r requirements.txt

🧠 Methodology
Advanced feature engineering (rolling windows, deltas, aggregations)

Model training with RandomizedSearchCV hyperparameter tuning

Evaluation metrics: F1-score, confusion matrix, MAE/RMSE (for regression)

📊 Results
Classification models achieve over 95% accuracy

Failure time regression with MAE ≈ 0.37 days

🔍 Author
Project developed by Marie-Ange Dieng, Artificial Intelligence student.
This work is part of an academic initiative focused on sustainable development.
