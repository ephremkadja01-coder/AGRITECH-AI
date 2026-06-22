🌾 Agripredict: Système de Prévision de Rendement Agricole

Agripredict est une plateforme d'intelligence artificielle conçue pour aider les agriculteurs et les décideurs à anticiper les rendements des cultures. Basé sur l'analyse climatique et historique, le système propose des prévisions de rendement personnalisées par culture.
🌟 Fonctionnalités

    Moteur de prédiction multi-cultures : Plus de 90 modèles d'apprentissage automatique (Random Forest) spécialisés par type de culture.

    Analyse climatique avancée : Utilisation de l'ingénierie des données (déviations climatiques, variables de décalage temporel) pour une meilleure précision.

    Interface web robuste : Application développée avec le framework Django, garantissant sécurité et évolutivité.

    Architecture MVT : Séparation claire entre la logique de calcul (ML), la gestion des données et l'interface utilisateur.

🛠 Stack Technique

    Backend : Python, Django

    Machine Learning : scikit-learn, pandas, joblib

    Frontend : HTML5, CSS3, JavaScript

    Base de données : SQLite (développement) / PostgreSQL (production)

📊 Performance du modèle

Le système a été optimisé pour éviter le surapprentissage (overfitting) en intégrant des variables de décalage temporel (Last_Year_Features), permettant d'expliquer les variations saisonnières avec une robustesse accrue.

🏗 Architecture du projet


```text
agripredict/
├── manage.py
├── core/                   # Configuration Django (settings, urls)
├── prediction_app/         # Logique métier et vues
│   ├── ml_models/          # Stockage des modèles (.joblib)
│   ├── views.py            # Logique de prédiction
│   └── templates/          # Interface HTML/CSS
├── notebooks/              # Documentation et expérimentations
└── README.md


📈 Analyse des données

Le système identifie la température (Temp_Deviation) comme le facteur critique influençant la majorité des cultures, confirmant l'importance du stress thermique dans les prévisions agricoles.

Projet développé avec passion pour l'agriculture intelligente.
