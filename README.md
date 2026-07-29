# Livrable - YouCode
# Exploration de données - Sell4All

## 1. Présentation du besoin

L'objectif de ce projet est de réaliser une première exploration des données avec Python (Pandas, Matplotlib) dans un notebook Jupyter, puis de produire un ensemble de données propre, prêt à être exploité dans un futur projet d'IA permettant de recommander automatiquement des vêtements d'occasion aux utilisateurs de Sell4All, en s'appuyant notamment sur leur pays, leur âge, leur genre et leurs dépenses sur le site.

## 2. Étapes suivies pendant les 3 jours de réalisation

**Jour 1 : Mise en place de l'environnement**
- Installation de Python via Miniconda
- Création d'un environnement virtuel dédié au projet
- Installation de Jupyter Notebook, Pandas et Matplotlib
- Prise en main du fichier **dataset-sell4all.csv** (lecture, première exploration)

**Jour 2 : Exploration et analyse des données**
- Lecture du fichier CSV avec Pandas
- Affichage des 5 premières lignes **.head()**
- Affichage et explication du résumé technique du dataset **.info()** : nombre d'entrées, valeurs non nulles, types de données
- Calcul de la moyenne et de la médiane des colonnes **Age** et **Customer spendings**
- Calcul bonus : médiane d'âge par pays **groupby**
- Création d'une visualisation (graphique à barres) des dépenses des clients par pays avec Matplotlib

**Jour 3 : Nettoyage des données et finalisation**
- Suppression des lignes correspondant à des clients ayant dépensé moins de 10 € sur le site
- Suppression des lignes en doublon
- Export des données nettoyées dans un nouveau fichier CSV **dataset-sell4all-clean.csv**, en ne conservant que les colonnes **Country**, **Age**, **Gender**, **Customer spendings**
- Relecture complète du notebook (exécution de bout en bout, vérification des explications Markdown)
- Rédaction du README.md et publication du dépôt GitHub

## 3. Fonctionnalités développées / éléments finalisés

- Chargement et inspection du dataset **dataset-sell4all.csv**
- Résumé technique des données (nombre de lignes, colonnes, types) avec explication détaillée en Markdown
- Statistiques descriptives : moyenne et médiane de l'âge et des dépenses clients
- Médiane d'âge par pays (question bonus)
- Visualisation des dépenses clients par pays (graphique à barres)
- Nettoyage des données :
  - Suppression des clients ayant dépensé moins de 10 €
  - Suppression des doublons
- Export du fichier nettoyé **dataset-sell4all-clean.csv** avec les colonnes **Country**, **Age**, **Gender**, **Customer spendings**

Le notebook final est disponible dans **exploration_sell4all.ipynb**.

## 4. Mode d'exécution du projet

### Prérequis
- Miniconda installé ([https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html))
- Python via Miniconda (version 3.14.6)
- Jupyter Notebook
- Les bibliothèques Python : Pandas et Matplotlib

### Étapes pour lancer le projet
1. **Lancer Miniconda Prompt**
  Taper dans le barre de recherche de votre PC "Anaconda Prompt", puis la lancer.

3. **Cloner le dépôt**
   ```bash
   git clone <url-du-depot>
   cd <nom-du-dossier>
   ```

4. **Créer et activer un environnement Python**
   ```bash
   conda create -n sell4all python=3.14
   conda activate sell4all
   ```

5. **Installer les dépendances**
   ```bash
   conda install jupyter pandas matplotlib
   ```

6. **Lancer Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

7. **Ouvrir le notebook**
   - Dans l'interface Jupyter, ouvrir le fichier **exploration_sell4all.ipynb**
   - Exécuter les cellules dans l'ordre **Kernel → Restart & Run All**
