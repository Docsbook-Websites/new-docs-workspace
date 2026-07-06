---
title: How to Deploy Your First Container with Nimbus CLI
description: Deploy your first container using Nimbus CLI in just a few steps. Streamline your container management process today.
---

# How to Deploy Your First Container with Nimbus CLI

Follow these steps to deploy your first container using Nimbus CLI. This guide assumes you have Nimbus CLI installed and configured on your system.

## Step 1: Open Your Terminal

Launch your terminal application. Ensure you have access to Nimbus CLI by typing the following command:

```bash
nimbus --version
```

If you see the version number, you are ready to proceed.

## Step 2: Log in to Your Container Registry

Use the following command to log in to your container registry. Replace `your-registry-url` with the URL of your container registry.

```bash
nimbus login your-registry-url
```

Enter your username and password when prompted. Successful login will allow you to push and pull containers.

## Step 3: Create a Dockerfile

In your project directory, create a file named `Dockerfile`. This file contains instructions for building your container image. Here’s a simple example:

```dockerfile
FROM node:14
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "index.js"]
```

This Dockerfile sets up a Node.js application. Adjust the content based on your application requirements.

## Step 4: Build Your Container Image

Run the following command to build your container image. Replace `your-image-name` with a name for your image.

```bash
nimbus build -t your-image-name .
```

This command compiles the Dockerfile and creates a container image. Check for any errors during the build process.

## Step 5: Push Your Image to the Registry

After building the image, push it to your container registry using:

```bash
nimbus push your-registry-url/your-image-name
```

This command uploads your image to the specified registry. Verify the upload by checking your registry dashboard.

## Step 6: Deploy Your Container

Now, deploy your container using the following command. Replace `your-container-name` with a name for your container.

```bash
nimbus deploy your-registry-url/your-image-name --name your-container-name
```

This command starts your container based on the image you pushed. Monitor the deployment process for any issues.

## Step 7: Verify Your Deployment

To ensure your container is running, execute:

```bash
nimbus ps
```

This command lists all running containers. Check that your container appears in the list and is in a healthy state.

## Step 8: Access Your Application

If your application exposes a port, access it via your browser or API client. Use the appropriate URL, typically `http://localhost:your-port`.

Congratulations! You have successfully deployed your first container using Nimbus CLI.

---

### Related

- [Nimbus CLI Documentation](https://nimbuscli.com/docs)
- [Docker CLI Overview](https://docs.docker.com/cli/)
- [Kubernetes Quick Start Guide](https://kubernetes.io/docs/setup/quick-start/)
- [OpenShift Deployment Guide](https://docs.openshift.com/container-platform/latest/developing_apps/deployments/deployment.html)