# Analyse détaillée du benchmark

## 1. Détection simple et identification
Face Tracking et Face Recognition ne remplissent pas exactement le même rôle. Le premier sert surtout à repérer rapidement un visage, alors que le second ajoute une couche d’identification. Il est donc logique que Face Recognition soit plus coûteux, même si le résultat obtenu reste encore exploitable.

## 2. Détection de scène avec YOLO
YOLO Objects et YOLO Pose ressortent comme les modules les plus convaincants pour une lecture de scène temps réel. Leur débit reste globalement correct, tout en apportant une information utile :
- objets et personnes pour l’un,
- posture et squelette pour l’autre.

Ces deux modules apparaissent comme les meilleurs candidats pour le cœur de la démonstration.

## 3. Effet des combinaisons
Le passage à des modules combinés modifie nettement le comportement :
- baisse du FPS moyen,
- augmentation de la mémoire occupée,
- coût de traitement plus important.

Shape + Face illustre déjà ce phénomène. Combined Recognition le montre encore plus clairement, avec un débit moyen très inférieur aux briques unitaires.

## 4. Cas particulier de la détection de main
Hand Recognition est intéressant, mais plus secondaire. Son intérêt est plus démonstratif et expérimental. Il enrichit la compréhension du projet, mais ne doit pas faire oublier que la détection de présence humaine reste prioritaire.

## 5. Conséquence pour la suite
L’analyse du benchmark conduit à une hiérarchie technique :
1. détection de personnes comme cœur fonctionnel,
2. pose ou visage comme enrichissement,
3. modules plus secondaires ou combinés à activer selon l’usage.
