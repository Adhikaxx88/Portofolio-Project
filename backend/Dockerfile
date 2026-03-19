# backend/Dockerfile
FROM python:3.11-slim

WORKDIR /app

# Install dependencies dasar
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy semua kode backend
COPY . .

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]