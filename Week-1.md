# Week 1

This is supposed to be an intro to practical use of docker and the tools it has to offer. Read the docs, they are very good. Avoid using AI for these tasks, the intention is not to get stuff done, but to learn docker. If you must, use AI as a search engine, or explainer for things that are unclear to you in the docs.

## Recommendations
- Avoid Docker Desktop
  - Docker might be useful tool, but its also a product. They will try to sell you shit.
  - Docker GUI and DockerHub usage is pushed heavily in the docs. Avoid them and learn the cli.
  - Tools like `lazydocker` are helpful, if you use it, make sure you understand what commands it runs under the hood. 
- Use linux
  - Docker on Windows uses a hidden linux VM, which is slow and annoying.
  - Networking is different
  - Just runs better on linux
  - Why are you trying to learn DevOps if you arn't using linux?
- Explore
  - Get inside the Docker container and see whats really going on
  - Try to `rm -rf *` and see what happens
  - Try breaking things then fixing them
- Build Muscle Memory
  - Once you are done with a task, delete the image and redo it without looking at notes
  - Tasks are small, once you have learned, you can be done in less than 10 min


## Resources
- Getting Started: https://docs.docker.com/get-started/
- Dockerfile Reference: https://docs.docker.com/engine/reference/builder/
- Volumes and Persistent Storage: https://docs.docker.com/storage/volumes/
- Networking in Docker: https://docs.docker.com/network/
- Best Practices: https://docs.docker.com/engine/security/
- Compose: https://docs.docker.com/compose/compose-file/

## Instructions

1. Create a public github repo for these tasks
2. Create `Week-1/README.md`, use headings and subheadings for each task and subtask
3. For each subtask
  - write the commands used
  - relevant output/screenshots
  - Problems faced if any
  - Interesting observations
4. Include your final `Dockerfile`/`docker-compose.yaml` in codeblocks
5. Include comments explaining each line, skip if explained before
6. Include the files for each task in folders `Week-1/Task-1`

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
