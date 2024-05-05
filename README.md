# Emart App

Welcome to the Emart App repository. This project uses Docker and Docker Compose to manage and run the application. This README will guide you through setting up the app, running it, and cleaning up the environment.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Setup and Run](#setup-and-run)
- [Accessing the App](#accessing-the-app)
- [Clean Up](#clean-up)
- [Troubleshooting](#troubleshooting)

## Prerequisites

Before getting started, ensure you have the following installed on your system:

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Setup and Run

Follow the steps below to set up and run the Emart App:

1. **Clone the repository**:

    ```shell
    git clone https://github.com/devopshydclub/emartapp.git
    cd emartapp/
    ```

2. **Bring up the containers**:

    To start the application, use Docker Compose:

    ```shell
    docker compose up -d
    ```

3. **Check the running containers**:

    Ensure the containers are running:

    ```shell
    docker compose ps
    ```

4. **List all Docker containers**:

    ```shell
    docker ps -a
    ```

## Accessing the App

Once the application is running, you can access it using a web browser:

1. Find the IP address of your system or the VM running the Docker containers:

    ```shell
    ip addr show
    ```

2. Open a web browser and navigate to `http://<IP>:80`, replacing `<IP>` with the IP address you found in the previous step.

## Clean Up

To stop and clean up the application:

1. **Stop the Docker containers**:

    ```shell
    docker compose down
    ```

2. **Remove unused Docker resources**:

    ```shell
    docker system prune -a
    ```

This will stop the application and remove unused Docker resources, freeing up space on your system.

## Troubleshooting

If you encounter issues while running the app, consider the following:

- **Check logs**: View logs to diagnose issues with the containers:

    ```shell
    docker compose logs
    ```

- **Check network**: Ensure your network settings allow for communication between your browser and the application.

- **Review Docker Compose file**: Make sure the `docker-compose.yaml` file is correctly configured.

For more detailed troubleshooting steps, refer to the [Docker documentation](https://docs.docker.com/) or open an issue on the [GitHub repository](https://github.com/devopshydclub/emartapp/issues).

## Contributing


If you would like to contribute to this project, please open a pull request or submit an issue.

Happy coding!


![image](https://github.com/YoussefTarek2911/E-mart_App/assets/108703940/78b7868f-43ac-4779-946c-33eb7cacc28a)

