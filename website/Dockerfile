FROM node:latest
WORKDIR /app
RUN apt-get update
COPY package.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 4173
CMD ["npm", "run", "preview"]
