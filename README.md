# Best Buy – Store Admin

This is the employee-facing administration web application for the **Best Buy Cloud-Native Final Project**.

The Store Admin application is used by Best Buy staff to manage store operations, including
monitoring orders and interacting with backend services.

It is part of a microservices-based architecture deployed on **Azure Kubernetes Service (AKS)**.

This project is adapted from the **Algonquin Pet Store (On Steroids)** reference architecture
and has been rebranded and extended for the Best Buy cloud-native final project in CST8915.

---

## Architecture Context

The Store Admin service communicates with backend services such as:
- **Order Service** – to view and manage customer orders
- **Makeline Service** – to track order processing
- **RabbitMQ** – for asynchronous messaging

All services are containerized and orchestrated using Kubernetes.

---

## Running the App Locally (Optional)

> ⚠️ Local execution is for development and testing only.  
> In production, this service runs inside Kubernetes (AKS).

### Prerequisites
- Node.js  
- Docker  
- Docker Compose  

### Local Development

The Store Admin application can be run locally using Docker Compose
alongside the required backend services.

```bash
docker compose up
``