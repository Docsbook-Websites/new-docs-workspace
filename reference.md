```yaml
title: "Nimbus CLI Command Reference for Container Deployment"
description: "Master Nimbus CLI commands for efficient container deployment and management. Streamline your workflow with this comprehensive reference."
---

# Nimbus CLI Command Reference

This reference provides a detailed overview of the commands and parameters available in Nimbus CLI, designed for deploying containers efficiently.

## Container Management Commands

| Parameter/Command         | Type            | Description                                           | Example                          |
|---------------------------|-----------------|-------------------------------------------------------|----------------------------------|
| `nimbus deploy`           | Command         | Deploys a container from a specified image.          | `nimbus deploy my-app:latest`   |
| `nimbus list`             | Command         | Lists all deployed containers.                        | `nimbus list`                    |
| `nimbus remove`           | Command         | Removes a specified container from deployment.       | `nimbus remove my-app`           |
| `nimbus status`           | Command         | Displays the status of a specified container.        | `nimbus status my-app`           |

## Image Management Commands

| Parameter/Command         | Type            | Description                                           | Example                          |
|---------------------------|-----------------|-------------------------------------------------------|----------------------------------|
| `nimbus pull`             | Command         | Pulls a container image from a registry.             | `nimbus pull my-image:latest`    |
| `nimbus tag`              | Command         | Tags a local image with a new name.                  | `nimbus tag my-image:latest my-image:v1` |
| `nimbus push`             | Command         | Pushes a local image to a specified registry.        | `nimbus push my-image:v1`        |

## Configuration Commands

| Parameter/Command         | Type            | Description                                           | Example                          |
|---------------------------|-----------------|-------------------------------------------------------|----------------------------------|
| `nimbus config set`       | Command         | Sets a configuration parameter for Nimbus CLI.       | `nimbus config set region us-west-1` |
| `nimbus config get`       | Command         | Retrieves the current configuration settings.         | `nimbus config get`              |

## Networking Commands

| Parameter/Command         | Type            | Description                                           | Example                          |
|---------------------------|-----------------|-------------------------------------------------------|----------------------------------|
| `nimbus network create`   | Command         | Creates a new network for container communication.    | `nimbus network create my-network` |
| `nimbus network list`     | Command         | Lists all available networks.                         | `nimbus network list`            |
| `nimbus network remove`   | Command         | Removes a specified network.                          | `nimbus network remove my-network` |

## Volume Management Commands

| Parameter/Command         | Type            | Description                                           | Example                          |
|---------------------------|-----------------|-------------------------------------------------------|----------------------------------|
| `nimbus volume create`    | Command         | Creates a new volume for container storage.          | `nimbus volume create my-volume` |
| `nimbus volume list`      | Command         | Lists all available volumes.                          | `nimbus volume list`             |
| `nimbus volume remove`    | Command         | Removes a specified volume.                           | `nimbus volume remove my-volume`  |

Utilize this reference to enhance your deployment workflow with Nimbus CLI, ensuring efficient container management tailored for developers and DevOps engineers.
```