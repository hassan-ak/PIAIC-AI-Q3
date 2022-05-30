# Build and Push Docker imgae (UBUNTU App)

## Steps

1. Intiate package.json file using `npm init--yes` and install express using `npm i express`
   ```json
   {
     "name": "demojsapp",
     "version": "1.0.0",
     "description": "demo nodejs app in ubuntu",
     "main": "app.js",
     "scripts": {
       "test": "echo \"Error: no test specified\" && exit 1"
     },
     "author": "Hassan Ali Khan",
     "license": "ISC",
     "dependencies": {
       "express": "^4.17.3"
     }
   }
   ```
2. Create project files 'app.js'

   ```js
   const express = require("express");
   const app = express();
   const port = 3000;
   app.get("/", (req, res) => res.send("Hello World! NodeJS"));
   app.listen(port, () =>
     console.log(`Example app listening on port ${port}!`)
   );
   ```

3. Create 'Dockerfile' to write instructions for the docker image creation

   ```Dockerfile
   FROM ubuntu:16.04
   RUN apt-get update
   RUN apt-get upgrade -y
   RUN apt-get dist-upgrade -y
   RUN apt-get install curl htop git zip nano ncdu build-essential chrpath libssl-dev libxft-dev pkg-config glib2.0-dev libexpat1-dev gobject-introspection python-gi-dev apt-transport-https libgirepository1.0-dev libtiff5-dev libjpeg-turbo8-dev libgsf-1-dev fail2ban nginx -y
   # Install Node.js
   RUN curl -sL https://deb.nodesource.com/setup_8.x | bash
   RUN apt-get install --yes nodejs
   RUN node -v
   RUN npm -v
   RUN npm i -g nodemon
   RUN nodemon -v
   # Cleanup
   RUN apt-get update && apt-get upgrade -y && apt-get autoremove -y
   # Node App
   COPY . /app
   WORKDIR /app
   # Install app dependencies
   RUN npm install
   # Binds to port 3000
   EXPOSE  3000
   #  Defines your runtime(define default command)
   # These commands unlike RUN (they are carried out in the construction of the container) are run when the container
   CMD ["node", "app.js"]
   ```

4. Build the image using `docker image build -t hassanak/ubuntu-js-app:v1 .`
5. Login to docker hub from terminal using `docker login`
6. Push the image to docker hub using `docker image push hassanak/ubuntu-js-app:v1`
7. Pull the image using `docker image pull hassanak/ubuntu-js-app:v1`
8. Run container using `docker container run -d --name=testingubuntujsapp -p 8003:3000 hassanak/ubuntu-js-app:v1`
9. Test using `curl http://localhost:8003`
10. Stop container using `docker container stop testingubuntujsapp`
11. Remove conatiner using `docker container rm testingubuntujsapp`
12. Remove image using `docker image rm hassanak/ubuntu-js-app:v1`
