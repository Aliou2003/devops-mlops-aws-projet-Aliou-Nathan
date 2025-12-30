# 🚀 MobileNet Segmentation & Déploiement AWS - Projet Tutoré MLOps

## 🎯 Contexte Académique
**Projet réalisé dans le cadre du module DevOps/MLOps** - Démonstration d'un pipeline complet de Machine Learning opérationnel, de l'entraînement au déploiement cloud.

## 📋 Résumé du Projet
Déploiement d'un modèle **MobileNetV2** pour la segmentation sémantique sur le dataset **Oxford-IIIT Pets**, avec une interface Streamlit et infrastructure AWS automatisée.

**Période :** 29/11/2025 au 31/12/2025  
**Encadrement :** Module DevOps/MLOps  
**Niveau :** Projet tutoré

## 🏗️ Architecture Technique
```mermaid
graph TB
    A[Oxford-IIIT Pets Dataset] --> B[Google Colab]
    B --> C[MobileNetV2 Model]
    C --> D[Model Weights .h5]
    D --> E[Streamlit Application]
    E --> F[Docker Container]
    F --> G[GitHub Actions CI/CD]
    G --> H[AWS EC2 Instance]
    H --> I[🌐 API Live]
    
    style A fill:#e1f5fe
    style I fill:#c8e6c9
