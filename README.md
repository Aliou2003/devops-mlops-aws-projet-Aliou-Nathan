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
```mermaid
graph TD
    A[Notebook Jupyter] --> B[Modèle .pkl]
    B --> C[API Flask/FastAPI]
    C --> D[Docker Container]
    D --> E[GitHub Actions CI/CD]
    E --> F[AWS EC2 Instance]
    F --> G[API Live]
