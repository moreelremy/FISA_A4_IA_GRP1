# FISA_A3_IA_GRP1 - IA for HumanForYou

## Contexte

Ce projet s'inscrit dans le bloc **Intelligence artificielle (machine learning)**.  
L'entreprise **HumanForYou**, une société pharmaceutique basée en Inde comptant environ **4000 employés**, fait face à un **taux de rotation annuel d'environ 15 %**.

L'objectif du projet est d'exploiter des données RH pour :

- identifier les facteurs qui influencent le départ des employés,
- construire des modèles de **prédiction de l’attrition**,
- proposer des **pistes d’amélioration concrètes** pour réduire ce turnover.

---

## Problématique

Le turnover élevé entraîne plusieurs impacts négatifs pour l’entreprise :

- ralentissement des projets,
- dégradation de l’image auprès des clients et partenaires,
- charge importante sur les ressources humaines,
- perte de temps liée au recrutement, à l’intégration et à la formation des nouveaux employés.

Le besoin métier est donc double :

1. **comprendre** pourquoi les employés quittent l’entreprise,
2. **anticiper** les départs grâce à des modèles de machine learning.

---

## Objectifs du projet

- Réaliser une **analyse exploratoire** des données RH.
- Préparer, nettoyer et consolider plusieurs sources de données.
- Identifier les variables les plus liées à l’attrition.
- Construire et comparer plusieurs modèles de **classification supervisée**.
- Évaluer les performances des modèles avec des métriques adaptées.
- Justifier le choix du modèle final selon le besoin client.
- Formuler des recommandations métier basées sur les résultats.

---

## Données fournies

Les données sont anonymisées et reliées par `EmployeeID`.

### 1. Données RH principales — `general_data.csv`

Ce fichier contient les informations générales des employés, notamment :

- `Age`
- `Attrition`
- `BusinessTravel`
- `DistanceFromHome`
- `Education`
- `EducationField`
- `EmployeeCount`
- `EmployeeID`
- `Gender`
- `JobLevel`
- `JobRole`
- `MaritalStatus`
- `MonthlyIncome`
- `NumCompaniesWorked`
- `Over18`
- `PercentSalaryHike`
- `StandardHours`
- `StockOptionLevel`
- `TotalWorkingYears`
- `TrainingTimesLastYear`
- `YearsAtCompany`
- `YearsSinceLastPromotion`
- `YearsWithCurrentManager`

### 2. Évaluation manager — `manager_survey_data.csv`

Dernière évaluation réalisée en février 2015 :

- `EmployeeID`
- `JobInvolvement`
- `PerformanceRating`

### 3. Enquête qualité de vie au travail — `employee_survey_data.csv`

Résultats d’une enquête RH menée en juin 2015 :

- `EnvironmentSatisfaction`
- `JobSatisfaction`
- `WorkLifeBalance`

Certaines réponses peuvent être absentes et codées par `NA`.

### 4. Horaires de travail — `in_out_time.zip`

Deux fichiers contiennent les horaires d’entrée et de sortie des employés entre le **1er janvier 2015** et le **31 décembre 2015**.

Ces données permettent d’extraire des indicateurs complémentaires sur les habitudes de travail.

---

## Approche envisagée

Le projet suit une démarche classique de data science :

1. **Compréhension du besoin métier**
2. **Exploration et nettoyage des données**
3. **Fusion et transformation des différentes sources**
4. **Création de variables pertinentes**
5. **Analyse des facteurs explicatifs de l’attrition**
6. **Entraînement de modèles de classification**
7. **Évaluation et amélioration des performances**
8. **Interprétation des résultats et recommandations**

---

## Enjeux techniques

Ce projet met en jeu plusieurs problématiques courantes en machine learning :

- gestion des valeurs manquantes,
- encodage de variables catégorielles,
- sélection et interprétation des variables,
- déséquilibre potentiel de la cible `Attrition`,
- comparaison de plusieurs algorithmes,
- interprétation métier des résultats.

---

## Livrables attendus

### 1. Livrable éthique

Un document présentant une démarche éthique appliquée au projet, en tenant compte notamment des 7 exigences recommandées par la Commission Européenne :

- respect de l’autonomie humaine,
- robustesse technique et sécurité,
- confidentialité et gouvernance des données,
- transparence,
- diversité, non-discrimination et équité,
- bien-être environnemental et sociétal,
- responsabilité.

### 2. Bibliographie

Un document référençant les sources académiques, techniques, méthodologiques et éthiques utilisées pour orienter et justifier le travail.

### 3. Présentation finale

Une soutenance de 20 minutes accompagnée d’un notebook Jupyter présentant :

- la préparation des données,
- les choix de modélisation,
- les métriques utilisées,
- les tests réalisés,
- l’amélioration des modèles,
- le choix final retenu,
- les recommandations proposées au client.

---

## Source des données

Les données du projet sont issues d’un jeu de données généré à partir de cette étude Kaggle :

**HR Analytics Case Study**  
https://www.kaggle.com/vjchoudhary7/hr-analytics-case-study

---

## Finalité

L’objectif final n’est pas seulement de construire un bon modèle prédictif, mais aussi de fournir à HumanForYou des **leviers d’action concrets** pour améliorer la fidélisation des employés et réduire durablement le turnover.
