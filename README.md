# E-Commerce Project For Baby Tools

### Technologies

- Python 3.9
- Django 4.0.2
- Venv
- Pillow

## Instructions

1. Navigate to the application directory

```bash
  cd babyshop_app
```

2. Build the Docker Image

```bash
  docker build -t babyshop .
```

3. Create a Docker Container from the Image

```bash
  docker run -p 5000:5000 --name babyshop-app babyshop
```

4. Log into the Container

```bash
  docker exec -it babyshop-app bash
```

5. Create an Admin User

```bash
  python manage.py createsuperuser
```

```bash
  Username: admin
  E-Mail-Adresse: admin@example.com
  Passwort: **\*\*\*\***
  Passwort (nochmals): **\*\*\*\***
```

6. Open the Admin Dashboard [http://localhost:5000/admin](http://localhost:5000/admin)

7. Log in with the Admin User

8. Add Content to the Application

   - Categories
   - Items
