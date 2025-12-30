# 🚀 Projet DevOps/MLOps - Déploiement AWS EC2

## 📋 Description
Projet étudiant démontrant un pipeline complet MLOps avec entraînement de modèle ML et déploiement sur AWS EC2.

## 🎯 Objectifs
- [x] Entraîner un modèle de Machine Learning
- [x] Créer une API de prédiction (Flask/FastAPI)
- [x] Conteneuriser avec Docker
- [x] Mettre en place CI/CD avec GitHub Actions
- [x] Déployer sur AWS EC2
- [x] Tester l'API déployée

## 🏗️ Architecture
(voir dans architecture.png)

📁 Structure du projet

devops-mlops-aws-student-project/
├── README.md
├── requirements.txt
├── notebooks/
│   └── train_model.ipynb          # Entraînement du modèle
├── model/
│   └── model.pkl                  # Modèle sauvegardé
├── api/
│   ├── app.py                     Application principale
│   ├── model_loader.py           # Chargement du modèle
│   └── __init__.py
├── docker/
│   └── Dockerfile                # Configuration Docker
├── tests/
│   └── test_api.py              # Tests unitaires
├── .github/
│   └── workflows/
│       └── ci.yml               # Pipeline CI/CD
└── docs/
    └── screenshots/             # Captures d'écran


    🛠️ Technologies

    ML : Scikit-learn / TensorFlow / PyTorch

API : Flask / FastAPI / Streamlit

Conteneurisation : Docker

CI/CD : GitHub Actions

Cloud : AWS EC2

Monitoring : (optionnel)
