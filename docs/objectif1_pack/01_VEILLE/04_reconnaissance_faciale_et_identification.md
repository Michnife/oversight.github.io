# Veille 4 — Reconnaissance faciale et identification

## Rôle dans le projet
La reconnaissance faciale n’est pas la première brique nécessaire pour savoir s’il y a quelqu’un dans une pièce. En revanche, elle apporte une forte valeur de démonstration et permet de tester une logique d’identification sur des visages connus.

## Approche retenue dans le prototype
Le projet s’appuie sur :
- un dataset d’images classées par personne,
- une phase d’encodage des visages connus,
- une comparaison sur flux caméra.

Cette chaîne est pertinente pour un prototype, car elle permet de construire un scénario complet sans nécessiter une infrastructure lourde.

## Atouts
- Montre rapidement un résultat visible et compréhensible.
- S’appuie sur un dataset construit au sein du projet.
- Peut être activée seule ou combinée avec une brique de détection.

## Limites
- Très dépendante de la qualité du dataset.
- Les images floues, mal cadrées ou mal éclairées pénalisent fortement le résultat.
- Le coût de traitement est supérieur à celui d’un simple tracking.

## Lecture projet
La reconnaissance faciale est donc utile comme brique d’expérimentation et de démonstration, mais elle ne remplace pas la détection de présence. Elle vient plutôt se greffer sur un pipeline déjà capable de repérer une personne.

## Décision retenue
Le module est conservé dans le projet, mais son activation doit rester ciblée selon le scénario.
