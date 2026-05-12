# Tests retenus

## Principe
Le projet contient beaucoup de modules graphiques et dépendants du matériel.
Pour l’objectif 2, il est plus pertinent de tester des éléments fiables et non interactifs.

## Tests proposés
1. **Benchmark helpers**
   - vérifie `_safe_slug`
   - vérifie l’analyse d’une ligne `FPS_SUMMARY`

2. **Health check**
   - vérifie `has_module`
   - prouve qu’un bout d’infrastructure critique est testable

3. **Repo structure**
   - vérifie la présence de fichiers clés du dépôt

## Pourquoi ces tests sont pertinents
Ils montrent une démarche de validation automatique sans exiger un environnement complet de vision.
