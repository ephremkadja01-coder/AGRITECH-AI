Projet : Système de Prévision et d'Alerte Agricole (Climate-Yield Predictor)

Ce projet vise à modéliser et prédire le rendement des cultures agricoles en utilisant des données climatiques historiques. En combinant l'apprentissage automatique (Machine Learning) et l'ingénierie de données climatiques, le système fournit une estimation du rendement par culture, permettant d'anticiper les risques climatiques.
🚀 Fonctionnalités principales

    Modélisation multi-cultures : Entraînement de modèles spécialisés pour 93 types de cultures.

    Ingénierie de données climatiques : Calcul de déviations climatiques (Température, Précipitations) pour capturer l'impact des anomalies sur les récoltes.

    Mémoire temporelle : Intégration de variables de décalage (Lag Features) pour prendre en compte l'impact des conditions climatiques de l'année précédente.

    Système d'alerte : Capacité à projeter le rendement futur sur la base de prévisions météorologiques.

🛠 Architecture Technique

    Langage : Python

    Bibliothèques principales : pandas, scikit-learn, joblib

    Algorithme : RandomForestRegressor (optimisé avec n_estimators=200, max_depth=10)

📊 Performance

Le modèle a été validé sur un score R2 permettant d'expliquer les variations de rendement dues aux facteurs environnementaux. Le système privilégie la généralisation pour éviter le surapprentissage.
📂 Structure du projet
Plaintext

├── data/                   # Données brutes et traitées
├── modeles_cultures/       # Modèles entraînés (format .joblib)
├── notebooks/
│   ├── 01_exploration.ipynb
│   ├── 02_nettoyage.ipynb
│   └── 03_entrainement_modele.ipynb
└── README.md

📈 Analyse des facteurs influents

Les résultats démontrent que la déviation de la température est le facteur prédictif le plus déterminant pour la productivité agricole.
💡 Utilisation

Pour tester le système avec une nouvelle culture :
Python

# Exemple de prédiction
resultat = predire_rendement_pour_culture(item_code=38, temp_dev=2.0, ...)
print(resultat)

Développé dans le cadre d'un projet de Data Science appliquée à l'agronomie.
