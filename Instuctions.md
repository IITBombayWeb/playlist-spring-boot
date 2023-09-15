# Instructions for Testing the Application

**Objective**: Evaluate the deployment of the Java application using Docker within a professional context.

## Instructions

### Application Code

1. Develop the application code according to the specifications provided.
2. Ensure that the application is complete and functional before proceeding to the next steps.

### Docker Installation and Image Creation

1. Install Docker on your local machine. You can download it from the [official Docker website](https://www.docker.com/get-started).
2. Using Docker, create a Docker image of your application.

### DockerHub Account and Repository

1. Create an account on [DockerHub](https://hub.docker.com/).
2. Once you have an account, create a public repository. It's important that the repository is public to facilitate seamless evaluation.
3. You will receive a Dockerfile for image creation.
4. Push the Docker images you created for frontend and backend in the previous step to this newly created repository.

## GitHub Actions Workflow for Docker Image Creation

To automate the Docker image creation using GitHub Actions, follow these steps to set up the necessary workflow:

1. In your GitHub repository, create a `.github/workflows` directory if it doesn't exist.
2. Inside the `.github/workflows` directory, create a YAML file, e.g., `docker-build.yml`.
3. Store sensitive information or secret variables in GitHub repository settings under "Secrets." These secrets can be accessed in your workflows as environment variables

### Docker Compose

1. You will receive a Docker Compose file.
2. Open the Docker Compose file and specify the image name of the Docker images you pushed to DockerHub in the appropriate section of the file.

## Evaluation Criteria

Your performance will be evaluated based on the following criteria:

- **Correctness**: The application should run without errors or issues. It should be accessible at the specified port on localhost.
- When initiating the 'docker-compose up' command, the orchestration process will automatically retrieve the required Docker images for the frontend, backend, and database components from DockerHub. Subsequently, it will initiate the application, making it accessible on the local host. This procedure facilitates the thorough evaluation of the application's functionality

## Need to Submit

- GitHub Repository Link:
- Comprehensive Process Documentation:


