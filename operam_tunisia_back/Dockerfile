# Use Python base image
FROM python:3.12

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PWD=password
    
# Set working directory in the container
WORKDIR /app

# Copy and install requirements
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copy the rest of the application files to the container
COPY . .

# Expose the port your Django app runs on
EXPOSE 8000

# Start the Django server

# CMD ["python", "manage.py", "runserver", "0.0.0.0:8000", "&&", "python", "manage.py", "migrate"]
CMD ["sh", "-c", "python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]


