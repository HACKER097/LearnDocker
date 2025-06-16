# Intro

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


## Instructions

1. Create a public github repo for these tasks
2. For each week, create `Week-N/README.md`, use headings and subheadings for each task and subtask
3. For each subtask
  1. write the commands used
  2. relevant output/screenshots
  3. Problems faced if any
  4. Interesting observations
4. Include your final `Dockerfile`/`docker-compose.yaml` in codeblocks
5. Include comments explaining each line, skip if explained before
6. Include the files for each task in folders `Week-N/Task-N`
