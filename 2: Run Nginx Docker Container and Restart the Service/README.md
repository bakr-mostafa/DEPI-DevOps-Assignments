# Assignment 2: Run Nginx Docker Container and Restart the Service

## Description
In this assignment, I ran an Nginx Docker container and made it accessible via a browser. I then accessed the container and restarted the Nginx service.

## Steps Followed

### 1. **Run an Nginx Container and Make it Accessible Through Your Browser**

- Pulled the Nginx Docker image from Docker Hub:
    ```bash
    docker pull nginx
    ```

- Ran the Nginx container in detached mode and mapped the host port 8080 to container port 80:
    ```bash
    docker run -d -p 8080:80 --name nginx-container nginx
    ```

- Verified that the container was running using:
    ```bash
    docker ps
    ```

- Opened a browser and navigated to `http://localhost:8080` to confirm that the default Nginx page was visible.

### 2. **Enter the Nginx Container and Restart the Nginx Service**

- Accessed the running Nginx container:
    ```bash
    docker exec -it nginx-container bash
    ```

- Restarted the Nginx service using the `nginx -s reload` command:
    ```bash
    nginx -s reload
    ```

- Exited the container:
    ```bash
    exit
    ```
