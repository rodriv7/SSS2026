FROM node:22-alpine

RUN apk add --no-cache git

RUN git clone -b branch-2 https://github.com/rodriv7/SSS2026.git /repo

WORKDIR /repo/esercitazione2/frontend

RUN npm ci

EXPOSE 4200

CMD ["npm", "start", "--", "--host", "0.0.0.0", "--port", "4200"]
