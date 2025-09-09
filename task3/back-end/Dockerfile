FROM ubuntu:latest

RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

# If you get a This environment is externally managed error when trying to install Python packages, add the following line before
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

RUN pip3 install flask-cors

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers dans le conteneur
COPY api.py /app

#On redirige le port 5252 du conteneur docker vers le port 5252 de la machine hôte
EXPOSE 5252

#run server
CMD ["python3", "api.py"]
