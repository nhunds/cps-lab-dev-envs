# Devcontainer for CPS Lab Dev Environments

This devcontainer is designed for developing Docker images and Devcontainer Features for the CPS Lab Dev Environments project.

## Features

- **Base Image**: Uses the official `mcr.microsoft.com/devcontainers/universal:linux` image, which includes a wide range of tools and runtimes.
- **Docker-in-Docker**: Enables Docker CLI and Docker-in-Docker for building and testing Docker images.
- **Extensions**: Includes VSCode Docker and Remote Containers extensions for seamless integration.

## Usage

1. Open this repository in VSCode with the Remote Containers extension.
2. The devcontainer will automatically build and start.
3. Use the integrated terminal to run Docker commands and develop Devcontainer Features.

## Extensions

- **VSCode Docker**: Provides Docker integration in VSCode.
- **Remote Containers**: Enables seamless development in a containerized environment.

## Post-Create Command

The devcontainer runs a simple echo command to confirm it is ready for development:

```bash
echo 'Devcontainer ready for Docker and Devcontainer Features development.'
```

## Customization

To customize the devcontainer, edit the `.devcontainer/devcontainer.json` file. You can add additional features, extensions, or settings as needed.
