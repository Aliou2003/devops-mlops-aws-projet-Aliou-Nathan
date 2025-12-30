# 1. Base image
FROM python:3.10-slim

# 2. Créer le dossier de l'application
WORKDIR /app

# 3. Copier uniquement le fichier requirements.txt pour utiliser le cache
COPY requirements.txt .

# 4. Installer les dépendances
RUN pip install --no-cache-dir --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

# 5. Copier le reste du projet
COPY app/ ./app
COPY model/ ./model

# 6. Exposer le port pour Streamlit
EXPOSE 8501

# 7. Commande pour lancer l'application
CMD ["streamlit", "run", "app/app.py", "--server.port=8501", "--server.address=0.0.0.0"]
