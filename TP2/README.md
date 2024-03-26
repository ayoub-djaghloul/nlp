# TP2 : Analyse de Sentiments avec SVM

## Auteur
DJAGHLOUL AYOUB AHMED AMINE

## Présentation du Projet
Ce projet implique la mise en œuvre d'un classificateur à Machines à Vecteurs de Support (SVM) pour l'analyse de sentiments sur des données Twitter. L'objectif est de classifier les tweets en catégories positives, négatives ou neutres en fonction de leur contenu.

## Configuration de l'Environnement
Assurez-vous d'avoir Python 3.6+ installé ainsi que les packages suivants :
- pandas
- scikit-learn
- re (expressions régulières)

### Installation des Dépendances
Installez les packages Python requis en utilisant pip :

```bash
pip install pandas scikit-learn
```

## Prétraitement des Données
Les données sont chargées à partir de fichiers texte contenant les tweets avec leurs étiquettes de sentiment. Les étapes de prétraitement du texte incluent la conversion du texte en minuscules, la suppression des caractères non-mots et le remplacement de plusieurs espaces par un seul espace.

### Chargement des Données
Les jeux de données utilisés sont `twitter-2013train-A.txt`, `twitter-2013dev-A.txt` et `twitter-2013test-A.txt`, contenant respectivement les données d'entraînement, de développement et de test.

## Extraction des Caractéristiques
Un identifiant numérique unique est attribué à chaque mot du lexique du jeu de données. Les textes des tweets sont ensuite convertis en vecteurs de caractéristiques basés sur les occurrences des mots.

## Classification SVM
Un modèle SVM est entraîné sur les données traitées. Ce modèle est ensuite utilisé pour prédire le sentiment des tweets dans les ensembles de développement et de test.

### Évaluation du Modèle
La performance du modèle est évaluée à l'aide des métriques de précision, de rappel et de score F1, avec des résultats détaillés pour chaque catégorie de sentiment.

## Résultats
La section des résultats comprend les rapports de classification pour les ensembles de données de développement et de test, mettant en évidence l'efficacité du classificateur SVM dans les tâches d'analyse de sentiments.
