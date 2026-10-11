# Laboratory Activity 6 Reflection

In this laboratory activity, I learned how to deploy a web application using Docker Compose. I used Nextcloud as the application and MariaDB as the database. This helped me understand how different containers can work together to provide a complete application.

One challenge I encountered was understanding how the application connects to the database. I learned that the `MYSQL_HOST=database` setting allows Nextcloud to find the MariaDB service through its service name in the Docker Compose configuration.

Docker Compose is useful because it allows me to manage multiple containers using one configuration file. Instead of starting each container separately with individual commands, I can use `docker-compose up -d` to start the services in the background. I can also check their status and stop them when they are no longer needed.

Separating the application and database into different containers makes the system more organized and easier to maintain. If a problem occurs, I can check the logs and container status to help identify the cause.

Overall, this activity improved my understanding of container deployment and basic cloud operations. I also learned the importance of checking configurations, monitoring containers, and documenting the steps performed. These skills will help me when working with more complex applications in the future.
