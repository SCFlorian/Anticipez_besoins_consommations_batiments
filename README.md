# Anticipez les besoins en consommation des bâtiments
L’objectif de ce projet est de développer un modèle de prédiction de la consommation énergétique des bâtiments à partir de données publiques de la ville de Seattle (2016).

Le travail consiste à explorer les données, tester plusieurs modèles de machine learning et comparer leurs performances afin d’identifier les facteurs ayant le plus d’impact sur la consommation.

## Table des matières
- [Problématique](#problematique)
- [Données utilisées](#donnees-utilisees)
- [Organisation du projet](#organisan-du-projet)
- [Installation & Utilisation (VS Code)](#installation_&_utilisation_(_VS_Code_))


### Problématique
L'objectif ici est :
- de préparer une courte analyse exploratoire
- de réaliser des tests des différentes modèles supervisés
- la détermination des facteurs principaux impactant le plus le modèle

### Données utilisées
- Fichier csv de la formation. Ce sont des données de la ville de Seattle sur l'année 2016.
- Source officielle de la ville de Seattle : https://data.seattle.gov/Built-Environment/Building-Energy-Benchmarking-Data-2015-Present/teqw-tu6e/about_data

### Organisation du projet
```
Projet_Besoins_Consommation_Bâtiments
├── Data/                   # Jeux de données nettoyés et préparés
│   ├── Projet_3_etape1_clean.csv
│   ├── Projet_3_etape2_clean.csv
│   ├── Projet_3_etape3_clean.csv
│   └── building_clean_second.csv
│
├── graphiques/             # Visualisations générées
│   ├── boxplot_buildingtype.png
│   ├── boxplot_compliancestatus.png
│   ├── boxplot_neighborhood.png
│   ├── boxplot_numberoffloors.png
│   ├── boxplot_outlier.png
│   └── boxplot_primarypropertytype.png
│
├── notebooks/              # Analyse et modélisation (Jupyter Notebooks)
│   ├── Notebook_1_analyse_exploratoire.ipynb
│   ├── Notebook_2_preparation_features.ipynb
│   ├── Notebook_3_modelisation_features.ipynb
│   ├── Notebook_4_tests_modeles.ipynb
│   └── Notebook_5_optimisation_modele.ipynb
│
├── .gitignore              # Fichiers/dossiers ignorés par Git
├── README.md               # Documentation du projet
├── __init__.py             # Initialisation du module Python
└── pyproject.toml          # Configuration et dépendances
```
### Installation & Utilisation (VS Code)
1. Cloner le projet
```
git@github.com:SCFlorian/Anticipez_besoins_consommations_batiments.git
```
2. Installer les dépendances
Le projet utilise pyproject.toml pour la gestion des dépendances.
Deux options possibles :
```
# Installer poetry si besoin
pip install poetry

# Installer les dépendances
poetry install
```
Avec pip directement
```
pip install .
```
3. Ouvrir le projet dans VS Code
```
code .
```
4. Configurer l’environnement Python dans VS Code
	1.	Installez l’extension Python (si ce n’est pas déjà fait).
	2.	Appuyez sur Ctrl+Shift+P (Windows/Linux) ou Cmd+Shift+P (Mac).
	4.	Recherchez “Python: Select Interpreter”.
	5.	Sélectionnez l’environnement créé par Poetry ou celui dans lequel tu as installé le projet.

5. Travailler avec les notebooks
	•	Les notebooks se trouvent dans le dossier :
```
notebooks/
```
	•	Ouvrez n’importe quel fichier .ipynb (ex. Notebook_1_analyse_exploratoire.ipynb).
	•	VS Code activera automatiquement l’éditeur interactif Jupyter.
	•	Vous pouvez exécuter les cellules avec Shift+Enter.

