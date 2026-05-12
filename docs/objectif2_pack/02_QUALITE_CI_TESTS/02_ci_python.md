# CI Python proposée

## Objectif
Mettre en place une GitHub Action simple, fiable et compatible avec l’état actuel du repo.

## Ce que fait la CI
- checkout du dépôt,
- installation de Python,
- installation de quelques dépendances utiles à la vérification,
- exécution de Black en mode `--check`,
- exécution de Ruff,
- exécution des tests pytest.

## Pourquoi ne pas tout tester
Le dépôt contient des modules lourds et dépendants d’un environnement matériel.
Une CI trop ambitieuse risquerait de casser sans valeur pédagogique.

## Choix retenu
On vérifie prioritairement :
- les fichiers d’infrastructure Python,
- la cohérence minimale du dépôt,
- les helpers testables sans caméra ni GPU.
