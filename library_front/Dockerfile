FROM node:alpine
WORKDIR /src
COPY package.json ./
COPY ./ ./
RUN npm i
CMD ["npm", "run", "start"]