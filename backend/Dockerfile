FROM python:3.11-slim
WORKDIR /app

#Install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

#Set environment variables from .env
#Copy project files

COPY . .
ENV KAGGLE_CONFIG_DIR=/app/kaggle
CMD ["python", "main.py"]
