# Stage 1: Build backend
FROM node:18.9.1 AS builder

WORKDIR /app

# copy package files and install dependencies
COPY package*.json ./
RUN npm install


# copy the rest of the backend code
COPY . .

# Stage 2: Run backend

# expose backend port
EXPOSE 5050

# run server
CMD ["npm", "start"]




