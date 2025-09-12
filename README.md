# docker-ghcr-project

This project provides a Docker container for running R with the Bioconductor `bambu` package. It includes all necessary files for building the Docker image and deploying it to GitHub Container Registry.

## Project Structure

- **Dockerfile**: Contains instructions for building the Docker container, including the base image and package installations.
- **.github/workflows/docker-publish.yml**: Defines the GitHub Actions workflow for building and publishing the Docker image to GitHub Container Registry.
- **.dockerignore**: Specifies files and directories to be ignored by Docker during the build process.
- **README.md**: Documentation for the project, including build and deployment instructions.
- **LICENSE**: Licensing information for the project.

## Building the Docker Container

To build the Docker container, navigate to the project directory and run the following command:

```
docker build -t your-image-name .
```

Replace `your-image-name` with the desired name for your Docker image.

## Deploying to GitHub Container Registry

The project includes a GitHub Actions workflow that automatically builds and publishes the Docker image to GitHub Container Registry when changes are pushed to the main branch. Ensure that you have set up the necessary secrets in your GitHub repository for authentication.

## License

This project is licensed under the terms specified in the LICENSE file.