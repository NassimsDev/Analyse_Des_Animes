# 📝 Analyse et Ranking d'Animés (Anime Score Index)

Ce projet propose une méthode d'analyse de données pour classer les animés non pas uniquement sur leur popularité, mais sur un **indice de performance multidimensionnel**. L'objectif est de déterminer de manière objective quelles sont les véritables pépites d'un catalogue de streaming d'animés.

## 🚀 Installation

### Prérequis

- **Python 3.x** (disponible via l'extension Python dans VS Code ou sur python.org)
- Un environnement de notebook (Jupyter, VS Code ou Google Colab)

### Modules nécessaires

Lancez la commande suivante dans votre terminal pour installer les bibliothèques utilisées dans l'analyse :

```bash
pip install pandas matplotlib numpy

```

---

## 🧠 Méthodologie du "Score Final"

Pour éviter le biais des notes de fans parfois subjectives, ce projet calcule un score basé sur trois piliers :

1. **La Note Globale ()** : La base de l'appréciation du public.
2. **La Régularité ()** : Calculée par l'écart entre le meilleur et le pire épisode. Un score de 10 indique une qualité constante sans aucun "épisode raté".
3. **Le Mérite de Longévité ()** : Un bonus calculé via un logarithme (`np.log10`) pour récompenser les animés qui maintiennent une haute qualité sur un grand nombre d'épisodes.

---

## 📊 Fonctionnalités du Notebook

Le projet suit les étapes classiques de la Data Science :

- **Nettoyage (Data Cleaning)** : Suppression des colonnes inutiles, gestion des doublons et traitement des valeurs manquantes.
- **exploration et calculs** : Création d'indicateurs personnalisés (Écart, Score de Régularité).
- **Visualisation** :
- Graphique de corrélation entre régularité et note globale.
- Histogramme de la distribution des notes.
- Top 10 final sous forme de diagramme à barres.

- **Exportation** : Génération d'un fichier CSV (`dataset_trié_cleané.csv`) prêt pour Excel avec un classement humain (commençant à 1).

---

## 🏆 Résultats

L'analyse permet de mettre en avant dans le catalogue les animés les plus susceptible de plaire
