# Robustesse, logs et gestion d’erreurs

## Ce qui existe déjà
Le dépôt contient déjà plusieurs scripts qui impriment des messages clairs :
- `[RUN]`
- `[INFO]`
- `[ERROR]`
- `[WARN]`

## Ce qu’il faut mettre en avant
Même si le projet n’a pas encore une couche de logging complexe, il existe déjà :
- une gestion d’erreurs visible,
- des messages de sortie utiles,
- un benchmark qui sauvegarde des logs.

## Ce que tu peux dire dans le rendu
Le projet adopte une stratégie de robustesse simple mais cohérente :
- vérification de fichiers critiques,
- contrôle des imports / dépendances,
- messages explicites,
- arrêt propre des processus quand possible.
