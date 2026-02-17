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

L’ensemble de l’analyse est documenté dans le fichier `Projet_regression_Final.Rmd`.  
Le rapport complet est disponible au format HTML (`Projet_regression_Final.html`).

Le jeu de données au format CSV doit être téléchargé depuis la plateforme Kaggle (voir lien indiqué dans la section Jeu de données).  

Pour reproduire l’analyse, il est nécessaire de placer le fichier CSV dans le répertoire de travail, puis d’ouvrir le fichier `.Rmd` dans RStudio et de compiler le document.
Le logo UCA ainsi que le fichier de style CSS utilisés pour la mise en forme du rapport doivent également être téléchargés et placés dans le même répertoire.

---

## Remarque

Ce projet académique de master 1 illustre une démarche complète de modélisation statistique incluant estimation, validation des hypothèses, sélection de modèle et analyse critique des performances.  

