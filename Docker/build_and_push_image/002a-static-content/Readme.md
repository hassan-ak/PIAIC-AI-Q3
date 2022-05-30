# Build and Push Docker imgae (Static Web)
## Steps
1. Create project files in this case a simple html page 'index.html'
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Hello World!</title>
    </head>
    <body>
        <div align="center">
        <h1>Hello World!</h1>
        <img src="images/one.jpeg" alt="Hello World" />
        </div>
    </body>
    </html>
    ```
2. Create 'Dockerfile' to write instructions for the docker image creation
    ```Dockerfile
    FROM nginx:latest
    COPY . /usr/share/nginx/html
    ```
3. Build the image using `docker image build -t hassanak/static-web-content:v1 .`
4. Login to docker hub from terminal using `docker login`
5. Push the image to docker hub using `docker image push hassanak/static-web-content:v1`
6. Pull the image using `docker image pull hassanak/static-web-content:v1`
7. Run container using `docker container run -d --name=testingStaticWeb -p 8000:80 hassanak/static-web-content:v1`
8. Test using `curl http://localhost:8000`
9. Stop container using `docker container stop testingStaticWeb`
10. Remove conatiner using `docker container rm testingStaticWeb`
11. Remove image using `docker image rm hassanak/static-web-content:v1`