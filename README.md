#  Prédiction du Risque de Diabète par Analyse Clinique

##  Contexte

Ce projet a été réalisé en équipe avec **@hasNae111** au sein d’un **laboratoire biomédical**. 
L ’objectif principal est de concevoir un **système intelligent** capable de :

- **Prédire si un patient présente un risque élevé de développer le diabète**, à partir de critères cliniques.
- **Segmenter les patients** par regroupement non supervisé (clustering) pour identifier des profils similaires.

Les variables cliniques utilisées comprennent :
- Glycémie (`Glucose`)
- Pression artérielle (`BloodPressure`)
- Épaisseur du pli cutané (`SkinThickness`)
- Insuline (`Insulin`)
- Indice de Masse Corporelle (`BMI`)
- Hérédité du diabète (`DiabetesPedigreeFunction`)
- Âge (`Age`)

---

## Structure du projet

```bash
.
├── datas/
│   └── dataset.csv               # Jeu de données brut
├── notebooks/
│   └── script.ipynb       # Notebook principal avec tout le code
│   └── script_.ipynb   
├── models/
│   └── best_model.pkl             # Modèle sauvegardé après entraînement
├── outputs/
│   ├── clustering_plots/          # Graphiques de clustering (KMeans, PCA)
│   └── classification_reports/    # Matrices de confusion, scores F1, etc.
├── README.md                      # Présentation du projet
└── requirements.txt               # Dépendances du projet

##  Librairies utilisées

* pandas, numpy
* matplotlib, seaborn
* scikit-learn
* pickle

## Instructions d’exécution

1. Cloner le repo :

```bash
git clone https://github.com/r00tMG/risque_diabete_par_analyse_clinique_model_apprentissage.git
cd risque_diabete_par_analyse_clinique_model_apprentissage
```

2. Créer un environnement virtuel et l’activer :

```bash
python -m venv .venv
source .venv/bin/activate  
```

3. Installer les dépendances :

```bash
pip install -r requirements.txt
```

4. Lancer le notebook principal :

```bash
jupiter-lab
```

## Résultats attendus

* Intégrabilité backend/web via `best_model.pkl`

## Suivi Agile (Jira)

* Organisation en sprints
* Epics : Data cleaning, Model Training, Classification, Packaging
* Outils : Kanban, backlog, daily meetings

