# Laboratory 4: Cloud-Native Engineer

## Mission Overview

This laboratory introduces cloud-native engineering and the use of Docker containers. The activities were completed using a KillerCoda Playground. An Nginx web server was downloaded and deployed inside a Docker container to understand how containers can make application deployment faster and more efficient than using traditional Virtual Machines.

## Objectives

- Understand the difference between Virtual Machines and Containers.
- Use Docker in a cloud-based environment through KillerCoda.
- Practice basic Docker commands.
- Download and run an Nginx container.
- Learn how to start, stop, check, and remove containers.
- Document the laboratory activities using Markdown.
- Organize the laboratory files for the Cloud Computing GitHub portfolio.

## Docker Commands Executed

### Checkpoint 3 — Checking Docker

- `docker --version` – Checks if Docker is installed and displays its version.
- `docker info` – Shows information about the Docker system and running environment.

### Checkpoint 4 — Running Nginx

- `docker pull nginx` – Downloads the Nginx image from Docker Hub.
- `docker run -d -p 8080:80 --name my-nginx nginx` – Creates and starts an Nginx container in the background.
- `curl http://localhost:8080` – Tests the Nginx web server through port 8080.

### Checkpoint 5 — Managing the Container

- `docker ps` – Displays the currently running containers.
- `docker stop my-nginx` – Stops the Nginx container.
- `docker ps -a` – Displays all containers, including stopped containers.
- `docker rm my-nginx` – Removes the stopped Nginx container.

## Skills Learned

- Learned the basic differences between VMs and containers.
- Learned how to use Docker commands.
- Learned how to download and run an Nginx image.
- Learned how port mapping works between the host and container.
- Learned how to manage a container from creation to removal.
- Improved my skills in creating technical documentation using Markdown.

## Challenges Encountered

One challenge I encountered was remembering the correct Docker commands and their options. I also needed to understand how port mapping works when accessing the Nginx server. After practicing the commands several times, I was able to run the container, check its status, stop it, and remove it successfully.

## Conclusion

This laboratory helped me understand how Docker containers can be used to deploy applications in a simple and efficient way. I also learned the basic container lifecycle and how Docker can be useful in cloud-native development.
