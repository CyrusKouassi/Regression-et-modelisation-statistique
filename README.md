# Modélisation statistique et analyse de régression sous R

## Objectif

Ce projet académique, réalisé dans le cadre d’un Master en Mathématiques Appliquées et Statistiques, vise à identifier les facteurs marketing influençant le volume des ventes d’un produit.

L’étude cherche à déterminer quels canaux publicitaires contribuent le plus efficacement à l’augmentation des ventes, tout en garantissant la validité statistique des modèles estimés.

---

## Jeu de données

Le dataset contient 992 observations et 8 variables quantitatives représentant :

- Les ventes hebdomadaires
- Les dépenses publicitaires (TV, radio, en ligne, magasin)
- Les remises appliquées
- Le prix du produit
- Le taux de rupture de stock

Source des données : Kaggle  
https://www.kaggle.com/datasets/ai0909/sales-data-for-company-product

---

## Démarche méthodologique

Le projet suit une approche rigoureuse en plusieurs étapes :

- Analyse exploratoire et étude des corrélations  
- Analyse en Composantes Principales (ACP) comme prétraitement  
- Estimation d’un modèle de régression linéaire (MCO)  
- Vérification des hypothèses (normalité, homoscédasticité, indépendance)  
- Analyse des observations influentes (DFBETAS, DFFITS)  
- Étude de la multicolinéarité (VIF, tolérance)  
- Sélection de variables via AIC et BIC  
- Comparaison avec des Modèles Linéaires Généralisés (GLM)  
- Test de Vuong pour comparaison de modèles  

---

## Résultats principaux

Les critères AIC et BIC convergent vers un modèle simplifié excluant les variables Publicités_Radio et Dépenses_En_Ligne.

La suppression des observations influentes améliore significativement les critères d’information.

La comparaison LM vs GLM montre que le modèle linéaire classique reste le plus performant dans ce contexte.

---

## Technologies utilisées

- R
- RMarkdown
- Méthodes de régression linéaire (MCO)
- Modèles Linéaires Généralisés (GLM)
- Sélection de modèles (AIC, BIC)
- Diagnostics statistiques

---

## Reproductibilité

L’analyse complète est disponible dans :

- `Projet_regression_Final.Rmd`
- `Projet_regression_Final.html`

Le projet peut être reproduit en ouvrant le fichier `.Rmd` dans RStudio et en compilant le document.

---

## Remarque

Ce projet illustre une démarche complète de modélisation statistique incluant estimation, validation des hypothèses, sélection de modèle et analyse critique des performances.  

Il met en évidence des compétences en statistique appliquée, en diagnostic de modèles et en interprétation rigoureuse des résultats.
