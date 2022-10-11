FROM node:14-alpine

EXPOSE 3001

COPY ["package.json", "package-lock.json", "./"]
RUN npm install


COPY ["src", "./src"] dest
ADD ["node_modules.tar.gz", "./"]

ENTRYPOINT [ "npm", "start" ]