FROM node:22-alpine

WORKDIR /app

# Installa le dipendenze sfruttando la cache di Docker
COPY package.json package-lock.json ./
RUN npm ci

# Copia il resto dei file sorgente Angular
COPY . .

EXPOSE 4200

# Avvia Angular in ascolto su tutte le interfacce del container
CMD ["npm", "start", "--", "--host", "0.0.0.0", "--port", "4200"]
