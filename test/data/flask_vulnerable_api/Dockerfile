# Use an official Python base image
FROM python:3.10-slim@sha256:d8e262e069903a0b7790cd17a66d5343b2f04b9d9e19dc70f152c50fb511acfe

# Set working directory inside the container
WORKDIR /app

# Install Python dependencies
RUN pip install --no-cache-dir flask

# Expose port Flask will run on
EXPOSE 5000

# Run the Flask app
CMD ["python", "app.py"]
