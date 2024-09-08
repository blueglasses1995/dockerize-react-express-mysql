FROM node:18.0.0-alpine3.14
RUN apk update
RUN apk add --no-cache bash curl git
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
CMD ["npm", "run", "dev"]
