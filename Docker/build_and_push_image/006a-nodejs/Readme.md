# Build and Push Docker imgae (Node Js App)

## Steps

1. Create a 'package.json' file using `npm init` 
   ```json
   {
     "name": "docker_nodejs_app",
     "version": "1.0.0",
     "description": "Node.js on Docker",
     "main": "server.js",
     "scripts": {
       "test": "echo \"Error: no test specified\" && exit 1"
     },
     "author": "Hassan Ali Khan",
     "license": "ISC"
   }
   ```
2. Install express in the app using `npm i express` this will add dependancies in the package.json file and update the file to add scripts
   ```json
   "scripts": {
       "start": "node server.js"
   },
   ```
3. Create .gitignore and .dockerignore file
   '''
   node_modules
   npm-debug.log
   '''
5. Create 'server.js'

   ```js
   "use strict";
   const express = require("express");
   // Constants
   const PORT = 8080;
   const HOST = "0.0.0.0";
   // App
   const app = express();
   app.get("/", (req, res) => {
     res.send("Hello world\n");
   });
   app.listen(PORT, HOST);
   console.log(`Running on http://${HOST}:${PORT}`);
   ```

5. Create 'Dockerfile' to write instructions for the docker image creation
    ```Dockerfile
    FROM node:latest
    WORKDIR /usr/src/app
    COPY package*.json ./
    RUN npm install
    COPY . .
    EXPOSE 8080
    CMD [ "npm", "start" ]
    ```
6. Build the image using `docker image build -t hassanak/node-js-app1:v1 .`
7. Login to docker hub from terminal using `docker login`
8. Push the image to docker hub using `docker image push hassanak/node-js-app1:v1`
9. Pull the image using `docker image pull hassanak/node-js-app1:v1`
10. Run container using `docker container run -d --name=testingNodeJsApp -p 8000:8080 hassanak/node-js-app1:v1`
11. Test using `curl http://localhost:8000`
12. Stop container using `docker container stop testingNodeJsApp`
13. Remove conatiner using `docker container rm testingNodeJsApp`
14. Remove image using `docker image rm hassanak/node-js-app1:v1`
