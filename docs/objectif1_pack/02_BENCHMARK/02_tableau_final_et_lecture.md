# Tableau final et lecture synthétique

| IA | FPS moyen | FPS min | FPS max | CPU moyen | RAM moyenne (MB) | Lecture | Décision |
|---|---:|---:|---:|---:|---:|---|---|
| Face Tracking | 19.78 | 3.01 | 23.83 | 862.28 | 87.21 | Module simple, utile pour une détection rapide et légère d’un visage sans logique d’identification. | Conservé comme solution simple et de secours. |
| Face Recognition | 21.93 | 3.27 | 115.41 | 165.67 | 479.29 | Pipeline plus coûteux qu’un simple tracking mais pertinent pour les démonstrations d’identification. | Conservé pour les scénarios ciblés d’identification. |
| YOLO Objects | 28.04 | 2.60 | 57.31 | 575.32 | 569.02 | Très bon compromis pour détecter rapidement des personnes et objets dans une scène. | Conservé comme brique centrale de détection. |
| YOLO Pose | 28.69 | 2.63 | 50.09 | 588.52 | 560.95 | Bonne fluidité et richesse d’information; intéressant pour enrichir la lecture de posture. | Conservé comme extension utile au scénario. |
| Shape + Face | 12.93 | 2.60 | 41.48 | 276.03 | 929.80 | La combinaison fait clairement baisser le débit et augmente fortement l’occupation mémoire. | À activer seulement dans les modes où l’identification est vraiment nécessaire. |
| Combined Recognition | 5.20 | 2.09 | pic non représentatif | 361.89 | 1174.13 | Pipeline combiné lourd; la valeur max observée n’est pas représentative et doit être ignorée. | À limiter et à optimiser avant un usage continu. |
| Hand Recognition | 216.11 | 2.55 | pic non représentatif | 172.46 | 746.68 | La brique main fonctionne mais son utilité métier reste plus secondaire; le max mesuré est bruité. | Conservé comme module complémentaire, non prioritaire. |

## Comment lire ce tableau

- Le **FPS moyen** est l’indicateur principal de fluidité.
- Le **FPS minimum** permet d’identifier les baisses ponctuelles de débit.
- Le **FPS maximum** doit parfois être relativisé lorsqu’il s’agit d’un pic isolé.
- Le **CPU moyen** donne une idée du coût global du module.
- La **RAM moyenne** est particulièrement utile pour repérer les modes combinés les plus lourds.
