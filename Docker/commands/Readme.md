# Docker Commands

## 1. Docker Installation and testing

| Sr. No. | Command                            | Description                                                           |
| ------- | ---------------------------------- | --------------------------------------------------------------------- |
| 1       | [Script File](../installDocker.sh) | Install Docker                                                        |
| 2       | docker --version                   | Display version of docker                                             |
| 3       | docker info                        | Detailed info about docker client and server                          |
| 4       | docker system info                 | Detailed info about docker client and server                          |
| 5       | docker version                     | Test client and daemon (server) are running and talking to each other |
| 6       | service docker status              | Check docker status                                                   |
| 7       | systemctl is-active docker         | Check docker status                                                   |
| 8       | systemlctl restart docker          | Restart docker                                                        |

## 2. Use Docker with out sudo

| Step. No. | Command                              | Description                                          |
| --------- | ------------------------------------ | ---------------------------------------------------- |
| 1         | sudo groupadd docker                 | Create the docker group.                             |
| 2         | sudo usermod -aG docker &lt;USER&gt; | Add your user to the docker group.                   |
| 3         |                                      | Log out and log back                                 |
| 4         | docker version                       | Verify that you can run docker commands without sudo |

## 3. Docker Images

### 3.1. List Images

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Flag</th>
      <th>Flag Value</th>
      <th>Argument</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=1>1</td>
      <td rowspan=1>docker images</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List all docker images on the system</td>
    </tr>
    <tr>
      <td rowspan=11>2</td>
      <td rowspan=11>docker image ls</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List all docker images on the system</td>
    </tr>
    <tr>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>&lt;image_name&gt;</td>
      <td rowspan=1>List all versions of an image</td>
    </tr>
    <tr>
      <td rowspan=1>--digests</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List images along with digest/hash</td>
    </tr>
    <tr>
      <td rowspan=1>-q</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>List image ids only</td>
    </tr>
    <tr>
      <td rowspan=6>--filetr</td>
      <td rowspan=1>dangling=true</td>
      <td rowspan=1></td>
      <td rowspan=1>List all dangling images</td>
    </tr>
    <tr>
      <td rowspan=1>dangling=false</td>
      <td rowspan=1></td>
      <td rowspan=1>List all images other than dangling images</td>
    </tr>
    <tr>
      <td rowspan=1>before=&lt;image_name/image_id&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Returns all images created before given image</td>
    </tr>
    <tr>
      <td rowspan=1>since=&lt;image_name/image_id&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Returns all images created after given image</td>
    </tr>
    <tr>
      <td rowspan=1>label=&lt;label&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Filters images based on the presence of a label or label and value.</td>
    </tr>
    <tr>
      <td rowspan=1>reference="&lt;filter_value&gt;"</td>
      <td rowspan=1></td>
      <td rowspan=1>List images based on any other type of filter</td>
    </tr>
    <tr>
      <td rowspan=1>--format</td>
      <td rowspan=1>"&lt;{{.format}}&gt;"</td>
      <td rowspan=1></td>
      <td rowspan=1>Format output using Go templates</td>
    </tr>
  </tbody>
</table>

### 3.2. Search Images

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Flag Value</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=4>1</td>
      <td rowspan=4>docker search</td>
      <td rowspan=4>&lt;image_name&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Search docker for all images with specfied name</td>
    </tr>
    <tr>
      <td rowspan=2>--filter</td>
      <td rowspan=1>"is-official=true"</td>
      <td rowspan=1>Search docker for all official images with specfied name</td>
    </tr>
    <tr>
      <td rowspan=1>"is-automated=true"</td>
      <td rowspan=1>Search docker for images with specfied name and automated build</td>
    </tr>
    <tr>
      <td rowspan=1>--limit</td>
      <td rowspan=1>&lt;int_limit&gt;</td>
      <td rowspan=1>Search docker for all images with specfied name with max number of images to list</td>
    </tr>
  </tbody>
</table>

### 3.3. Pull Images

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=4>1</td>
      <td rowspan=4>docker image pull</td>
      <td rowspan=1>&lt;image_name&gt;:&lt;image_tag&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Download an image from official account</td>
    </tr>
    <tr>
      <td rowspan=1>&lt;user_name/image_name&gt;:&lt;image_tag&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Download an image from user account</td>
    </tr>
    <tr>
      <td rowspan=1>&lt;image_name&gt;@&lt;image_digest&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Pull image based on digest</td>
    </tr>
    <tr>
      <td rowspan=1>&lt;image_name&gt;</td>
      <td rowspan=1>-a</td>
      <td rowspan=1>Pull all images from a repo with all tags</td>
    </tr>
  </tbody>
