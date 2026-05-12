# Veille 6 — Structuration logicielle, benchmark et synthèse des choix

## Pourquoi cette partie relève aussi de la veille
La veille ne porte pas seulement sur des algorithmes. Elle porte aussi sur les façons de rendre un projet :
- testable,
- démontrable,
- comparable,
- documenté,
- et évolutif.

Dans ce cadre, la structuration logicielle et l’outillage de benchmark font pleinement partie des choix technologiques du projet.

## Axes retenus
Le projet a progressivement intégré :
- un launcher unique pour lancer rapidement les démonstrations,
- un health check pour vérifier l’environnement,
- un benchmark centralisé avec mesures et rapport,
- une organisation plus lisible du dépôt,
- des outils de dataset pour les visages.

## Pourquoi c’est important
Sans cette structuration, les briques resteraient dispersées et plus difficiles à comparer. Avec elle, le projet peut :
- exécuter plusieurs modules sur une base commune,
- conserver des résultats de test,
- présenter un état d’avancement plus sérieux,
- préparer la suite avec un minimum de capitalisation.

## Synthèse des choix techniques
À ce stade, les choix retenus se dessinent clairement :
- détection de personnes comme priorité,
- enrichissement par pose ou visage selon le besoin,
- modules complémentaires activés à la demande,
- benchmark comme outil de décision.

## Conclusion générale de la veille
La veille réalisée conduit à une architecture hiérarchisée, où le cœur du projet repose sur la perception humaine dans une scène, et où les autres briques viennent compléter ou enrichir ce socle sans le remplacer.
