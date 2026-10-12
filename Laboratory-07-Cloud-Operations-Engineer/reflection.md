# Reflection

This laboratory activity gave me an opportunity to examine a Linux server and observe how a Dockerized website behaves. I learned that checking an application through a browser is not enough to understand its overall condition. System information, logs, and resource measurements provide additional details that can help explain what is happening behind the scenes.

**1. Why is it important to check the host server's resources even if your containers are running perfectly?**

The host provides the resources that containers need to operate. Even if an application is currently working, low memory, limited disk space, or heavy CPU usage could affect its performance later. Checking the host helps identify these limitations early.

**2. If a user complains that they cannot log into a web application, how would the `docker logs` command help you solve the problem?**

I would inspect the container logs for messages related to the time the user experienced the issue. If the application records authentication errors, database failures, or other warnings, those entries may help me determine what needs further investigation.

**3. What is the difference between monitoring logs and monitoring metrics?**

Logs provide individual records of events, such as web requests and error responses. Metrics are measurements collected over time, including CPU and memory usage. Logs help investigate specific incidents, while metrics help assess resource consumption and performance trends.

**4. How do you think large enterprise companies monitor thousands of containers at the same time?**

They can use centralized monitoring platforms to gather data from many servers and containers. Prometheus can collect and store metrics, while Grafana can display those measurements in dashboards so technical teams can spot unusual conditions and respond to alerts.

**5. How has your ability to troubleshoot Linux environments improved?**

I am more familiar with choosing commands based on the information I need. I can check memory and disk capacity, observe processes, inspect Docker logs, and review container statistics. This gives me a more organized way to investigate problems and support my conclusions with command output.

Overall, I learned that reliable cloud operations require regular observation and evidence-based troubleshooting. I can apply these practices to future projects by checking the system first, investigating application activity, and reviewing resource usage before deciding what action to take.

