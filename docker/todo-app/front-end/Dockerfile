FROM node:14-alpine

EXPOSE 3000

COPY ["package.json", "package-lock.json", "./"]
RUN npm install


COPY ["src", "./src"]
COPY [".env", "./"]
ADD ["node_modules.tar.gz", "./"]

ENTRYPOINT [ "npm", "start" ]