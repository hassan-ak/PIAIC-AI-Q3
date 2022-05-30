# Build and Push Docker imgae (python App)

## Steps

1. Create project files in this case a simple python app 'app.py'
   ```py
   from flask import Flask
   import os
   import socket
   app = Flask(__name__)
   @app.route("/")
   def hello():
       html = "<body bgcolor='{bgname}'><h3>Hello {name}!</h3> <b>Hostname:</b> {hostname}<br/></body>"
       return html.format(name=os.getenv("NAME", "world"), hostname=socket.gethostname(), bgname=os.getenv("BGNAME", "orange"))
   if __name__ == "__main__":
       app.run(host='0.0.0.0', port=4000)
   ```
2. Create 'Dockerfile' to write instructions for the docker image creation
    ```Dockerfile
    # Use an official Python runtime as a parent image
    FROM python:2.7-slim
    WORKDIR /app
    ADD . /app
    RUN pip install --trusted-host pypi.python.org Flask
    ENV NAME World
    ENV BGNAME=purple
    EXPOSE  4000
    CMD ["python", "app.py"]
    ```
3. Build the image using `docker image build -t hassanak/py-app:v1 .`
4. Login to docker hub from terminal using `docker login`
5. Push the image to docker hub using `docker image push hassanak/py-app:v1`
6. Pull the image using `docker image pull hassanak/py-app:v1`
7. Run container using `docker container run -d --name=testingpyapp -p 8001:4000 hassanak/py-app:v1` and `docker container run -d --name=testingpyapp1 -p 8002:4000 -e NAME="Hassan" -e BGNAME="red" hassanak/py-app:v1`
8. Test using `curl http://localhost:8001` and `curl http://localhost:8002`
9. Stop container using `docker container stop testingpyapp` and `docker container stop testingpyapp1`
10. Remove conatiner using `docker container rm testingpyapp` and `docker container rm testingpyapp1`
11. Remove image using `docker image rm hassanak/py-app:v1`
