# Analyse de données multivariées, première partie

Ce projet s’inscrit dans le cadre de mon master en Data Science et consiste en une analyse approfondie d’un jeu de données regroupant des caractéristiques chimiques de différents vins, associées à des notes de qualité. L’objectif est de mettre en œuvre des méthodes d’exploration, de réduction de dimensionnalité et de clustering afin de mieux comprendre la structure et les patterns présents dans les données.

L’analyse débute par l’importation et l’exploration du dataset (1143 observations, 12 variables), avec une description statistique des principaux indicateurs (acides, sucres résiduels, chlorures, etc.).

Une Analyse en Composantes Principales (ACP) est réalisée afin de visualiser la variance expliquée par chaque axe principal. Ce travail est illustré par un scree plot et la comparaison avec la variance moyenne, mettant en lumière les dimensions les plus pertinentes pour la structure des vins.

En complément, un clustering hiérarchique selon la méthode de Ward est mis en œuvre, permettant de segmenter les échantillons en 20 groupes. L’inertie inter-groupe rapportée à l’inertie totale atteste de la pertinence des clusters formés.

Un heatmap combiné à l’arbre hiérarchique permet de visualiser les regroupements découverts et d’identifier des clusters singuliers, notamment grâce à la représentation transposée des données et l’utilisation d’une palette de couleurs contrastée.

Ce projet met en avant l’usage d’outils statistiques avancés pour l’exploration, la visualisation et l’interprétation de données multivariées, appliqués à une problématique concrète d’œnologie. Le code, reproductible sous R, illustre chaque étape, des premiers traitements au rendu graphique des résultats.


# Analyse de données multivariées, deuxième partie

Dans la continuité du projet précédent sur les vins, cette seconde étude se concentre sur un jeu de données génétiques recueilli auprès de 50 patientes atteintes d’un cancer de l’ovaire. L’objectif vise à exploiter des techniques d’analyse multivariée pour dégager des profils génétiques distincts susceptibles d’avoir une valeur clinique ou biologique.

L’approche méthodologique s’est construite autour de plusieurs axes complémentaires :

Prétraitement des données
Les données brutes et standardisées ont été comparées, la standardisation ayant été privilégiée pour une meilleure interprétabilité des résultats.
Réduction de la dimensionnalité
L’Analyse en Composantes Principales (ACP) a permis de concentrer l’information sur un nombre restreint d’axes, facilitant ainsi la visualisation de la structure sous-jacente des profils ADN. La première composante explique la majeure partie de la variance, révélant l’existence de grandes tendances de variation génétique parmi les patientes.
Segmentation et exploration des groupes
En mobilisant les algorithmes de K-means et de classification hiérarchique ascendante (CAH, méthode ward.D2), l’analyse statistique a permis de révéler des sous-groupes d’individus partageant des anomalies génétiques similaires. La cohérence des clusters identifiés par différentes méthodes conforte la solidité des résultats.
Cette étude met en lumière la puissance des approches combinant réduction de dimensionnalité et clustering pour extraire de l’information pertinente dans des jeux de données à très grande dimension, comme ici avec 10 000 variables pour seulement 50 observations.

Elle ouvre également la réflexion sur l’importance de confronter les résultats issus de la modélisation statistique à des critères cliniques et biologiques dans une perspective de médecine personnalisée, par exemple en étudiant le lien entre profils génétiques, évolution de la maladie et réponse aux traitements.

Chaque étape analytique, de la préparation initiale à la visualisation des résultats, est rigoureusement documentée et reproductible via des scripts R disponibles dans ce dépôt.
