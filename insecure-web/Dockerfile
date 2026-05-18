# Base image
FROM python:3.9-slim

# Install dependencies
RUN apt-get update && apt-get install -y sqlite3 && apt-get clean

# Set working directory
WORKDIR /app

# Copy application code
COPY app /app

# Install Python dependencies
RUN pip install flask

# Expose port
EXPOSE 5000
EXPOSE 80

# Run the application
CMD ["python", "app.py"]
