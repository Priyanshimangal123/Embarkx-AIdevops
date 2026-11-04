FROM node:24-slim
WORKDIR /app
COPY package*.json ./
# Install any dependencies and packages specified in package.json and no caches are considered to reduce the image size
RUN npm install --production
COPY . .
EXPOSE 3000
CMD [ "node", "app.js" ]