# 📊 TP4 — Analyse de données avec Python

**Analyse numérique, manipulation de données et visualisation**

## 📌 Présentation

Ce TP met en pratique plusieurs bibliothèques Python dédiées à l’analyse de données, aux calculs statistiques et à la visualisation graphique.

Il est organisé en quatre exercices portant sur l’analyse des températures de plusieurs villes algériennes, l’étude des notes d’étudiants, l’analyse de données hospitalières et la création de visualisations avec Matplotlib et Seaborn.

## 🎯 Objectifs

- Manipuler des tableaux multidimensionnels avec **NumPy**.
- Calculer des statistiques descriptives : moyenne, médiane, variance, écart-type et percentiles.
- Utiliser les masques booléens pour filtrer des données.
- Créer et transformer des DataFrames avec **Pandas**.
- Réaliser des opérations de regroupement, d’agrégation et de tableaux croisés.
- Nettoyer et enrichir des jeux de données.
- Générer des graphiques avec **Matplotlib** et **Seaborn**.
- Exporter les résultats au format CSV et enregistrer les figures.

## 🛠️ Technologies utilisées

- Python 3
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook (facultatif)

## 📂 Structure du projet

```text
TP4-Python-Data-Analysis/
├── exercise01_temperature.py
├── exercise02_grades.py
├── exercise03_hospital_pandas.py
├── exercise04_hospital_viz.py
├── requirements.txt
├── run_all.sh
└── outputs/
    ├── hospital_risk.csv
    ├── city_summary.csv
    └── figures/
        ├── ex04_matplotlib_cost.png
        ├── ex04_matplotlib_satisfaction.png
        ├── ex04_matplotlib_scatter.png
        ├── ex04_matplotlib_subplots.png
        ├── ex04_sns_bar.png
        ├── ex04_sns_risk.png
        ├── ex04_sns_heatmap.png
        ├── ex04_sns_pairplot.png
        └── ex04_dashboard.png
```

## 🧪 Contenu des exercices

### Exercice 1 — Analyse des températures avec NumPy

Étude des températures sur sept jours dans trois villes : Alger, Annaba et Oran.

Les opérations réalisées comprennent :

- Création et manipulation d'un tableau NumPy.
- Calcul des températures maximales par ville et par jour.
- Identification du maximum global et de sa localisation.
- Comparaison des températures entre Alger et Oran.
- Calcul des moyennes par ville.
- Identification des jours où Annaba était la ville la plus chaude.

### Exercice 2 — Analyse des notes des étudiants

Génération et analyse des notes de 100 étudiants dans cinq modules : THL, DSS, DB, SE et RE.

Les traitements comprennent :

- Calcul des moyennes individuelles et par module.
- Calcul des médianes, variances et écarts-types.
- Détermination des notes minimale et maximale.
- Calcul des percentiles du module THL.
- Filtrage des notes comprises entre 10 et 15.
- Identification des étudiants ayant obtenu plus de 15 dans tous les modules.
- Classement des cinq meilleures moyennes.
- Visualisation des résultats avec un diagramme en barres et un boxplot.

### Exercice 3 — Analyse des données hospitalières avec Pandas

Manipulation d'un jeu de données hospitalières concernant Alger, Annaba et Oran.

Les principales opérations sont :

- Création et enrichissement d'un DataFrame.
- Calcul du coût total d'hospitalisation.
- Classification des patients par groupe d'âge.
- Ajout, renommage et suppression de colonnes.
- Calcul de scores de risque et définition de catégories.
- Classement des patients selon le coût total.
- Agrégation des données par ville.
- Calcul du taux de réadmission.
- Nettoyage des données et correspondance des codes régionaux.
- Création d'un tableau croisé dynamique.
- Exportation des résultats en fichiers CSV.

### Exercice 4 — Visualisation avec Matplotlib et Seaborn

Création de graphiques pour explorer les coûts, la satisfaction et les risques hospitaliers.

**Avec Matplotlib :**
- Diagramme en barres des coûts par ville.
- Histogramme de la satisfaction.
- Nuage de points comparant le coût total et la satisfaction.
- Graphiques comparatifs par ville.

**Avec Seaborn :**
- Comparaison des coûts par ville et département.
- Boxplots et violinplots des scores de risque.
- Matrice de corrélation sous forme de heatmap.
- Pairplot pour explorer les relations entre variables.
- Dashboard combinant plusieurs visualisations.

Les graphiques sont enregistrés dans le dossier `outputs/figures/`.

## ⚙️ Installation

### 1. Cloner le dépôt

```bash
git clone <URL_DU_DEPOT>
cd <NOM_DU_DEPOT>
```

Remplace les valeurs entre chevrons par l'URL et le nom réels de ton dépôt GitHub.

### 2. Créer un environnement virtuel

Sous Windows :

```bash
python -m venv .venv
.venv\Scripts\activate
```

Sous Linux ou macOS :

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Installer les dépendances

```bash
python -m pip install -r requirements.txt
```

## ▶️ Exécution

Pour lancer tous les exercices sous Linux ou macOS :

```bash
bash run_all.sh
```

Pour exécuter les exercices individuellement :

```bash
python exercise01_temperature.py
python exercise02_grades.py
python exercise03_hospital_pandas.py
python exercise04_hospital_viz.py
```

**Remarque :** le script `run_all.sh` crée les dossiers de sortie nécessaires avant l'exécution. Si tu lances les fichiers individuellement, crée d'abord les dossiers `outputs/` et `outputs/figures/` lorsque les exercices doivent y enregistrer des fichiers.

## 📦 Dépendances

Les bibliothèques principales sont définies dans `requirements.txt` :

```text
numpy>=1.24
pandas>=2.0
matplotlib>=3.7
seaborn>=0.12
jupyter>=1.0
```

## 📈 Résultats attendus

À la fin du TP, le projet produit notamment :

- Des statistiques descriptives sur les températures et les notes.
- Des analyses et classifications des données hospitalières.
- Deux fichiers CSV : `hospital_risk.csv` et `city_summary.csv`.
- Plusieurs graphiques statistiques et un dashboard.
- Une mise en pratique des principales fonctionnalités de NumPy, Pandas, Matplotlib et Seaborn.

## 👨‍🎓 Auteur

**Ouael DJEDDI**

- GitHub : [@djeddiouael](https://github.com/djeddiouael)

## 📄 Licence

Projet pédagogique réalisé dans le cadre de travaux pratiques. Aucune licence spécifique n'est définie dans les fichiers fournis.