</table>

### 3.4. Remove Images

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=2>1</td>
      <td rowspan=2>docker image prune</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Delete all dangling images</td>
    </tr>
    <tr>
      <td rowspan=1></td>
      <td rowspan=1>-a</td>
      <td rowspan=1>Delete all images not associated with a container</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>docker rmi</td>
      <td rowspan=1>&lt;image_name&gt;:&lt;tag&gt;</td>
      <td rowspan=1></td>
      <td rowspan=2>Delete / remove an image</td>
    </tr>
    <tr>
      <td rowspan=3>3</td>
      <td rowspan=3>docker image rm</td>
      <td rowspan=1>&lt;image_name&gt;:&lt;tag&gt;</td>
      <td rowspan=1></td>
    </tr>
    <tr>
      <td rowspan=1>$(docker image ls -q)</td>
      <td rowspan=2>-f</td>
      <td rowspan=1>Delet all images</td>
    </tr>
    <tr>
      <td rowspan=1>$(docker image ls -f "dangling=true" -q)</td>
      <td rowspan=1>Remove dangling images</td>
    </tr>
  </tbody>
</table>

### 3.5. Ispect Images

| Sr. No. | Command                                             | Description               |
| ------- | --------------------------------------------------- | ------------------------- |
| 1       | docker history &lt;image_name&gt;:&lt;image_tag&gt; | Build history of an image |
| 2       | docker inspect &lt;image_name&gt;:&lt;image_tag&gt; | Detailed info about image |

## 4. Containerizing Images

### 4.1. Dockerfile

| Sr. No. | Command                                         | Description                                                                  |
| ------- | ----------------------------------------------- | ---------------------------------------------------------------------------- |
| 1       | FROM                                            | Specifies the base image for the new image you will build                    |
| 2       | RUN                                             | Aallows you to run commands inside the image which create new layers         |
| 3       | COPY                                            | Adds files into the image as a new layer                                     |
| 4       | EXPOSE                                          | Documents the network port that the application uses                         |
| 5       | ENTRYPOINT                                      | Sets the default application to run when the image is started as a container |
| 6       | LABEL, ENV, ONBUILD, HEALTHCHECK, CMD and more… |                                                                              |

Note: `apt-get install -no-install-recommends` is used to skip recommended downloads

### 4.2. Login to docker hub

| Sr. No. | Command      | Description         |
| ------- | ------------ | ------------------- |
| 1       | docker login | login to docker hub |

### 4.3. Build Image

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description </th>
    </tr>

  </thead>
  <tbody>
    <tr>
      <td rowspan=3>1</td>
      <td rowspan=3>docker image build -t</td>
      <td rowspan=3>&lt;image_name&gt;:&lt;tag&gt; &lt;path_of_Dockerfile&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Build an image based on the dockerfile at an address</td>
    </tr>
    <tr>
      <td rowspan=1>--no-cache=true</td>
      <td rowspan=1>Build an image based on the dockerfile at an address and skip cache</td>
    </tr>
    <tr>
      <td rowspan=1>--squash</td>
      <td rowspan=1>Build an image based on the dockerfile at an address and squash it</td>
    </tr>
  </tbody>
</table>

### 4.4. Tag Images

| Sr. No. | Command                                                                                      | Description                      |
| ------- | -------------------------------------------------------------------------------------------- | -------------------------------- |
| 1       | docker tag &lt;image_name&gt;:&lt;image_tag&gt; &lt;image_new_name&gt;:&lt;image_new_tag&gt; | Rename and make copy of an image |

### 4.5. Push Images

| Sr. No. | Command                                                | Description                 |
| ------- | ------------------------------------------------------ | --------------------------- |
| 1       | docker image push &lt;image_name&gt;:&lt;image_tag&gt; | Push an image to docker hub |

## 5. Docker Volumes

| Sr. No. | Command                                   | Description       |
| ------- | ----------------------------------------- | ----------------- |
| 1       | docker volume ls                          | List all volumes  |
| 2       | docker volume create &lt;volume_name&gt;  | Create new volume |
| 3       | docker volume inspect &lt;volume_name&gt; | Inspect a volume  |
| 4       | docker volume rm &lt;volume_name&gt;      | Remove a volume   |

## 6. Docker Containers

### 6.1. List Containers

| Sr. No. | Command                | Description                 |
| ------- | ---------------------- | --------------------------- |
| 1       | docker ps              | List all running containers |
| 2       | docker container ls    | List all running containers |
| 3       | docker ps -a           | List all containers         |
| 4       | docker container ls -a | List all containers         |

### 6.2. Container Logs

