# Dockerfile
FROM python:3.9-slim

# Set the working directory
WORKDIR /babyshop

# Install system dependencies
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential libpq-dev && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Install Python dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Django project
COPY . .

# Run Django commands to set up the database
RUN python manage.py makemigrations
RUN python manage.py migrate

# Expose the port
EXPOSE 8000

# Command to run the app
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
