FROM python:3.13.0b1-slim

RUN adduser --disabled-password --gecos '' appuser
USER appuser

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "app/app.py"]