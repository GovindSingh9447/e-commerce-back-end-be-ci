FROM node:16.20
WORKDIR /app
COPY . .
RUN cp .env.example .env
RUN npm install
RUN npm install pm2 -g
EXPOSE 7770
ENTRYPOINT ["pm2-runtime", "index.js"]