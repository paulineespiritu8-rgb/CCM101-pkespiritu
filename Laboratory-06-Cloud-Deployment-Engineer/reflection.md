# Mission 6 Reflection

Writing a `docker-compose.yml` file makes a cloud engineer’s job easier because multiple containers can be configured and deployed from a single file. Instead of typing many commands manually, the deployment process becomes faster, more organized, and easier to repeat. It also helps reduce mistakes when setting up applications.

If there is an indentation error in a YAML file, Docker Compose may not be able to read the configuration correctly. Since YAML is space-sensitive, even a small formatting mistake can cause deployment errors or prevent the application from starting. This is why checking the spaces and indentation is important.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_HOST` were used to provide configuration settings for the containers. They help applications communicate with each other and make configuration easier to manage. They also allow the containers to use the correct database settings.

Deploying a fully functional enterprise cloud storage system in just a few minutes felt rewarding and exciting. It demonstrated how containerization and cloud technologies can simplify complex deployments. I also felt happy because I was able to understand how Nextcloud and MariaDB work together in one application.

Since Mission 1, my understanding of Cloud Computing has improved significantly. I have learned about cloud services, containerization, data storage, networking, and Infrastructure as Code. This mission helped me understand how these concepts work together to deploy and manage modern cloud applications efficiently. I also learned the importance of proper configuration and checking whether containers are running correctly. Overall, this activity gave me more experience using Docker Compose and helped me understand how cloud engineers can manage multiple services more easily.
