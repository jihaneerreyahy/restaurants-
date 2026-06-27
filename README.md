# RAPPORT DE PROJET

## Analyse des Restaurants à Paris avec Python

### Réalisé par :

Nom : jihane er-reyahy

### Année Universitaire :

2025 – 2026

---

# Introduction

L'analyse des données est devenue un outil essentiel pour comprendre les comportements des consommateurs et améliorer les services proposés.

Dans ce projet, nous avons réalisé une analyse de données sur les restaurants de Paris afin d'explorer les caractéristiques des établissements, leurs catégories, leurs localisations et leurs évaluations.

L'objectif est d'utiliser Python et les bibliothèques d'analyse de données pour extraire des informations utiles à partir d'un dataset de restaurants parisiens.

---

# Objectifs du Projet

* Charger un dataset de restaurants de Paris.
* Nettoyer les données.
* Réaliser une analyse statistique.
* Visualiser les résultats avec des graphiques.
* Identifier les tendances principales.

---

# Outils Utilisés

## Langage

* Python

## Bibliothèques

* Pandas
* NumPy
* Matplotlib

## Environnement

* Anaconda
* Jupyter Notebook

---

# Présentation du Dataset

Le dataset contient des informations sur des restaurants situés à Paris.

Les informations analysées peuvent inclure :

* Nom du restaurant
* Adresse
* Catégorie
* Prix
* Note
* Nombre d'avis

Des jeux de données publics sur les restaurants parisiens existent notamment via les portails Open Data et Kaggle.

---

# Chargement des Données

Les données sont importées avec Pandas :

```python
import pandas as pd

df = pd.read_csv("restaurants_paris.csv")
```

Affichage des premières lignes :

```python
df.head()
```

---

# Analyse Exploratoire

Les fonctions suivantes ont été utilisées :

```python
df.info()
df.describe()
```

Ces analyses permettent de comprendre :

* Le nombre de restaurants
* Les variables disponibles
* Les valeurs manquantes

---

# Visualisation des Données

## Répartition des Restaurants

Un graphique permet d'observer la distribution des restaurants.

```python
df["category"].value_counts().plot(kind="bar")
```

## Répartition des Notes

```python
df["rating"].hist()
```

Ces visualisations facilitent l'interprétation des données.

---

# Résultats

L'analyse montre que Paris possède une grande diversité de restaurants : cuisine française, asiatique, vietnamienne, gastronomique et internationale. Des établissements très connus apparaissent régulièrement parmi les mieux évalués.

Quelques exemples :

* Sacrée Fleur Montmartre
* Le Colimaçon
* Le Cinq
* Hanoi - Restaurant Vietnamese

Les résultats montrent également que les restaurants les mieux notés ne sont pas nécessairement les plus chers.

---

# Conclusion

Ce projet a permis d'appliquer les techniques de Data Analysis sur un jeu de données réel concernant les restaurants à Paris.

Grâce à Python, Pandas et Matplotlib, il a été possible de :

* Nettoyer les données.
* Réaliser des statistiques descriptives.
* Produire des visualisations.
* Tirer des conclusions pertinentes.

Ce type d'analyse peut être utilisé dans les domaines du tourisme, de la restauration et du marketing afin d'aider à la prise de décision.

---

# Bibliographie

* Open Data Paris.
* Kaggle – Paris Restaurants Dataset.
* Documentation Pandas.
* Documentation Matplotlib.
