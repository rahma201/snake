# Base image
FROM python:3.12-slim

# Set working directory
WORKDIR /app

# Copy game files
COPY . /app

# Install dependencies
RUN pip install --no-cache-dir flask

# Expose port 80 inside the container
EXPOSE 80

# Start Flask server serving index.html
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=80"]
