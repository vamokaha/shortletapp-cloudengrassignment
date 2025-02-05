# shortletapp-cloudengrassignment
This project aims to answer the following 
 
 Implement CI/CD Pipeline design using GitHub Actions pipeline that aims to:
 ● Runs Terraform to provision all required infrastructure, including Kubernetes resources.
 ● Builds the Docker image for the API.
 ● Deploys the API to the GKE cluster as part of the Terraform  deployment.
 ● Verifies that the API is accessible by running a test that hits the API endpoint and checks the response.

Suggestion/Prerequisites
GitHub Repository:

Ensure you have a GitHub repository (example vamokaha/shortletapp-cloudengrassignment.git)
Ensure you have appropriate permissions to push changes and configure GitHub Actions.

Google Cloud Platform (GCP) Account:
Ensure your GCP account is properly set up, and you have a service account with the necessary permissions (e.g., to manage GKE, IAM roles, and other infrastructure).

Docker Hub or Google Container Registry (GCR):
Ensure you have an account on Docker Hub or GCR where the Docker image will be pushed.
Obtain credentials (username, password, or service account JSON key) for the registry.

Terraform Configuration:
Have a working Terraform configuration in your repository to provision the required infrastructure, including GKE, networking, IAM roles, and Kubernetes resources.

Dockerfile:
Ensure you have a Dockerfile in your repository for building the API Docker image.

GitHub Secrets:
Set up the following secrets in your GitHub repository:
    GCP_PROJECT_ID: Your GCP project ID.
    GCP_CREDENTIALS: The base64 encoded contents of your GCP service account key JSON.
    DOCKER_USERNAME: Your Docker Hub or GCR username.
    DOCKER_PASSWORD: Your Docker Hub or GCR password or service account key.