# Veille 1 — Contexte du projet et fonctionnement général du mini-drone

## Objectif général
Le projet Over Sight vise à préparer un mini-drone de reconnaissance destiné à être envoyé dans une pièce pour en observer rapidement l’intérieur. Dans cette logique, le drone doit pouvoir se stabiliser, capter une image ou un flux vidéo, puis laisser la partie logicielle analyser ce qui est visible dans la scène. Le but n’est donc pas uniquement de “faire voler un drone”, mais de bâtir un système cohérent associant mobilité, perception et restitution d’information.

## Pourquoi cette veille est importante
Avant même de travailler sur les algorithmes de vision, il était nécessaire de comprendre :
- comment un quadricoptère se stabilise,
- quelles informations peuvent être remontées par ses capteurs,
- quelles sont les contraintes d’un vol en intérieur,
- pourquoi la partie vision peut être avancée indépendamment du matériel.

Cette compréhension permet d’éviter un prototype purement logiciel déconnecté de l’usage final.

## Architecture physique simplifiée
Un mini-drone de type quadricoptère repose sur quelques briques principales :
- un châssis léger,
- quatre moteurs et quatre hélices,
- des contrôleurs de vitesse,
- une batterie,
- un contrôleur de vol,
- une ou plusieurs caméras,
- éventuellement des capteurs additionnels.

Le contrôleur de vol est chargé de lire les capteurs et de corriger la vitesse des moteurs pour maintenir une attitude cohérente. Cette boucle est essentielle, car un lancement dans une pièce ne se fera pas toujours dans des conditions parfaitement contrôlées.

## Stabilisation et pilotage
Le maintien en vol s’appuie sur une boucle de correction continue. On retrouve généralement :
- le contrôle du roulis,
- le contrôle du tangage,
- le contrôle du lacet,
- et la gestion de la poussée globale.

Dans un environnement intérieur, le GPS n’est pas au centre du problème. La stabilité repose beaucoup plus sur les capteurs inertiels, la lecture rapide des perturbations et la capacité à corriger immédiatement la trajectoire.

## Lien direct avec Over Sight
Cette veille confirme une idée structurante pour le projet : la logique de vision peut être préparée avant l’intégration matérielle complète. Tant que le projet sait récupérer un flux caméra, il est possible d’avancer sur :
- la détection de personnes,
- la reconnaissance faciale,
- la lecture de gestes,
- la visualisation des résultats,
- et le benchmark de performance.

## Décision retenue
Le projet adopte donc une logique en deux temps :
1. prototypage logiciel sur un flux vidéo classique,
2. intégration progressive sur la plateforme volante finale.
