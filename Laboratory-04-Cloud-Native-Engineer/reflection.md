## Mission Reflection

### 1. How does booting a Docker container compare to installing an OS on a VM?

A Docker container starts faster because it does not need to boot a complete operating system. A VM requires its own Guest OS, while a container uses the Host OS. This makes containers lighter and faster to start.

### 2. Why is -p 8080:80 necessary?

The -p 8080:80 option connects port 8080 on the host machine with port 80 inside the container. Nginx uses port 80, so this mapping allows the web server to be accessed through http://localhost:8080.

### 3. What happens to data inside the container when you run docker rm?

The container is removed when docker rm is executed. Data that exists only inside the removed container is no longer available. This means important data should be stored separately when it needs to persist.

### 4. How does containerization change DevOps collaboration?

Containerization provides a consistent environment that can be shared between development and operations teams. Packaging an application in a container can help reduce differences between environments and make deployment more consistent.

### 5. How is your GitHub portfolio evolving as you complete more cloud computing activities?

My GitHub portfolio is becoming a collection of my completed cloud computing activities. Through this laboratory, I am documenting my experience with Docker, containers, Nginx, and container management. The portfolio also provides evidence of the skills I am learning through practical activities.
