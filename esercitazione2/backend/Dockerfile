FROM python:3.12-slim

WORKDIR /app

# Copia e installa i requirements
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copia il codice del backend e il database
COPY . .

EXPOSE 8000

# Avvia FastAPI rendendolo raggiungibile all'esterno del container
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
