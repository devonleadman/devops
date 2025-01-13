# Techstack
- Dynatrace: system monitoring
- Harness: CI/CD pipelines
- Gitlab: Automated software delivery
- Docker: containerization
- AWS ECR & ECS: Docker container registry and deployment

# General Process
- Store codebase on Gitlab
- Gitlab runs tests on code
- Gitlab builds a Docker image
- Gitlab sends image to AWS ECR
- Harness retrieves the stored image from AWS ECR
- Harness deploys the retrieved image to the AWS ECS environment
- Dynatrace monitors the AWS EC2 environment for errors/issues
