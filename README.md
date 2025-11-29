# Détection de fraude des réclamations en assurance automobile

## 📌 Aperçu du projet

La fraude en assurance automobile représente un enjeu financier majeur pour les assureurs. Un nombre important de réclamations inclut des informations falsifiées ou exagérées, ce qui augmente les coûts d’indemnisation et impacte les primes pour l’ensemble des assurés.\
Ce projet a pour objectif d’identifier les comportements frauduleux à partir des caractéristiques des réclamations et des assurés, en développant des modèles de classification capables de prédire si une réclamation est frauduleuse ou non.

------------------------------------------------------------------------

## 🎯 Objectifs

-   Analyser les variables les plus liées au comportement frauduleux
-   Construire des modèles d’apprentissage automatique pour classer les réclamations
-   Comparer les performances de plusieurs algorithmes
-   Proposer un outil d’aide à la décision permettant de soutenir le processus d’enquête
-   Traiter le déséquilibre des classes, caractéristique majeure dans ce type de problématique

------------------------------------------------------------------------

## 📊 Source des données

Le projet utilise un jeu de données public provenant de Kaggle : [Vehicle Claim Fraud Detection Dataset](https://www.kaggle.com/datasets/shivamb/vehicle-claim-fraud-detection){.uri}

Ce dataset contient des informations sur :

-   Les caractéristiques du véhicule
-   Les détails de la réclamation
-   Le profil de l’assuré
-   Une variable cible indiquant si la réclamation est frauduleuse

------------------------------------------------------------------------

## 🛠️ Méthodologie

### 🔹 Préparation des données

-   Nettoyage, transformation et encodage des variables catégorielles
-   Détection et traitement des valeurs manquantes
-   Analyse exploratoire des données (EDA)
-   Gestion du **déséquilibre des classes** via des techniques comme **SMOTE**

### 🔹 Modèles testés

Plusieurs modèles de classification ont été entraînés et comparés, notamment :

-   **Régression logistique**
-   **Random Forest**
-   **Gradient Boosting (LightGBM, XGBoost)**
-   **k-Nearest Neighbors**
-   **Support Vector Machine**

Les hyperparamètres ont été optimisés à l’aide de la **validation croisée**.

------------------------------------------------------------------------

## 📈 Évaluation des modèles

Les modèles ont été évalués avec des métriques adaptées aux données déséquilibrées :

-   **Accuracy**
-   **Précision**
-   **Rappel**
-   **F1-score**
-   **AUC**

La matrice de confusion a été utilisée pour visualiser les erreurs de classification.

Le meilleur modèle a obtenu une **précision élevée** tout en maintenant un bon équilibre entre détection de la fraude et limitation des faux positifs.

------------------------------------------------------------------------

## 🔍 Résultats principaux

-   Plusieurs variables (ex.: âge du véhicule, type de police, historique de réclamation) se sont révélées très discriminantes
-   Les modèles basés sur le **gradient boosting** ont offert les meilleures performances globales
-   Le projet démontre que l’apprentissage automatique peut assister efficacement les équipes antifraude

------------------------------------------------------------------------

## 🧾 Technologies utilisées

-   **Python** : prétraitement et modélisation
-   **Scikit-learn / LightGBM / XGBoost**
-   **SMOTE** pour le rééquilibrage des classes
-   **Visualisation** : matplotlib, seaborn