| Sr. No. | Command                                            | Description                     |
| ------- | -------------------------------------------------- | ------------------------------- |
| 1       | docker logs &lt;container_name or container_id&lt; | Fetch the logs of the container |

### 6.3. Run Containers in intractive mode

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=5>1</td>
      <td rowspan=5>docker container run -it</td>
      <td rowspan=5>&lt;image_name&gt;:&lt;tag&gt; &lt;environemt (sh)&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Run a container from an image in intractive mode in specified environment</td>
    </tr>
    <tr>
      <td rowspan=1>--name &lt;container_new_name&gt;</td>
      <td rowspan=1>Run a container in intractive mode and assign new name to container along with port</td>
    </tr>
    <tr>
      <td rowspan=1>--restart always</td>
      <td rowspan=1>Run a container which restarts always</td>
    </tr>
    <tr>
      <td rowspan=1>--restart unless-stoped</td>
      <td rowspan=1>Run a container which restarts unless-stoped</td>
    </tr>
    <tr>
      <td rowspan=1>--restart on-failed</td>
      <td rowspan=1>Run a container which restarts on-failed</td>
    </tr>
    <tr>
      <td rowspan=1>2</td>
      <td rowspan=1>exit</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Exit and terminate a container running in intractive mode</td>
    </tr>
    <tr>
      <td rowspan=1>3</td>
      <td rowspan=1>ctrl+pq</td>
      <td rowspan=1></td>
      <td rowspan=1></td>
      <td rowspan=1>Exit a container running in intractive mode</td>
    </tr>
    <tr>
      <td rowspan=1>4</td>
      <td rowspan=1>docker container exec -it</td>
      <td rowspan=1>&lt;container_name / id&gt; &lt;environemt (sh)&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Attach your shell to the terminal of a running container</td>
    </tr>
  </tbody>
</table>

### 6.4. Run Containers in detached mode

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=3>1</td>
      <td rowspan=3>docker container run -d</td>
      <td rowspan=3>&lt;image_name&gt;:&lt;tag&gt;</td>
      <td rowspan=1></td>
      <td rowspan=1>Run a container in detached mode</td>
    </tr>
    <tr>
      <td rowspan=1>-e &lt;variable_name&gt;=&lt;variable_value&gt;</td>
      <td rowspan=1>Run a container in detached mode with environmet variables</td>
    </tr>
    <tr>
      <td rowspan=1>--name &lt;container_new_name&gt; -p &lt;port&gt;:&lt;internal_port&gt; </td>
      <td rowspan=1>Run a container in detached mode and assign new name to container along with port</td>
    </tr>
  </tbody>
</table>

### 6.5. Start stop or pause containers

| Sr. No. | Command                                            | Description                        |
| ------- | -------------------------------------------------- | ---------------------------------- |
| 1       | docker container stop &lt;container_name / id&gt;  | Stop a running container           |
| 2       | docker container start &lt;container_name / id&gt; | Start a stoped or paused container |
| 3       | docker conatiner pause &lt;container_name / id&gt; | Pause a running container          |

### 6.6. Remove containers

| Sr. No. | Command                                            | Description                  |
| ------- | -------------------------------------------------- | ---------------------------- |
| 1       | docker container rm &lt;container_name / id&gt;    | Remove a stoped container    |
| 2       | docker container rm &lt;container_name / id&gt; -f | Forcefully delte a container |
| 3       | docker container rm $(docker container ls -aq) -f  | Remove all containers        |

## 7. Docker Volume Mount

<table>
  <thead>
    <tr>
      <th>Sr. No.</th>
      <th>Command</th>
      <th>Argument</th>
      <th>Flag</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan=5>1</td>
      <td rowspan=5>docker container run -d / -it</td>
      <td rowspan=5>&lt;image_name&gt;:&lt;image_tag&gt;</td>
      <td rowspan=1>-v &lt;host_path&gt;:&lt;container_path&gt;</td>
      <td rowspan=3>Start a container and bind a local directory with the container</td>
    </tr>
    <tr>
      <td rowspan=1>-v "$(pwd)"/&lt;folder_name&gt;:&lt;container_path&gt;</td>
    </tr>
    <tr>
      <td rowspan=1>--mount type=bind,source="$(pwd)"/&lt;folder_name&gt;,target=&lt;container_path&gt;</td>
    </tr>
    <tr>
      <td rowspan=1>-v &lt;volume_name&gt;:&lt;container_path&gt;</td>
      <td rowspan=2>Start a container and mount a volume with the container</td>
    </tr>
    <tr>
      <td rowspan=1>--mount source=&lt;volume_name&gt;,target=&lt;container_path&gt;</td>
    </tr>
  </tbody>
</table>
