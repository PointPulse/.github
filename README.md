# Ascenda Loyalty System

Welcome to the Ascenda Loyalty System, a comprehensive suite designed to empower loyalty programs with modern, scalable, and secure microservices architecture. This repository serves as the master repository, encapsulating all of our microservices and deployment sources to streamline the development and deployment processes.

## Components

The Ascenda Loyalty System comprises several key components, each serving a distinct role within the ecosystem:

- **`apidocs`**: Utilizes Redocly to provide comprehensive documentation for all available APIs, ensuring easy reference and integration for developers.

- **`database`**: Handles database migration and seeding, leveraging Prisma to ensure a smooth, efficient, and reliable database management process.

- **`frontend`**: A ReactJS-based frontend application that serves as the user interface, connecting seamlessly to our microservices to deliver a responsive and intuitive user experience.

- **`manifest`**: Contains Kubernetes deployment files, facilitating the orchestration and management of our microservices in a Kubernetes environment.

- **`mermaid`**: Supports the planning process with diagramming tools, enabling clear visualization of architecture and workflow.

- **`points-ledger`**: A backend service built with NestJS, dedicated to managing points-related services with Amazon QLDB for enhanced security and data integrity.

- **`protobuf`**: Hosts all our gRPC proto files, centralizing the definitions for inter-service communication to ensure consistency and reliability.

- **`proxy`**: A Golang application using the Gorilla Mux framework, this service is pivotal in handling authentication, authorization, caching, proxy, and logging functionalities.

- **`redaction`**: Focuses on PII anonymization for our logs. It consumes messages from a Kafka broker and anonymizes them using Presidio before indexing to Elasticsearch, thereby enhancing data privacy and compliance.

- **`terraform`**: Provides modules for infrastructure provisioning in AWS, enabling scalable and efficient management of cloud resources.

- **`users`**: Manages user details, roles, and permissions, serving as the cornerstone for access control and user management within the system.

## Getting Started

To get started with the Ascenda Loyalty System, please ensure you have the necessary prerequisites installed, including Docker, Kubernetes, and the respective CLI tools for interacting with AWS and Terraform.

### Setup and Deployment


To set up the Ascenda Loyalty System in your local development environment, follow these steps:

1. **Clone the Repository Recursively**:
   - This project uses Git submodules to manage its components. To clone the repository and its submodules in one step, use the following command:
     ```
     git clone --recurse-submodules git@github.com:cs301-itsa/project-2023-24t2-g1-t5.git
     ```
   - This command clones the main repository and initializes and updates each submodule contained within it.

2. **Navigate to Each Component Directory**:
   - After cloning, navigate into each component's directory to install dependencies or perform additional setup as described in the component-specific `README.md` files.

By following these updated steps, you ensure that not only the main repository but also all the associated submodules are correctly cloned and ready for use, simplifying the initial setup process for developers.
