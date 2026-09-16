## Mission Reflection

A Docker container starts faster because it does not need to install or boot a complete operating system. A VM has its own Guest OS, while a container shares the Host OS. Because of this, containers use fewer resources and can start in seconds. This makes them useful for applications that need to run quickly.

The `-p 8080:80` connects port 8080 of the host machine to port 80 of the container. Nginx uses port 80, so this allows us to open the web server using `http://localhost:8080`. Without the port mapping, we would not be able to access Nginx through port 8080 as required in the activity.

When `docker rm` is used, the container is completely removed. Any data stored only inside that container will also no longer be available. For important data, it should be stored separately so it can still be used even after the container is removed. In this activity, we remove the Nginx container after stopping it.

Containerization gives developers and operations teams a similar environment to work with. This can reduce differences between development and deployment setups. It also makes it easier to share, test, and run the same application environment. Because of this, teams can work together more consistently.

My GitHub portfolio is growing as I complete more cloud computing activities. In this laboratory, I added my work with Docker, containers, Nginx, and container management. It also shows the skills I learned through hands-on practice. Each laboratory adds more evidence of my progress and helps organize my cloud computing projects.
