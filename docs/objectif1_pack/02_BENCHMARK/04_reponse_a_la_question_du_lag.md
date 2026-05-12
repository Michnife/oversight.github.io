# Réponse claire à la question du lag

## Question
Est-ce que plusieurs algorithmes exécutés en même temps dégradent les performances ?

## Réponse
Oui. Les tests montrent que les modules combinés coûtent significativement plus cher que les briques unitaires.

## Ce que montrent les mesures
- Les modules YOLO unitaires restent globalement fluides.
- Face Recognition reste correct, mais plus coûteux qu’un tracking simple.
- Shape + Face perd en fluidité par rapport aux briques exécutées séparément.
- Combined Recognition représente le cas le plus parlant de dégradation lorsqu’on cumule plusieurs traitements.

## Interprétation
Le lag n’apparaît pas comme un simple ressenti visuel : il se traduit par une baisse mesurable du FPS moyen et par une hausse de la mémoire utilisée. Le benchmark confirme donc que le coût des traitements cumulés doit être pris en compte dans les choix du projet.

## Conclusion exploitable
Pour le scénario principal, il vaut mieux :
- garder une brique centrale robuste,
- n’ajouter que les enrichissements nécessaires,
- éviter de tout activer en continu dans une même boucle de traitement.
