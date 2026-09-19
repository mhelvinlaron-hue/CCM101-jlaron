# Mission Reflection

## 1. Boot time and setup: Docker vs. Virtual Machines

Docker containers can start in few seconds because they don't need to boot a whole operating system. A Virtual Machine takes more time because it needs to start the guest OS and setup the web server before it can be used.

## 2. Why is port mapping (-p 8080:80) necessary?

Port mapping is needed so the host computer can access the service inside the container. Nginx is running on port 80 inside the container, and `-p 8080:80` connects the host port 8080 to the container port 80.

## 3. What happens to data when you use docker rm?

When `docker rm` is used, the container and its writable data are removed from the system. The data inside the container will be lost if it was not saved in a volume or other persistent storage.

## 4. How does containerization change DevOps?

Containerization puts the application and its dependencies together, so it can help avoid the "works on my machine" problem. It also makes deployment easier because the team can manage the application as a service instead of setting up the server manually every time.

## 5. How is your GitHub portfolio evolving?

My GitHub portfolio is getting more organized as I add more laboratory activities and documentation. Compared to my first labs, I understand cloud computing more now and I also learned how Docker and containers are used in cloud-native development.
