# Maintenance Prédictive avec l’Intelligence Artificielle

## 🎯 Objectif du projet

Ce projet a pour but de développer des modèles de maintenance prédictive à l’aide de l’intelligence artificielle. À partir de données issues de capteurs et d’historiques de maintenance, le projet vise à :

1. Prédire si une machine tombera en panne dans les 14 prochains jours.
2. Identifier le composant susceptible d’être à l’origine de la panne.
3. Estimer le nombre de jours restants avant cette panne.

## ⚙️ Installation

Assurez-vous d’utiliser Python 3.10+.  
Installez les dépendances avec la commande suivante :

pip install -r requirements.txt

Dézipper le fichier dataset dans le même dossier que celui des notebooks.

## Liens utiles

- [Dataset Original sur Kaggle](https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance)
- [Table pour la classification binaire sur Kaggle](https://kaggle.com/datasets/ba9e1192415452c929a2267d73cb2c45e1fdd2395f67253082a2066335c37d13)
- [Table pour la classification multi-classe sur Kaggle](https://kaggle.com/datasets/1beb7bff38a64fb295cc01f86f211eff5e2f7b7440390559b75d544af7ff2be3)
- [Table pour la régression sur Kaggle](https://kaggle.com/datasets/1beb7bff38a64fb295cc01f86f211eff5e2f7b7440390559b75d544af7ff2be3)

## 🧠 Méthodologie

- Feature engineering : moyennes mobiles, deltas, interactions, cumul des erreurs, etc.
- Entraînement des modèles : LightGBM, XGBoost, Random Forest
- Optimisation par RandomizedSearchCV
- Validation croisée temporelle (TimeSeriesSplit)
- Évaluation : F1-score, matrice de confusion, MAE, RMSE

## 📊 Résultats

- Modèles de classification avec une précision supérieure à 95 %
- Modèle de régression avec une MAE d’environ 0.37 jours

## 👤 Auteur

Projet réalisé par Marie-Ange Dieng, étudiante en Intelligence Artificielle,  
dans le cadre d’un projet académique sur le développement durable.

---

# Predictive Maintenance with Artificial Intelligence (EN)

## 🎯 Project Goal

This project aims to develop AI models for predictive maintenance using sensor and maintenance data. The objectives are:

1. Predict if a machine will fail in the next 14 days.
2. Identify which component is likely to fail.
3. Estimate how many days remain before the failure occurs.


## ⚙️ Installation

Ensure you use Python 3.10+.  
Install dependencies with:

pip install -r requirements.txt

Unzip the dataset file in the same directory

## Links

- [Original dataset on Kaggle](https://www.kaggle.com/datasets/arnabbiswas1/microsoft-azure-predictive-maintenance)
- [Table for binary classification on Kaggle](https://kaggle.com/datasets/ba9e1192415452c929a2267d73cb2c45e1fdd2395f67253082a2066335c37d13)
- [Table for multi-class classification on Kaggle](https://kaggle.com/datasets/1beb7bff38a64fb295cc01f86f211eff5e2f7b7440390559b75d544af7ff2be3)
- [Table for regression on Kaggle](https://kaggle.com/datasets/1beb7bff38a64fb295cc01f86f211eff5e2f7b7440390559b75d544af7ff2be3)
  
## 🧠 Methodology

- Feature engineering: rolling averages, deltas, component interaction
- Models: LightGBM, XGBoost, Random Forest
- Hyperparameter tuning via RandomizedSearchCV
- TimeSeriesSplit cross-validation
- Evaluation: F1-score, confusion matrix, MAE, RMSE

## 📊 Results

- Classification accuracy above 95%
- Regression MAE ≈ 0.37 days

## 👤 Author

Project developed by Marie-Ange Dieng, Artificial Intelligence student,  
as part of an academic project on sustainability.
