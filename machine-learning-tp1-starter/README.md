
# TP de Machine Learning avec Python

## 1. Présentation

Ce TP a pour objectif de découvrir les bases du Machine Learning en utilisant Python. Il permet de manipuler un jeu de données, d'utiliser des bibliothèques spécialisées et de comprendre les premières étapes d'un projet d'apprentissage automatique.

## 2. Objectifs du TP

Les objectifs de ce travail pratique sont :

- Charger un jeu de données à partir d'un fichier CSV.
- Explorer et afficher les données.
- Utiliser les bibliothèques Pandas et NumPy.
- Comprendre la structure et les caractéristiques du dataset.
- Séparer les données pour préparer leur utilisation en Machine Learning.
- Découvrir les étapes nécessaires à la création d'un modèle d'apprentissage automatique.

## 3. Outils et bibliothèques utilisés

- **Python :** langage de programmation utilisé pour réaliser le TP.
- **Pandas :** bibliothèque permettant de charger et de manipuler les données.
- **NumPy :** bibliothèque utilisée pour effectuer des opérations numériques.
- **Scikit-learn :** bibliothèque permettant de préparer les données et de créer des modèles de Machine Learning.
- **VS Code :** éditeur utilisé pour écrire et exécuter le code Python.

## 4. Jeu de données

Le TP utilise le dataset **Iris**, un jeu de données classique en Machine Learning.

Il contient des informations sur trois espèces de fleurs Iris :

- Iris setosa
- Iris versicolor
- Iris virginica

Les caractéristiques étudiées comprennent la longueur et la largeur des sépales ainsi que la longueur et la largeur des pétales.

L'objectif est de découvrir comment ces données peuvent être utilisées pour réaliser une tâche de classification.

## 5. Étapes de réalisation

### Étape 1 : Importation des bibliothèques

Les bibliothèques nécessaires sont importées au début du programme.

```python
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
```

### Étape 2 : Chargement des données

Le fichier CSV est chargé à l'aide de Pandas.

```python
D = pd.read_csv("Iris_Dataset.csv")
```

### Étape 3 : Exploration des données

Les données sont affichées pour observer leur contenu et comprendre leur organisation.

```python
print(D)
print(D.head())
print(D.info())
print(D.describe())
```

Ces commandes permettent d'afficher les données, de consulter les premières lignes, de vérifier les types des colonnes et d'obtenir des statistiques descriptives.

### Étape 4 : Préparation des données

Les données sont examinées afin de vérifier leur structure et de préparer les caractéristiques qui seront utilisées pour l'apprentissage.

Cette étape peut notamment inclure la vérification des valeurs manquantes et la séparation des variables explicatives et de la variable cible.

### Étape 5 : Séparation des données

La fonction `train_test_split` de Scikit-learn permet de séparer les données en deux ensembles :

- **Ensemble d'entraînement :** utilisé pour apprendre au modèle.
- **Ensemble de test :** utilisé pour évaluer ses performances.

Cette séparation permet de vérifier si le modèle peut effectuer des prédictions sur des données qu'il n'a pas utilisées pendant son apprentissage.

## 6. Installation des bibliothèques

Pour installer les bibliothèques nécessaires, exécuter la commande suivante dans le terminal :

```bash
pip install pandas numpy scikit-learn
```

## 7. Exécution du TP

Pour exécuter le programme :

1. Ouvrir le dossier du TP dans VS Code.
2. Vérifier que Python est installé.
3. Vérifier que le fichier `Iris_Dataset.csv` se trouve dans le dossier approprié.
4. Installer les bibliothèques nécessaires.
5. Exécuter le script Python.
6. Observer les résultats affichés dans le terminal.

## 8. Résultats attendus

À la fin de ce TP, il sera possible de charger et d'explorer un jeu de données, de comprendre ses principales caractéristiques et de préparer les données pour une application de Machine Learning.

Le dataset Iris constitue un exemple simple pour découvrir les principes de la classification.

## 9. Conclusion

Ce TP permet de se familiariser avec Python et les principales bibliothèques utilisées en Machine Learning. Il aide à comprendre les premières étapes d'un projet, depuis le chargement des données jusqu'à leur préparation pour l'entraînement et l'évaluation d'un modèle.
