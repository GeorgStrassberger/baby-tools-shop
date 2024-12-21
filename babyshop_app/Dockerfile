# Pyhton version definieren
FROM python:3.9

#Festlegen des Arbeitsverzeichnis für den Container
WORKDIR /babyshop

#Kopieren der daten in das Arbeitsverzeichnis
COPY . /babyshop

# Packete updaten und installieren, Django & Pillow
RUN pip install --upgrade pip && pip install django==4.0.2 Pillow

#Run Django commands to set up the application
RUN python manage.py migrate

#Expose the Django default port
EXPOSE 5000

#Shell Befehl um den server im Container zu starten
CMD ["sh", "-c", "python manage.py runserver 0.0.0.0:5000"]

#CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
