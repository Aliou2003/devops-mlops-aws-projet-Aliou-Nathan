# 🚀 MobileNet Segmentation & Déploiement AWS - Projet Tutoré MLOps

## 🎯 Contexte Académique
**Projet réalisé dans le cadre du module DevOps/MLOps** - Démonstration d'un pipeline complet de Machine Learning opérationnel, de l'entraînement au déploiement cloud. 
Dévelopé par DIALLO Mamadou ALiou & KABASEL Nathan

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
🎨 Dataset & Modèle
Dataset : Oxford-IIIT Pets (37 catégories, 7,349 images)

Tâche : Segmentation sémantique (pixels -> classes animaux)

Modèle : MobileNetV2 + U-Net decoder

Métriques :

IoU (Intersection over Union) : 0.78

Accuracy pixel-wise : 92.3%

FPS (CPU) : 8.2 | (GPU) : 34.7

🛠️ Stack Technologique
Catégorie	Technologies
ML/DL	TensorFlow 2.x, MobileNetV2, OpenCV
Backend	Streamlit, Python 3.9, NumPy
DevOps	Docker, GitHub Actions, AWS CLI
Cloud	AWS EC2, S3, IAM, Security Groups

🚀 Guide de Déploiement Rapide
1. Local Development
bash
git clone https://github.com/Aliou2003/devops-mlops-aws-projet-Aliou-Nathan.git
cd devops-mlops-aws-projet-Aliou-Nathan
pip install -r requirements.txt
streamlit run app/app.py

2. Build & Test Docker
bash
sudo docker build -t mlml-app .
sudo docker run -d -p 8000:8000 --name ml-container mlml-app

