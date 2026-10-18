# Laboratory 09 Reflection

### 1. Why is automation critical when managing hundreds of cloud servers?

Automation is helpful when managing many cloud servers because it reduces the amount of manual work. Instead of entering the same commands repeatedly, an engineer can prepare a script to perform the task. This makes routine work easier to manage and gives engineers more time to handle other responsibilities.

### 2. What are the dangers of automation? What happens if a destructive typo runs on 1,000 servers?

Automation can become a serious risk when a script contains a harmful command. If that command runs across 1,000 servers, it could delete important files or interrupt many services at once. To avoid this, scripts should be reviewed and tested before deployment. Keeping backups and checking the results can also help reduce the damage caused by mistakes.

### 3. How did writing a Bash script differ from creating the Docker Compose file in Lab 6?

In Lab 9, I used Bash commands to create a backup folder and compress application data. In Lab 6, I used Docker Compose to describe how the Nextcloud application and database containers should run. The main difference is that Bash performs command line tasks, while Docker Compose defines the setup of container services.

### 4. How has your understanding of cloud computing changed from Lab 1 to Lab 9?

My understanding of cloud computing has become broader throughout the semester. I learned about setting up infrastructure, deploying applications, managing data, monitoring resources, securing systems, and automating tasks. Each laboratory introduced different tools and responsibilities. I now understand better how these parts work together to support cloud services.

### 5. Which cloud computing role did you enjoy most, and why?

The role I enjoyed most was Cloud Deployment Engineer because I found it interesting to learn how applications and their supporting services can be set up together. Working with Docker Compose helped me understand how containers can make application deployment more organized. I would like to improve my skills in this area because deployment is an important part of making applications available to users.
