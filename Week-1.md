# Week 1

## Resources
- Getting Started: https://docs.docker.com/get-started/
- Dockerfile Reference: https://docs.docker.com/engine/reference/builder/
- Volumes and Persistent Storage: https://docs.docker.com/storage/volumes/
- Networking in Docker: https://docs.docker.com/network/
- Best Practices: https://docs.docker.com/engine/security/
- Compose: https://docs.docker.com/compose/compose-file/

## Tasks

### 1. Make a docker file
1. Create a basic flask todo app
2. Use sqlite as db
3. Use volumes to made data persistent
4. use `gunicorn` instead of flask run
5. Bind mount code to edit without rebuilds
6. Make the flask app show a different page based on env variables
7. Pass these variables using `docker run`
8. Understand how this can be used for debugging and testing

### 2. Perm management 
1. Make a netcat shell in docker
2. Setup appropriate permisions so that user can't break the container
3. Allow user to edit files in `/home` without being able to break things
4. Try escaping the container, find out what you can/cannot do

### 3. Networking
1. Setup 2 netcat shell containers
2. Set them up on the same docker network
3. Assign IP addresses next to each other
4. Connect to one container using the other
5. Use docker compose to setup and destroy the network and the containers

### 4. Extra credit (Optional)
1. Learn about podman: https://podman.io/
2. Understand and explain why its different from docker
3. Redo tasks using podman, reporting the changes made
