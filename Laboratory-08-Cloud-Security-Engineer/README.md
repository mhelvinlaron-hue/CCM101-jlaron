# Laboratory Activity 8: The Cloud Security Engineer

## Mission Overview

This mission focused on protecting a Linux server from unwanted network connections. I used Docker to run an Nginx web application and configured UFW to control the traffic entering the server. Through this activity, I learned how to apply basic security rules while keeping the application accessible.

## Objectives

* Explain the Principle of Least Privilege and the concept of an attack surface.
* Inspect network ports and understand their security risks.
* Set up UFW with a Default Deny policy.
* Permit SSH and TCP traffic on port 8080.
* Record firewall settings and security practices in Markdown.
* Improve my GitHub portfolio through practical cloud computing tasks.

## Commands Executed

```bash
sudo docker run -d -p 8080:80 --name secure-web-app nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

I gained experience in running a web application with Docker and applying firewall rules on Ubuntu. I learned how to restrict incoming connections without blocking the services required by the application. I also understood why unnecessary ports should not be exposed and why checking firewall rules is important. These skills gave me a better understanding of basic server protection.
