# 1. FROM: Partiamo dall'immagine ufficiale ultraleggera di Nginx basata su Alpine Linux (Slide 20 e 33)
FROM nginx:alpine

# 2. WORKDIR: Ci spostiamo nella cartella interna di Nginx dove vengono letti i siti web (Slide 22 e 31)
WORKDIR /usr/share/nginx/html

# 3. COPY: Copiamo il nostro file index.html dal nostro PC dentro la WORKDIR del container (Slide 23)
COPY index.html .

# 4. EXPOSE: Documentiamo che il server dentro il container ascolta sulla porta 80 (Slide 28)
EXPOSE 80

# 5. CMD: Comando che tiene acceso Nginx in primo piano quando avvii il container (Slide 29 e 31)
CMD ["nginx", "-g", "daemon off;"]