FROM node:21 

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

COPY .env.docker .env.local

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]
