# Docker app basics
This project contains a simple basic docker file, which is used to create the docker image. The app simply displays the text "Docker App" on the browser, when the container is run.

The **Dockerfile** in the project has all the necessary instructions to build the docker image.

## Running the application using Docker
1. Build the docker image using `docker build -t node-app:1.0 .`
2. Use `docker images` to see the docker images, including the one you just built.

   You will see the port number on which it runs. You now need to bind this port to you local port while running the image using the next command.
3. Run the docker app using `docker run -d -p 3000:3000 node-app:1.0`.
4. Hit **localhost:3000** in your browser to see the running image.
5. `docker ps` lists all the running containers.
6. `docker logs <container id>` to see the logs.
7. `docker stop <container id>` to stop the container.
