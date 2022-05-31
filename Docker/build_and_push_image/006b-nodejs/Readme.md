# Build and Push Docker imgae (Node Js App)

## Steps

1. Create a 'package.json' file using `npm init`
   ```json
   {
     "name": "sample-node-js-app",
     "version": "1.0.0",
     "description": "",
     "main": "app.js",
     "scripts": {
       "test": "echo \"Error: no test specified\" && exit 1"
     },
     "author": "Hassan Ali Khan",
     "license": "ISC"
   }
   ```
2. Install express in the app using `npm i express` this will add dependancies in the package.json file
   ```

   ```
3. Create .gitignore and .dockerignore file
   '''
   node_modules
   npm-debug.log
   '''
4. Create 'app.js'

   ```js
   const express = require("express");
   const app = express();

   const port = 8080;
   const createdBy = process.env.CREATEDBY;

   app.get("/", function (req, res) {
     res.send(
       "This is a example of NODE JS containerize app, created by " + createdBy
     );
   });

   app.listen(port, () => {
     console.log("server is up, check http://localhost:" + port);
   });
   ```

5. Create 'Dockerfile' to write instructions for the docker image creation
   ```Dockerfile
   FROM alpine
   LABEL maintainer="johndoe@yahoo.com"
   RUN apk add --update nodejs npm
   COPY . /src
   WORKDIR /src
   RUN npm install
   ENV CREATEDBY="Hassan Ali Khan"
   EXPOSE 8080
   ENTRYPOINT ["node", "./app.js"]
   ```
6. Build the image using `docker image build -t hassanak/node-js-app2:v1 .`
7. Login to docker hub from terminal using `docker login`
8. Push the image to docker hub using `docker image push hassanak/node-js-app2:v1`
9. Pull the image using `docker image pull hassanak/node-js-app2:v1`
10. Run container using `docker container run -d --name=testingNodeJsApp -p 8000:8080 hassanak/node-js-app2:v1`
11. Test using `curl http://localhost:8000`
12. Stop container using `docker container stop testingNodeJsApp`
13. Remove conatiner using `docker container rm testingNodeJsApp`
14. Remove image using `docker image rm hassanak/node-js-app2:v1`
