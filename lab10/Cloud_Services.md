## Artifact registries

- AWS Elastic Container Registry (ECR):<br>
  - It is perfect if you want to integrate your service with other Amazon products such as  AWS Amazon ECS and Amazon EKS
  - Lifecycle policies allow to automate cleanup of unused images and automate your storage
  - Image Vulnerability Scanning to make you project more secure
  - It ensures that the containers are encrypted 
  
- Google Cloud Container Registry:
  - Easy to integrate with the Google services such as Google Kubernetes Engine
  - It also supports secure distribution and storage of docker images
  - Containers are competible with Docker
  - Audit loggings helps you to keep track of the changes to the containers

- Azure Container Registry
  - Integration with other Microsoft services
  - Geo-replication lets you replicate images across multiple Azure regions

## Serverless Computing Platforms
- AWS Lambda (AWS):
  - Very popular solution with lots of free to use materials on the Internet to get handy with it
  - Integrates well with the other Amazon services
  - Automatically scales based on the load
  - Supports multiple programming languages
  - Event-driven approach  
- Google Cloud Functions (GCP):
  -  Also scales based on the load
  -  Also supports many programming languages such as Node.js, Python, Go, Ruby, and many others
  -  You pay only for the resources that you use
  -  Supports versioning and rollbacks
- Azure Functions (Azure):
  - All the other comman features as listed in the other services
  - Built in logging and monitoring
  - Authentication and Authorization due to the integration with the Active directory
- AWS App Runner (AWS):
  - Integration with the other Amazon services
  - Great degree of automatization of the building, deploying and scaling processes
- Google Cloud Run (GCP):
 - Obviously integrates well with the Google services
 - Lets you deploy and manage docker containers
