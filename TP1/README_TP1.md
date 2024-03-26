# TP1 : Word Embeddings avec Word2Vec

## Auteur
DJAGHLOUL AYOUB AHMED AMINE

## Présentation du Projet
Ce TP explore l'utilisation de Word2Vec pour générer des word embeddings, permettant de capturer des relations sémantiques complexes entre les mots. À travers l'entraînement d'un modèle Word2Vec sur le corpus text8, nous démontrons comment ces embeddings peuvent être utilisés pour des tâches telles que la recherche de mots similaires et le calcul de similarités cosinus entre les mots.

## Configuration et Exécution

### Environnement Requis
- Python 3.6+
- Bibliothèques : NumPy, Pandas, Keras (pour TensorFlow backend)

### Installation des Dépendances
```bash
pip install numpy pandas keras tensorflow
```

### Exécution des Scripts
Les scripts sont configurés pour utiliser le modèle Word2Vec pré-entraîné. Pour exécuter l'analyse de similarité et trouver des mots proches :

```bash
python analyse_similarity.py
```

## Fonctionnalités Principales

### Génération de Word Embeddings
Utilisation de Word2Vec avec différentes configurations pour générer des embeddings de mots à partir du corpus text8. Les options clés incluent :
- Méthode d'apprentissage (CBOW ou Skip-gram)
- Dimension des vecteurs d'embedding
- Taille de la fenêtre contextuelle
- Downsampling des mots fréquents

### Analyse de Similarité
Calcul de la similarité cosinus entre les vecteurs de mots pour évaluer leur proximité sémantique. Par exemple, la similarité entre "hello" et "world" a été explorée.

### Recherche de Mots Proches
Identification des mots les plus proches sémantiquement pour un ensemble de mots donnés, illustrant la capacité des embeddings à capturer des relations de sens entre les mots.

## Résultats et Discussion
Les résultats démontrent l'efficacité des embeddings de mots à saisir des similarités et relations sémantiques subtiles. Une discussion approfondie sur les résultats obtenus, y compris les mots proches pour des termes tels que "best", "football", "france", "wine", "apple", "mouse", et "macron", est fournie dans le rapport associé au TP.