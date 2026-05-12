# Veille 2 — Capteurs, contraintes indoor et chaîne d’observation

## Capteurs utiles au scénario
Dans un contexte indoor, plusieurs familles de capteurs sont pertinentes :
- IMU pour mesurer les mouvements rapides,
- baromètre ou capteur équivalent pour certaines informations d’altitude,
- caméra ou optique grand angle pour la perception,
- capteurs de proximité ou distance selon les versions matérielles.

Cette veille n’a pas pour but de détailler un montage matériel complet, mais de comprendre quelles données seront réellement utiles à la chaîne d’observation.

## Pourquoi la caméra est centrale
Pour Over Sight, la caméra est la brique la plus importante du point de vue logiciel. C’est elle qui permet :
- de repérer une présence humaine,
- d’observer la posture,
- de reconnaître un visage dans un cadre de test,
- d’enrichir le retour visuel présenté à l’opérateur.

La caméra devient donc le point d’entrée de presque tous les prototypes réalisés à ce stade.

## Contraintes spécifiques au vol en intérieur
L’environnement intérieur impose plusieurs limites :
- espace réduit,
- faible recul sur certaines scènes,
- luminosité variable,
- obstacles proches,
- mouvements rapides du drone ou de la caméra.

Ces contraintes influencent directement la qualité du flux utilisé par les algorithmes. Une détection très correcte sur une image propre peut devenir bien plus instable dès que le cadrage se dégrade ou que la scène est plus chargée.

## Conséquences logicielles
Les prototypes logiciels doivent donc être pensés pour :
- accepter un flux imparfait,
- garder une certaine réactivité,
- éviter de cumuler des traitements trop lourds,
- rester lisibles visuellement pendant les démonstrations.

## Intérêt pour l’objectif 1
Cette veille relie les modules testés à un usage concret. Elle justifie le choix de travailler d’abord sur des briques de vision indépendantes, puis de mesurer leur coût, au lieu de chercher une intégration totale immédiate.
