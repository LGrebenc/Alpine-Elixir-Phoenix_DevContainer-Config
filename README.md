# Alpine-Elixir-Phoenix_DevContainer-Config
Configuration files for an Alpine Linux based dev container, for [Elixir](https://elixir-lang.org/)/[Phoenix framework](https://www.phoenixframework.org/) development. Using the base Alpine dev container [image](https://mcr.microsoft.com/en-us/product/devcontainers/base/about), a Dockerfile to install Elixir, Phoenix framework, and their dependencies, and docker-compose to bring postgresql into the mix (a requirement of the Phoenix Framework).

## Requirements:
- [Docker](https://docs.docker.com/get-docker/)
- [Visual Studio Code](https://code.visualstudio.com/download/)
- The [Dev Container extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## How to use:
Details on how to create dev containers can be found within [Microsoft's guide](https://code.visualstudio.com/docs/devcontainers/create-dev-container). For the best and most thorough documentation and instruction it would be best to look to Microsoft's guide.

### The gist: 
The configuration files define how the dev container is to be built. The file that is used to do this is the devcontainer.json. It defines what is being built, where that is to be pulled from. In the case of this configuration, it points to a Dockerfile and docker-compose.yml the which are used to customize the container.

To build the container clone or download the .devcontainer configuration files to the directory you wish to use for the container and open that directory with vscode. With their [dev container extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) installed and enabled toggle the Command Palette (ctrl + shift + p) then typing and choose option 'dev containers: open folder in Container'. With this vscode will build the container (if it hasn't been built yet) and open the folder in vscode within the container. From here you should be good to develop.

\*More details to come, as this repo gets fleshed out.\*

## Acknowlegements and Thanks:
All of this was made possible by the dev container folks (check them out at their [github](https://github.com/devcontainers) 
 or [website](https://containers.dev/)). In particular their [guide](https://containers.dev/guide/dockerfile) on creating dev containers using images, dockerfiles, and docker compose was incredibly useful. This dev container config was made standing on their shoulders.
