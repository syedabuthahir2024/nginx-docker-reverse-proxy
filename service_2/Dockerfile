# Use official Python slim image
FROM python:3.9-slim

# Set working directory inside container
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Copy all remaining source files
COPY . .

# Start the app
CMD ["python", "app.py"]
