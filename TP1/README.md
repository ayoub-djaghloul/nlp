# TP1 : Analyse de Sentiment avec SVM

## Auteur
DJAGHLOUL AYOUB AHMED AMINE

## Présentation du Projet
Ce TP se concentre sur l'utilisation d'un modèle SVM (Machine à Vecteurs de Support) pour l'analyse de sentiment sur des données de Twitter. Le but est de classifier les tweets en trois catégories : positifs, négatifs et neutres.

## Configuration et Exécution

### Environnement Requis
- Python 3.6+
- Bibliothèques : Pandas, Scikit-learn, re (pour les expressions régulières)

### Installation des Dépendances
```bash
pip install pandas scikit-learn
```

### Chargement des Données
Les données sont chargées à partir de fichiers texte pré-définis, séparés en ensembles d'entraînement, de développement et de test.

```python
import pandas as pd

def charge_donnees():
    ...
```

### Prétraitement des Textes
Les tweets sont nettoyés et prétraités pour enlever les caractères spéciaux et les espaces multiples.

```python
import re

def preprocess_text(text):
    ...
```

### Extraction des Caractéristiques et Conversion au Format SVM
La conversion des textes en un format compatible avec le modèle SVM est réalisée par comptage des occurrences des mots et mapping à un espace vectoriel.

```python
from collections import Counter

def convert_to_svm_format(data, word_counts):
    ...
```

### Entraînement et Évaluation du Modèle
Le modèle SVM est entraîné sur l'ensemble d'entraînement et évalué sur les ensembles de développement et de test pour mesurer sa performance.

```python
from sklearn.svm import LinearSVC
from sklearn.metrics import classification_report

clf = LinearSVC(dual=False)
...
```

## Résultats et Discussion
Les résultats obtenus montrent la capacité du modèle SVM à classifier efficacement les sentiments des tweets. Une discussion sur les performances du modèle et les métriques d'évaluation est incluse dans le rapport associé au TP.

### Résultats sur l'Ensemble de Développement
```plaintext
Rapport de classification pour l'ensemble de développement:
              precision    recall  f1-score   support

          -1       0.58      0.41      0.48       340
           0       0.64      0.69      0.67       739
           1       0.62      0.66      0.64       575

    accuracy                           0.62      1654
   macro avg       0.61      0.59      0.59      1654
weighted avg       0.62      0.62      0.62      1654
```

### Résultats sur l'Ensemble de Test
```plaintext
Rapport de classification pour l'ensemble de test:
              precision    recall  f1-score   support

          -1       0.57      0.37      0.45       559
           0       0.61      0.76      0.68      1513
           1       0.70      0.62      0.66      1475

    accuracy                           0.64      3547
   macro avg       0.63      0.58      0.60      3547
weighted avg       0.64      0.64      0.64      3547
```

---

Ces modifications reflètent le passage d'une approche basée sur les embeddings de mots à une utilisation directe d'un modèle SVM pour la classification de sentiment.
