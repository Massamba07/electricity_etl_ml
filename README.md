# **PowerFlow: An Integrated Data Pipeline for Electricity Analytics**

## **Description**
**PowerFlow** est un projet complet couvrant toutes les étapes d'un pipeline data autour des données d'électricité. Il inclut :
- **Data ingénierie** : Extraction, transformation et chargement (ETL) des données.
- **DevOps** : Intégration continue, tests unitaires et déploiement sur Kubernetes.
- **Data science** : Modèle de machine learning pour prédire la consommation électrique.
- **Data analysis** : Visualisation des données et analyse des tendances.

Ce projet est conteneurisé avec Docker et conçu pour être facilement déployé sur Kubernetes.

---

## **Fonctionnalités**
1. **ETL (Data Engineering)** :
   - Ingestion de données (fichiers CSV, API ou bases de données).
   - Transformation des données : nettoyage, enrichissement et normalisation.
   - Stockage des données nettoyées sur Google Cloud Storage ou Bitbucket.

2. **DevOps** :
   - Tests unitaires avec `pytest`.
   - Analyse de code avec `pylint` et formatage avec `black`.
   - Pipeline CI/CD via GitHub Actions pour automatiser les tests, l'analyse, et le déploiement.

3. **Data Science** :
   - Modèle prédictif pour la consommation électrique basé sur des données historiques.
   - Évaluation des performances du modèle avec des métriques standards.

4. **Data Analysis** :
   - Visualisation interactive des données avec `matplotlib`, `seaborn`, et `plotly`.
   - Rapports d’analyse des tendances et insights clés.

---

## **Architecture du projet**

```plaintext
PowerFlow/
│
├── data/               # Données brutes et transformées
├── src/                # Code source du projet
│   ├── etl/            # Scripts ETL (Extraction, Transformation, Chargement)
│   ├── ml/             # Modèle Machine Learning
│   ├── analysis/       # Scripts pour l'analyse et la visualisation
│   └── utils/          # Fonctions utilitaires communes
│
├── tests/              # Tests unitaires
├── Dockerfile          # Conteneurisation avec Docker
├── .github/            # Configurations pour GitHub Actions
│   └── workflows/
├── requirements.txt    # Dépendances Python
└── README.md           # Documentation du projet
