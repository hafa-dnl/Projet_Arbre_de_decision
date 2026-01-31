# Prédiction du montant engagé par l’État

## Objectif du projet
Ce projet vise à prédire le montant engagé par l’État pour le financement de projets publics à partir de caractéristiques administratives, économiques et territoriales des bénéficiaires.  
L’objectif est à la fois prédictif et explicatif, en s’appuyant sur des modèles d’arbres et d’ensembles d’arbres afin de conserver une bonne interprétabilité des résultats.

---

## Données
Les données utilisées proviennent de sources publiques et décrivent :
- les projets financés,
- le type de démarche associée,
- les caractéristiques des bénéficiaires (taille, forme juridique, activité),
- la localisation géographique des projets.

La variable cible est le **montant engagé**, qui a été transformée par une transformation logarithmique afin de réduire l’asymétrie de la distribution et l’influence des valeurs extrêmes.

---

## Méthodologie
Le projet suit une démarche classique de data science :

1. Analyse exploratoire des données et visualisations descriptives  
2. Nettoyage et sélection des variables pertinentes  
3. Encodage des variables catégorielles (One-Hot Encoding)  
4. Séparation des données en jeux d’entraînement et de test  
5. Comparaison de plusieurs modèles de régression :
   - Arbre de décision
   - Random Forest
   - Bagging
   - AdaBoost
   - Gradient Boosting
   - XGBoost
6. Sélection du modèle final sur la base des performances (MAE, RMSE et R², exprimés en euros)
7. Analyse de l’interprétabilité du modèle retenu

---

## Modèle final
Le **Gradient Boosting Regressor** a été retenu comme modèle final, car il offre le meilleur compromis global entre précision prédictive et capacité explicative.  
L’analyse des importances de variables montre que le montant engagé dépend principalement :
- du type de démarche financée,
- des caractéristiques structurelles du bénéficiaire (taille, forme juridique),
- et, dans une moindre mesure, de la localisation géographique.

---

## Résultats
Les performances des modèles ont été comparées à l’aide de métriques interprétables en euros :
- MAE (Mean Absolute Error),
- RMSE (Root Mean Squared Error),
- coefficient de détermination R².

Les méthodes de boosting se sont révélées globalement plus performantes que les modèles plus simples.

---

## Contenu du dépôt
- `notebooks/Fin.ipynb` : notebook principal du projet  
- `data/` : données utilisées (ou instructions pour les obtenir si non incluses)  
- `figures/` : graphiques générés pour l’analyse  
- `requirements.txt` : dépendances nécessaires à l’exécution du projet  

---

## Environnement
- **Python 3.10.11**
- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost

---