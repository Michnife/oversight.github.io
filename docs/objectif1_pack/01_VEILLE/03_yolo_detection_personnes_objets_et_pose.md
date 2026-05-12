# Veille 3 — Détection de personnes, d’objets et de pose avec YOLO

## Problème traité
Le projet a besoin d’une brique capable de lire rapidement une scène et d’identifier au moins la présence de personnes. Une solution de détection généraliste était donc nécessaire.

## Pourquoi YOLO
YOLO a été retenu parce qu’il permet :
- une intégration rapide dans un prototype,
- des détections visuellement faciles à interpréter,
- un usage en temps réel raisonnable,
- une déclinaison possible vers la pose.

Cette solution couvre donc à la fois la détection classique d’objets et une lecture plus riche de la posture humaine.

## Intérêt dans le projet
La détection de personnes constitue le cœur du besoin fonctionnel. Détecter des objets est un bonus utile pour enrichir la scène, mais l’objectif principal reste la présence humaine. YOLO répond bien à cette hiérarchie :
- il permet d’identifier immédiatement une personne,
- il s’intègre bien avec des overlays visuels,
- il est réutilisable dans plusieurs scripts de test.

## Avantages observés
- Bon compromis global entre simplicité et efficacité.
- Intégration rapide dans les démos.
- Possibilité de décliner les tests en version “objets” et “pose”.

## Limites observées
- Le coût devient plus important lorsqu’on cumule plusieurs modules.
- Certaines détections peuvent être moins stables selon la scène.
- Une partie des classes détectables n’est pas indispensable pour l’objectif principal.

## Décision retenue
YOLO est retenu comme brique principale de lecture de scène, en particulier pour la détection de personnes et l’enrichissement de la perception avec la pose.
