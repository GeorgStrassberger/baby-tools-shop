# E-Commerce Project For Baby Tools

### TECHNOLOGIES

- Python 3.9
- Django 4.0.2
- Venv
- Pillow

### Hints

1. Docker Image bauen

```bash
docker build -t babyshop .
```

2. Docker Container aus dem Image bauen

```bash
  docker run -p 8000:8000 --name babyshop-app babyshop
```

3. In den Container einloggen

```bash
docker exec -it babyshop-app bash
```

4. Adminuser erstellen

```bash
  python manage.py createsuperuser
```

> Benutzername: admin
> E-Mail-Adresse: admin@example.com
> Passwort: **\*\*\*\***
> Passwort (nochmals): **\*\*\*\***

5. AdminUser menü aufrufen
   link http://localhost:5000/admin

6. Mit dem adminuser anmelden

7. Content erstellen

- Kategorien
- Items

```bash
  asdf
```
