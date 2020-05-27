# docker_dev_environment

Development environment as docker container. Use in projects by copying `Dockerfile` and `run` to the respective directory (or add to path, for convenience). That means, the command is passed to docker: the command runs in the current directory but within the image. Docker does not copy your code to the image: everything is read and stored in the current directory.

**Prerequisites**

- A working docker installation under Linux, macOS or related system
- Bash

**Usage**

Start docker daemon:
```
sudo systemctl restart docker
```

Then run any command, e.g.,
```
./run 'mvn --version'
```

To cleanup use `docker system prune`.
