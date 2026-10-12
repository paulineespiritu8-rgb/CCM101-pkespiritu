# Mission Reflection

Checking the host server's resources is important even if containers are running perfectly because all containers share the host's CPU, memory, and disk space. If the host does not have enough resources when traffic increases, the containers will slow down or stop working. Knowing the baseline first makes sure the server can handle more users without crashing.

If a user cannot log into the web application, the docker logs command helps by showing the full request and response. It shows if the login request reached the server, if there was an error message, or if the request failed entirely. This makes it clear exactly what went wrong instead of guessing.

Monitoring logs and monitoring metrics are different: logs are records of individual events such as requests and errors that show what happened. Metrics are measurements like CPU percentage and memory usage that show how the system is performing over time. Logs help find specific problems; metrics help see the overall health and performance of the system.

Large enterprise companies monitor thousands of containers at the same time using tools like Prometheus and Grafana. Prometheus collects metrics from all containers automatically. Grafana displays the data on dashboards so teams can see everything in one place. These tools also send alerts when something is not working right, so problems are found quickly.

My ability to troubleshoot Linux environments has improved because I now know which commands to use and in what order. I start by checking the host system resources before looking at the application. I can read logs to find errors and use metrics to check performance. I feel more confident using the terminal and I know where to look to find the cause of an issue.
