FROM node:20-bullseye
WORKDIR /usr/src/app
COPY ../package*.json ./
RUN npm install
RUN chown -R node:node /usr/src/app
USER node
CMD ["npm", "run", "dev"]
