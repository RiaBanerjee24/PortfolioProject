# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 5000 for Flask
EXPOSE 5000

# Set the environment variable for Flask to run in production mode
ENV FLASK_APP=app.py
ENV FLASK_ENV=production

# Run the application
CMD ["python", "server.py"]
