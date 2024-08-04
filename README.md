

# Docker WordPress Setup

![Owner Avatar](https://avatars.githubusercontent.com/u/USER_ID)

Easily set up and host a WordPress site on your local machine using Docker Compose. This project provides a seamless configuration to get you started quickly.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
  - [Clone the Repository](#clone-the-repository)
  - [Navigate to Project Directory](#navigate-to-project-directory)
  - [Start the Services](#start-the-services)
- [Accessing WordPress](#accessing-wordpress)
- [Managing the Services](#managing-the-services)
  - [Stopping the Services](#stopping-the-services)
  - [Viewing Logs](#viewing-logs)
  - [Restarting the Services](#restarting-the-services)
- [Conclusion](#conclusion)

## Introduction

This project leverages Docker Compose to create a local WordPress development environment. It includes a MySQL database service and a WordPress service configured to work together seamlessly.

## Features

- **Quick Setup**: Get your WordPress site up and running in minutes.
- **Persistent Data**: Data is stored persistently using Docker volumes.
- **Easy Management**: Easily start, stop, and manage your WordPress and MySQL services.

## Prerequisites

Before you begin, ensure that you have Docker and Docker Compose installed on your machine. You can download and install them from the [official Docker website](https://www.docker.com/get-started).

## Setup Instructions

### Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/KIRAN-KUMAR-K3/vulnweb-docker.git
```

### Navigate to Project Directory

Navigate into the project directory:

```bash
cd vulnweb-docker
```

### Start the Services

Start the WordPress and MySQL services using Docker Compose:

```bash
docker-compose up -d
```

The `-d` flag runs the containers in detached mode, allowing you to continue using your terminal.

## Accessing WordPress

Once the services are up and running, you can access your WordPress site by opening your web browser and navigating to:

```
http://localhost
```

## Managing the Services

### Stopping the Services

To stop and remove the services, use the following command:

```bash
docker-compose down
```

This command stops the containers and removes the associated networks but preserves the volumes for persistent data.

### Viewing Logs

If you need to view the logs for any of the services, use:

```bash
docker-compose logs
```

You can also view logs for a specific service by specifying the service name:

```bash
docker-compose logs wordpress
```

### Restarting the Services

To restart the services, first stop them and then start them again:

```bash
docker-compose down
docker-compose up -d
```

## Conclusion

This Docker Compose setup provides an efficient way to run a WordPress site with a MySQL database locally. With Docker Compose, you can easily manage the services, ensuring a smooth and hassle-free development experience.

For any further assistance or questions about the project, feel free to reach out. Happy coding!
