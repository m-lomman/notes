Following this guide: [Docker Workshop](https://docs.docker.com/get-started/workshop/02_our_app/)

Using base project from: [Docker Getting Started App](https://github.com/docker/getting-started-app/tree/main)

`docker build` → Downloads an image if you don’t have one already (e.g. `node:lets-alpine`, `node:18`). Does not start a container, and utilises a `Dockerfile` . Use `-t <name>` to give it a tag.

`docker run` → Runs the image. `-d` runs the container in the background (detach). `run` pulls dependencies, and using [Bind Mounts](https://docs.docker.com/get-started/workshop/06_bind_mounts/) you can make it so the dependencies are not downloaded to your local machine.

`docker ps` → Lists containers running with ID 

`docker stop <container-id>` → Stops the container using the ID from `docker-ps` 

`docker rm <container-id>` → Deletes the image (`stop` retains its state, meaning you can start it again). You can use a container’s name instead of id `--name test-name`.

`docker rmi <image-id>` → Deletes the image. Can only be done if the image is not in use, but can use a tag id `-t test-tag`

`docker compose` → (needs a more in depth description) [Using Docker Compose](https://docs.docker.com/get-started/workshop/08_using_compose/)

---

`CMD` → Used in a Dockerfile. Specifies the default command to run when starting a container from that image

`<container-id>` → You do not need to list all ID characters, just enough to differentiate it from other ones

`RUN` → Run a command while building container

`ENV` → Set an environment variable in dockerfile