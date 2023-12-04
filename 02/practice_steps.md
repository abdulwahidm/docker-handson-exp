# Practice Stpes

This folder contains files related to a hands-on Docker experience. The folder `02` includes several files to demonstrate Dockerfile creation, containerization, and basic scripting. Below are the explanations for each file:

## 1. Dockerfile

The `Dockerfile` defines the steps to build a Docker image. It uses the base image from Ubuntu, installs necessary packages (`curl` and `bash`), and sets up the entrypoint script. The entrypoint script is copied into the image, and the container is configured to run this script when started.

## 2. entrypoint.bash

The `entrypoint.bash` script is the entry point for the Docker image. It performs the following tasks:
- Checks if the current Bash version is 5.
- Verifies the installation of Curl.
- Retrieves the current date and time from Google.
- Displays a greeting message along with the current date and time.

## 3. server.bash

The `server.bash` script is a simple Bash script to simulate a server. It performs the following tasks:
- Checks if the current Bash version is 5.
- Starts a simple server (infinite loop) and prints a message.

## 4. server.Dockerfile

The `server.Dockerfile` demonstrates another Dockerfile for creating a server image. It uses the base image from Ubuntu, installs Bash, and sets up the server script as the entrypoint.

## Practice Steps:

1. **Build the Docker image using the Dockerfile:**
   ```bash
   docker build -t my-docker-image -f Dockerfile .
