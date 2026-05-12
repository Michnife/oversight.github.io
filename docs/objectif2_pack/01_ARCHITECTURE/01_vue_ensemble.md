# Vue d’ensemble de l’architecture

## Organisation générale
Le dépôt est structuré en plusieurs zones complémentaires :

- `Poc/` : cœur des expérimentations IA et du launcher
- `documentation/` : documentation projet et livrables
- `website/` : site statique de présentation
- `interface/` : essais d’interface web complémentaires
- `benchmark_all.py` : benchmark centralisé
- `health_check.py` : contrôle rapide de l’environnement

## Idée d’architecture
L’architecture actuelle suit une logique modulaire :
- un ensemble de modules IA spécialisés,
- un point d’entrée utilisateur (launcher),
- des outils de benchmark / vérification,
- des documents et interfaces séparés.

## Intérêt
Cette séparation est adaptée à un projet étudiant évolutif :
- elle facilite les démos,
- elle simplifie la maintenance,
- elle permet de travailler en parallèle sur plusieurs briques.
