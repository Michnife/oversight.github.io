# Méthode de test et logique du benchmark

## Objectif
Le benchmark vise à répondre à une question simple mais décisive pour le projet : quelles briques de vision sont les plus pertinentes à conserver et lesquelles deviennent trop coûteuses lorsqu’elles sont combinées ?

## Modules testés
Les modules comparés couvrent les principales briques du projet :
- Face Tracking,
- Face Recognition,
- YOLO Objects,
- YOLO Pose,
- Shape + Face,
- Combined Recognition,
- Hand Recognition.

## Indicateurs suivis
Les mesures produites par le benchmark sont :
- FPS moyen,
- FPS minimum,
- FPS maximum,
- charge CPU moyenne,
- consommation mémoire moyenne.

Ces indicateurs suffisent à produire une première lecture comparative cohérente.

## Lecture prudente des données
Certaines valeurs maximales sont clairement des pics non représentatifs. Elles ne doivent pas être lues comme une performance réelle stable, mais comme une anomalie ponctuelle liée au mode de mesure ou à une phase transitoire du pipeline.

C’est pour cette raison que l’analyse finale privilégie :
- le FPS moyen,
- le comportement général,
- le coût CPU,
- et surtout le coût mémoire.

## Intérêt pour l’objectif 1
Cette méthode permet de passer d’un prototype “qui marche” à une expérimentation mesurée, donc à une base de décision technique défendable dans un rendu académique.
