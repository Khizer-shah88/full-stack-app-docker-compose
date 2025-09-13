FROM node:18.9.1

WORKDIR /app

# copy package.json and install deps
COPY package*.json ./
RUN npm install

# copy source code
COPY . .

# vite needs to listen on 0.0.0.0 so it's accessible from outside the container
ENV HOST=0.0.0.0

EXPOSE 5173

CMD ["npm", "run", "dev"]
