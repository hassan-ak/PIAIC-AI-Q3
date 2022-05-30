# Build and Push Docker imgae (php App)
## Steps
1. Create project files in this case a simple php page 'index.php'
    ```php
    <?php
        echo "Hello World!";
        echo "PHP is so easy!";
    ?>
    ```
2. Create 'Dockerfile' to write instructions for the docker image creation
    ```Dockerfile
    FROM php:apache
    COPY index.php /var/www/html
    EXPOSE 80
    ```
3. Build the image using `docker image build -t hassanak/php-app:v1 .`
4. Login to docker hub from terminal using `docker login`
5. Push the image to docker hub using `docker image push hassanak/php-app:v1`
6. Pull the image using `docker image pull hassanak/php-app:v1`
7. Run container using `docker container run -d --name=testingphpapp -p 8000:80 hassanak/php-app:v1`
8. Test using `curl http://localhost:8000`
9. Stop container using `docker container stop testingphpapp`
10. Remove conatiner using `docker container rm testingphpapp`
11. Remove image using `docker image rm hassanak/php-app:v1`