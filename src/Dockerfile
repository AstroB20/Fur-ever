# 1. Specify the base image (Python)
FROM python:3.9-slim

# 2. Set the working directory
WORKDIR /app

# 3. Copy requirements.txt and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 4. Copy the application code into the container
COPY . .

# 5. Expose a port (e.g., for Flask)
EXPOSE 5000

# 6. Specify the command to run the application
CMD ["python", "app.py"]
