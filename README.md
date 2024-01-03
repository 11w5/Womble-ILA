# Womble-ILA
Internal Logistic Application made to streamline the internal processes of the application.

---

## Description

This project is a comprehensive solution for managing trucking logistics operations tailored for a mid-sized transportation company. It facilitates real-time vehicle tracking, dispatch and load assignment, customer and order management, document handling, and includes an administration dashboard as well as API for integration. Our goal is to support 1000+ inbound/outbound orders per day and accommodate 5000+ concurrent users with real-time functionality.

## Key Features

- Customer and Order Management
- Dispatch and Load Assignment
- Real-Time Vehicle Tracking
- Document Handling: Bills of Lading (BOLs), Proof of Deliveries (PODs), Invoices
- Administration Dashboard
- API for integration with third-parties
- Web and Mobile User Interface

## Architecture Overview

The system is built using a microservices architecture to ensure scalability and maintainability. Each microservice runs in its own container, allowing for independent scaling and deployment. Real-time tracking and dispatch features require robust and responsive backend services.

### Microservices:

- `auth-service`: Handles user authentication and authorization.
- `user-service`: Manages user accounts and role permissions.
- `customer-service`: Manages customer profiles and order histories.
- `order-service`: Processes and tracks orders.
- `dispatch-service`: Assigns loads and manages dispatch operations.
- `tracking-service`: Provides real-time GPS tracking of the truck fleet.
- `document-service`: Manages transport documents such as BOLs, PODs, and invoices.
- `admin-dashboard`: Offers a comprehensive overview of logistics operations for administrators.
- `api-gateway`: Facilitates communication between the front-end and various microservices.

### Frontend:

- Web Application: Built with React for interacting with the back-end services.
- Mobile Application: Built with React Native for use on both iOS and Android devices.

### Infrastructure:

- Docker and Kubernetes for containerization and orchestration.
- Hosted on AWS/GCP with automated deployment pipelines.
- PostgreSQL database for persistent data storage.

## Technology Stack

- **Backend API**: Node.js, Express
- **Database**: PostgreSQL
- **Web App**: React
- **Mobile Apps**: React Native
- **Hosting and Orchestration**: Docker, Kubernetes, AWS/GCP
- **Monitoring**: Prometheus, Grafana, ELK Stack

## Getting Started

Below are the instructions to set up your development environment and get the application running.

### Prerequisites

- Node.js (v14 or later)
- Docker
- Kubernetes (Minikube for local development)
- PostgreSQL (local or a managed cloud instance)
- Git

### Installation

1. Clone the repository.
   ```sh
   git clone https://github.com/<organization>/trucking-logistics-app.git
   cd trucking-logistics-app
   ```
2. Initialize and pull the submodules for each service.
   ```sh
   git submodule init
   git submodule update
   ```
3. Follow the individual READMEs in each service for further instructions.

### Running Locally

_To be completed by each microservice's documentation._

### Testing

_Run the automated test suite with the following command (to be customized per service):_

```sh
npm test
```

## Deployment

Working on this.

## Monitoring and Logging

Working on this.

## Acknowledgments

Working on this.


