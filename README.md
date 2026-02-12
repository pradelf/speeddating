# Bloc 2

Ce projet est sur Github à l'url : [https://github.com/pradelf/speeddating](https://github.com/pradelf/speeddating)

[TOC]

# Contexte

Ce projet est à réaliser pour valider partiellement la certification _Data Science - Fullstack : Certification RNCP35288 CDSD_ avec le bloc 2.

**Bloc 2 - Analyse exploratoire, descriptive et inférentielle de données**

- Traiter des bases de données grâce à des analyses statistiques descriptives et inférentielles via des librairies de programmation comme Numpy ou Pandas, pour les organiser et les nettoyer afin de les normaliser par rapport à la population étudiée.
- Effectuer des analyses univariées et multivariées sur des bases de données structurées afin de préciser des relations entre plusieurs variables et d'établir des liens statistiques entre elles.
- Optimiser les analyses statistiques grâce au traitement parallélisé via l'utilisation d'outils comme Spark pour accélérer le temps de calcul d'un ordinateur afin de pouvoir analyser des volumes de données massifs (Big Data)
- Présenter le résultat d'une analyse statistique de données structurées, massives ou non, grâce à des librairies de programmation comme Plotly ou Matplotlib pour synthétiser ce résultat devant un public profane afin de faciliter la prise de décisions et appuyer leurs déclinaisons opérationnelles

Le fichier brut énoncé du porjet est dans le notebook [01-Speed_Dating.ipynb](./01-Speed_Dating.ipynb) et mon rendu de projet est dans le notebook [01-Speed_Dating_FPr.ipynb](./01-Speed_Dating_FPr.ipynb).  

Pour installer ce projet, il faut se reporter à la description [INSTALL.md](./INSTALL.md)

# Speed Dating avec Tinder

![Tinder](https://full-stack-assets.s3.eu-west-3.amazonaws.com/M03-EDA/Tinder-Symbole.png)

## Description de la société 📇

<a href="https://tinder.com/" target="_blank">Tinder</a> est une **application de rencontres en ligne et de réseautage géosocial**.
Sur Tinder, les utilisateurs **“swipent à droite”** pour indiquer qu’ils aiment un profil, ou **“swipent à gauche”** pour passer — chaque profil comprenant **des photos, une courte biographie et une liste d’intérêts**.

L’application a été **lancée en 2012** par **Sean Rad**, lors d’un **hackathon organisé au sein de l’incubateur Hatch Labs**, à **West Hollywood (Californie)**.

## Étude Speed Dating — Analyse exploratoire et modélisation

Ce notebook présente une analyse académique du jeu de données _Speed Dating_, avec une démarche structurée : contexte, objectifs, préparation des données, EDA, modélisation et discussion des limites.

### Projet 🚧

L’équipe marketing a besoin d’aide pour un nouveau projet.
Elle observe une **diminution du nombre de matchs** et cherche à comprendre **ce qui favorise l’attirance mutuelle entre deux individus**.

Pour ce faire, Tinder a organisé une **expérience de speed dating** : les participants ont dû fournir à l’entreprise de **nombreuses informations personnelles**, susceptibles de **refléter leur futur profil sur l’application**.

Tinder a ensuite **collecté les données issues de cette expérience**.
Chaque ligne du jeu de données correspond à **un rendez-vous entre deux personnes** et indique si chacune d’elles a **secrètement exprimé le souhait de revoir l’autre** pour un second rendez-vous.

### Projet — Contexte et objectifs 🚧

**Objectif général :** identifier les déterminants d'une seconde rencontre.

**Objectifs spécifiques :**

- documenter la structure des données (variables, valeurs manquantes, distributions) ;
- explorer les corrélations et éventuelles non‑linéarités ;
- proposer une première base de modèles prédictifs et d'interprétabilité (coefficients, importances).

Le rendu du projet est dans le notebook : [01-Speed_Dating_FPr.ipynb](01-Speed_Dating_FPr.ipynb)

## Conclusion de l'étude

Le taux de match est faible (~16 %), et l’attractivité perçue apparaît comme le facteur dominant (surtout chez les hommes), tandis que les centres d’intérêt sont faiblement corrélés et que les hommes subissent davantage de rejets.
En effet, malgré des données très incomplètes (dataswamp) et des résultats non causaux, cette étude exploratoire montre que l’affection mutuelle prime largement sur les critères objectifs.
On en tire donc des considérations plutôt descriptives même en s'appuyant sur des données chiffrées.  
Rien n'est rééllement tranché, on est plus sur de la tendance pour comprendre ce qui amène à un deuxième rendez-vous.
Le deuxième rendez-vous tourne autour du concept d'amabilité assez vague chez l'humain :

- plutôt une recherche de fun et attractivité chez les femmes pour les hommes
- et plutôt une recherche de sincérité et d'intelligence chez les hommes pour les femmes.  

Ce n’est ni purement une question de centres d’intérêt, ni de loisirs, ni même totalement d’attractivité ou d’intelligence.
En réalité, tout repose sur le concept assez vague de degré d’affection que l’autre vous porte et qui semble un subtil cocktail à base de fun, attractivité, sincérité ét intelligence sans pour autant qu'il ait des dosages exacts.
Il n’existe donc pas de critère unique qui rende quelqu’un “aimable” pour susciter un deuxième rendez-vous.  
On reste dans le domaine de l'alchimie pour comprendre l'initiation de l'amour voir le coup de foudre.
Ce qui compte avant tout, c’est le degré d’affection mutuelle, plus que les caractéristiques objectives ou déclarées.  
Les données ne font donc pas tout pour comprendre l'humain.
La dissymétrie sur les caractéristiques qui rendent l'autre attirable entre les hommes et les femmes pousse à essayer de rechercher la mise en avant de critères « communs » d’affection entre homme et femme lors des dtaes.
Par exemple, l'humour pourrait activer l'aspect fun connectable à l'intelligence.
  
En cela c'est rassurant car il y a peu de risque que les machines s'appui sur l'intelligence artificielle pour bien cerner le comportement amoureux humain si même les humains n'y arrivent pas.
