# Linux-Podman-basics

## Preqrequisites

0. On Windows make sure you have WSL installed:
https://learn.microsoft.com/en-us/windows/wsl/install

1. Also, on Windows make sure you have enabled [hyper-v](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v) before trying to install Docker.

2. Install Docker - https://docs.docker.com/engine/install/ for your OS.

3. On Windows use the WSL terminal.

4. Pro tip: Better use Linux instead of Windows.

5. Bonus: Better use Podman instead of Docker.

## Lab environment

To launch the notebook server for this lab:
### Bash
```
docker run --name linux-basics -d -v "$(pwd)"/lab:/usr/project/lab:Z -p 8888:8888 adrianbranescu93/jupyter-node
```

```
docker run --name linux-basics-interactive --rm -it --entrypoint /bin/bash -v "$(pwd)/lab":/usr/project/lab:Z adrianbranescu93/jupyter-node
```

### PowerShell
```
docker run --name linux-basics -d -v "$pwd\lab:/usr/project/lab" -p 8888:8888 adrianbranescu93/jupyter-node
```

```
docker run --name linux-basics-interactive --rm -it --entrypoint /bin/bash -v "$pwd\lab:/usr/project/lab" adrianbranescu93/jupyter-node
```
