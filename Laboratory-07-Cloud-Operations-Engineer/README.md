# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

This activity focuses on checking the health of a Linux server and observing a running Docker container. I used system commands and container monitoring tools to gather information about resource usage, web requests, and application behavior.

## Objectives

- Examine the server's memory and storage capacity.
- Launch an Nginx web server using Docker.
- Send HTTP requests and observe the server's responses.
- Review container logs to identify successful and unsuccessful requests.
- Monitor CPU and memory usage while the container is running.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Displays memory usage in a readable format. |
| `df -h /` | Checks the available disk space on the root filesystem. |
| `top` | Shows running processes and system resource usage. |
| `docker ps` | Lists running containers. |
| `curl http://localhost:8080` | Sends a request to the Nginx web server. |
| `docker logs client-website` | Displays the web server's recorded activity. |
| `docker stats` | Shows real-time container resource usage. |

## Skills Practiced

Through this activity, I practiced using Linux commands to inspect a server and Docker commands to observe an application. I also learned how web request logs and resource statistics can help identify issues and evaluate the condition of a running container.

## Screenshots

Place the required laboratory screenshots in the `screenshots/` directory. Include the system memory and disk checks, Nginx deployment, web request tests, container logs, and resource monitoring results.
