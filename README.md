# Analyse de données

Ce projet s’inscrit dans le cadre de mon master en Data Science et consiste en une analyse approfondie d’un jeu de données regroupant des caractéristiques chimiques de différents vins, associées à des notes de qualité. L’objectif est de mettre en œuvre des méthodes d’exploration, de réduction de dimensionnalité et de clustering afin de mieux comprendre la structure et les patterns présents dans les données.

L’analyse débute par l’importation et l’exploration du dataset (1143 observations, 12 variables), avec une description statistique des principaux indicateurs (acides, sucres résiduels, chlorures, etc.).

Une Analyse en Composantes Principales (ACP) est réalisée afin de visualiser la variance expliquée par chaque axe principal. Ce travail est illustré par un scree plot et la comparaison avec la variance moyenne, mettant en lumière les dimensions les plus pertinentes pour la structure des vins.

En complément, un clustering hiérarchique selon la méthode de Ward est mis en œuvre, permettant de segmenter les échantillons en 20 groupes. L’inertie inter-groupe rapportée à l’inertie totale atteste de la pertinence des clusters formés.

Un heatmap combiné à l’arbre hiérarchique permet de visualiser les regroupements découverts et d’identifier des clusters singuliers, notamment grâce à la représentation transposée des données et l’utilisation d’une palette de couleurs contrastée.

Ce projet met en avant l’usage d’outils statistiques avancés pour l’exploration, la visualisation et l’interprétation de données multivariées, appliqués à une problématique concrète d’œnologie. Le code, reproductible sous R, illustre chaque étape, des premiers traitements au rendu graphique des résultats.
