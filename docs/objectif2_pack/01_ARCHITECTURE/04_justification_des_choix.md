# Justification des choix

## Pourquoi garder une architecture modulaire
Le projet contient plusieurs briques IA de nature différente.
Les séparer permet :
- d’isoler les bugs,
- de comparer les performances,
- de lancer uniquement ce qui est utile,
- d’éviter une dépendance forte entre tous les modules.

## Pourquoi garder un launcher
Le launcher centralise la démonstration.
Dans un projet EIP, c’est utile pour :
- faciliter les tests,
- montrer les fonctionnalités au jury,
- réduire le temps d’accès aux démos.

## Pourquoi ajouter une CI
La CI montre qu’il existe une vérification automatique.
Même minimale, elle apporte :
- une preuve de rigueur,
- une meilleure reproductibilité,
- une base pour sécuriser les futures évolutions.

## Pourquoi ajouter des tests
Les tests proposés ici ne prétendent pas couvrir toute la vision.
Ils servent surtout à prouver :
- qu’un module critique peut être validé automatiquement,
- qu’une partie de l’infrastructure projet est testée,
- que le projet n’est pas uniquement vérifié à la main.
