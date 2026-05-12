# Architecture technique — Objectif 2

## 1. Vue générale
Le dépôt est organisé autour de plusieurs blocs :

- `Poc/` : cœur des scripts, expérimentations IA et outil de démonstration
- `documentation/` : documents projet et livrables
- `website/` : site statique de présentation
- `interface/` : interface web complémentaire
- scripts racine comme `benchmark_all.py` et `health_check.py`

## 2. Rôle des composants
### 2.1 Poc
`Poc` contient :
- les modules IA dans `IA Sources/`
- le launcher graphique
- un point d’entrée Python
- les dépendances du sous-projet

### 2.2 Benchmark
`benchmark_all.py` sert d’orchestrateur :
- lance plusieurs modules
- collecte les métriques
- écrit les rapports

### 2.3 Health check
`health_check.py` sert à vérifier rapidement l’état minimal de l’environnement.

### 2.4 Website
Le site statique présente :
- le projet,
- les livrables,
- les captures,
- les documents utiles.

## 3. Flux principal
1. lancement d’un module via le launcher ou une commande directe,
2. capture / traitement / affichage,
3. sortie standard et éventuels logs,
4. benchmark possible via le runner principal.

## 4. Justification
Cette architecture modulaire est adaptée à un projet EIP évolutif :
- elle facilite la démonstration,
- elle rend les modules plus lisibles,
- elle permet d’ajouter une CI et des tests ciblés.

## 5. Limites actuelles
- certains modules restent dépendants du matériel,
- les tests automatiques ne couvrent pas la totalité des traitements IA,
- l’infrastructure de qualité est encore en cours de formalisation.

## 6. Évolution visée
L’objectif 2 vise à faire passer le dépôt :
- d’un prototype fonctionnel,
- à un dépôt mieux structuré, mieux documenté et vérifiable automatiquement.
