FROM node:14.21.1
WORKDIR /app
RUN npm install -g @angular/cli
COPY package.json ./
RUN npm install -f
COPY . .
RUN npm run build
EXPOSE 3000
CMD [ "npm", "start" ]