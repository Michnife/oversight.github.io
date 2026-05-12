# Modules et responsabilités

## `Poc/launcher_gui.py`
Rôle :
- point d’entrée unique pour lancer les démos,
- affichage centralisé des sorties,
- accès direct au benchmark et au health check.

## `benchmark_all.py`
Rôle :
- exécuter plusieurs modules automatiquement,
- collecter les métriques,
- générer les rapports.

## `health_check.py`
Rôle :
- vérifier rapidement que l’environnement est exploitable,
- contrôler la présence de modules importants,
- tester la caméra.

## `Poc/IA Sources/*`
Rôle :
- héberger les briques de vision :
  - reconnaissance faciale,
  - face tracking,
  - détection d’objets,
  - pose,
  - gestes,
  - modes combinés.

## `documentation/`
Rôle :
- stocker les documents projet et les livrables.

