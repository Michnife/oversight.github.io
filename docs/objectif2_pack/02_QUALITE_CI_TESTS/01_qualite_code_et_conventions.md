# Qualité de code et conventions

## Outils retenus
- **Black** : formatage automatique
- **Ruff** : linting léger et rapide
- **pytest** : base de tests automatisés

## Pourquoi ces outils
Ils sont simples à mettre en place et adaptés à un projet Python multi-fichiers.

## Convention proposée
- nommage clair des fichiers,
- fonctions courtes quand possible,
- imports regroupés en haut des fichiers,
- chemins calculés avec `pathlib`,
- gestion d’erreurs explicite pour les scripts critiques.

## Ce que cela apporte
- code plus cohérent,
- relecture plus simple,
- base exploitable pour travailler à plusieurs.
