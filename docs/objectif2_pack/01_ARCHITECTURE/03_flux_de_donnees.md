# Flux de données

## Flux simple du projet
1. Capture vidéo ou image
2. Envoi au module IA choisi
3. Inférence / détection / comparaison
4. Affichage ou restitution locale
5. Log, capture ou export éventuel

## Cas du benchmark
1. Le benchmark lance un module
2. Le module produit de la sortie standard et un résumé FPS
3. Le benchmark collecte :
   - FPS,
   - CPU,
   - RAM,
   - logs
4. Le benchmark produit :
   - un tableau,
   - un rapport markdown,
   - des exports JSON / CSV,
   - des graphes

## Intérêt pour l’objectif 2
Ce flux montre que le dépôt n’est pas uniquement un assemblage de scripts manuels :
il existe déjà une logique d’orchestration et de restitution.
