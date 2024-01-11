# UIC-CS411-Environment
Development container configuration for UIC's Spring 2024 CS-411

## Prerequisites
1. [Docker](https://www.docker.com/get-started/)
2. [Visual Studio Code](https://code.visualstudio.com/Download)
3. [Dev Containers Extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
4. [Local Clone of this Repository](https://github.com/garrettpfoy/UIC-CS411-Environment)

## How to Run
*Assuming you've installed all the requirements listed above, open this repository (or any repository with the .devcontainer folder and configuration in its root folder) in Visual Studio Code*

1. Open Command Pallete (Control + Shift + P) or (Command + Shift + P)
2. Type "Open Folder in Container" or "Rebuild and Reopen in Container"
3. Wait for the installation and download to complete
4. You should be all set!

## Adding Dependencies
*As the course progresses, it is almost a certainty we will need to include additional packages installed from PIP in our development environment, follow the below steps to add packages to the initial build of the environment*

1. Install the library using `pip install [package-name]` in your development environment
2. Run `pip freeze > requirements.txt`, which overwrites the current requirement list (with versions) with your latest environment's dependencies
3. Rebuild the container, the Dockerfile will automatically install all dependencies listed in the `requirements.txt` file
