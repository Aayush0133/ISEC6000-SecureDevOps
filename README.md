# ISEC6000 SecureDevOps

## Project Overview

In this **ISEC6000 SecureDevOps** project, I focused on building, deploying, and securing a microservices-based e-commerce application. The application, Saleor, is an open-source e-commerce solution built on a microservices architecture. My goal was to demonstrate my skills in deploying and securing a modern e-commerce application using tools like Docker, Kubernetes, and Google Kubernetes Engine (GKE).

## Project Goals

1. **Design and Deploy a Scalable Microservices Architecture:**
   - I utilized Kubernetes and Docker to deploy the Saleor application, ensuring that it is scalable and that each component is isolated and manageable.

2. **Implement Robust Security Measures:**
   - I secured Docker containers by following best practices, scanning for vulnerabilities, and applying runtime security measures.

3. **Integrate Continuous Monitoring and Logging:**
   - I set up monitoring and logging solutions to provide real-time insights and ensure proactive issue resolution.

4. **Document and Share My Work:**
   - I created detailed documentation, including setup instructions, configurations, and security measures, to share the process and results.

## Prerequisites

- **Google Cloud Account:** I ensured that I had access to Google Cloud Platform.
- **Google Kubernetes Engine (GKE) Setup:** I was familiar with creating and managing GKE clusters.
- **Docker:** I had a basic knowledge of Docker for containerizing applications.
- **Kubernetes:** I understood Kubernetes for deploying and managing containerized applications.
- **Git:** I used Git for version control.

## Setup Instructions

1. **Create a Kubernetes Cluster:**
   - I used Google Cloud Console or `gcloud` CLI to create a Kubernetes cluster with the appropriate settings.
   - Example command:
     ```bash
     gcloud container clusters create saleor-cluster --location us-central1 --num-nodes 3 --machine-type e2-small
     ```

2. **Configure `kubectl`:**
   - I configured `kubectl` to interact with my cluster.
   - Example command:
     ```bash
     gcloud container clusters get-credentials saleor-cluster --location us-central1
     ```

3. **Clone the GitHub Repository:**
   - I cloned the repository to my local machine.
   - Example command:
     ```bash
     git clone https://github.com/yourusername/ISEC6000-SecureDevOps.git
     ```

4. **Deploy Saleor:**
   - I modified the Docker Compose file as needed and deployed Saleor using Kubernetes manifests.
   - Example command:
     ```bash
     kubectl apply -f saleor-deployment.yaml
     ```

## Usage

- **Access Saleor Dashboard:**
  - Once deployed, I accessed the Saleor Dashboard at:
    ```plaintext
    http://<Your-Server-IP>:9002
    ```

## Security Measures

1. **Container Security:**
   - I configured Docker containers to run as non-root users.
   - I set resource limits and used secure base images.

2. **Vulnerability Scanning:**
   - I used tools like Trivy to scan container images for vulnerabilities.
   - Example command:
     ```bash
     trivy image <your-image>
     ```

## Continuous Monitoring and Logging

1. **Set Up Monitoring:**
   - I implemented monitoring tools like Prometheus and Grafana.
   - I configured alerts and dashboards for real-time insights.

2. **Configure Logging:**
   - I set up centralized logging with tools like ELK Stack or Google Cloud Logging.
   - I ensured that logs were collected and stored securely.

## Contribution

- **Fork the Repository:**
  - I forked this repository on GitHub to make my own changes and contributions.
  

## Documentation

- **Project Documentation:**
  - Detailed documentation is provided in the project report.

## Contact

- **Full Name:** Aayush Bhattarai
- **Student ID:** 21448827

