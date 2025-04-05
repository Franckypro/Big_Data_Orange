# Big_Data_Orange
Analyse Prédictive de la Qualité des Oranges 🍊

📌 Description
Ce projet utilise PySpark, Pandas, Matplotlib, Seaborn et scikit-learn pour effectuer une analyse exploratoire et une prédiction de la qualité des oranges à partir d’un ensemble de données contenant diverses caractéristiques (taille, poids, acidité, douceur, couleur, etc.). Il s'agit d'un workflow complet allant du prétraitement des données jusqu’à l'entraînement d’un modèle de régression avec GBTRegressor.

📦 Prérequis
Les bibliothèques nécessaires sont :

pip install findspark

pip install xgboost

pip install scikit-learn

pip install pyspark

⚙️ Étapes de traitement
Initialisation de Spark :

Création d’une session Spark avec SparkSession

Détection du nombre de cœurs de calcul disponibles

Chargement des données :

Lecture du fichier orange.csv

Vérification de la structure, des valeurs nulles et des doublons

Analyse exploratoire :

Affichage de la distribution des variables

Utilisation de boxplot et histplot pour détecter les outliers

Visualisation par nuage de points

Prétraitement des données :

Encodage des variables catégorielles (Color, Variety, Blemishes)

Nettoyage et renommage des colonnes

Standardisation des données numériques avec StandardScaler

Préparation des features :

Construction du vecteur de features avec VectorAssembler

Séparation du dataset en ensembles d’entraînement et de test

Modélisation :

Entraînement d’un modèle de régression GBTRegressor (Gradient Boosted Tree)

Évaluation avec différentes métriques (R², RMSE, MAE)

Optimisation des hyperparamètres avec ParamGridBuilder et CrossValidator


📊 Technologies utilisées
Apache Spark / PySpark

Pandas & PySpark.Pandas

Matplotlib & Seaborn

Scikit-learn

XGBoost


📁 Données
Les données utilisées dans ce projet se trouvent dans le fichier orange.csv, qui contient les colonnes suivantes :

Size (cm), Weight (g), Brix (Sweetness), pH (Acidity)

Softness (1-5), HarvestTime (days), Ripeness (1-5)

Color, Variety, Blemishes (Y/N), Quality (1-5)


🎯 Objectif
L'objectif principal est de prédire la qualité (Quality (1-5)) d’une orange à partir de ses caractéristiques physiques et chimiques en utilisant un modèle supervisé de régression.

✍️ Auteur
Fouejio Francky Joël
