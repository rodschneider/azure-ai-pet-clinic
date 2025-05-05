# 🐾 Azure AI PetClinic: AI-Powered Pet Care with Cloud-Native Design

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/rodschneider/azure-ai-pet-clinic) [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=7517918)

Welcome to **Azure AI PetClinic**, an enhanced version of the Spring PetClinic app. This project transforms the traditional pet management system into a cloud-native, AI-driven application that provides health insights, automated notifications, and scalable deployment on Azure Kubernetes Service (AKS). My goal is to make this a valuable resource for developers learning cloud-native development, DevOps, and AI integration.

## 🎯 Objective
The goal is to modernize the Spring PetClinic app as both a functional system and a teaching tool. Key features include:
- **AI-driven health insights** to identify pet health trends.
- **Event-driven notifications** for appointment updates.
- **Cloud-native deployment** on AKS with a CI/CD pipeline.
- A demo-ready app suitable for hackathons, tutorials, or portfolio projects.

Detailed guides are available on [dev.to/rod_schneider](https://dev.to/rod_schneider/) and [rodschneider.com](https://www.rodschneider.com/), covering steps like AKS setup and Azure AI integration.

## 🐕 Why It Matters

- **Real-World Utility**: Enables pet clinics to predict health issues (e.g., recurring allergies) and automate appointment reminders, improving care and efficiency.
- **Educational Value**: Covers a broad tech stack—Spring Boot, React, Kubernetes, Azure, AI — making it a strong learning tool and portfolio piece.
- **Scalable Design**: Kubernetes and Azure services support real clinic workloads, with a CI/CD pipeline demonstrating DevOps best practices.
- **Demo Appeal**: AI insights and notifications make it engaging for hackathons or tech talks.

## 🩺 Key Features

### 🐾 Core PetClinic Functionality
- Manage owners, pets, visits, and veterinarians via a **REST API** (Spring Boot, Spring Data JPA) and **React frontend**.
- Store persistent data in **Azure Database for MySQL**, replacing the default H2 database.

### 🧠 AI-Driven Health Insights
- Use **Azure AI Text Analytics** to analyze visit notes, assessing symptom severity and identifying recurring issues (e.g., “lethargy”).
- Apply **Azure OpenAI Service** embeddings to cluster similar visit descriptions, detecting patterns like seasonal allergies.
- Display insights in a **React dashboard** with “Top Health Trends” or “Potential Chronic Issues.”

### 📬 Event-Driven Notifications
- Publish appointment updates (e.g., “Fluffy’s checkup on May 10, 2025”) using **Azure Event Hubs**.
- A **Spring Boot consumer** processes events and sends emails via **Azure Communication Services** or in-app alerts on the React frontend.

### ☁️ Cloud-Native Deployment
- Containerize the Spring Boot backend and React frontend with **Docker**.
- Deploy to **Azure Kubernetes Service (AKS)** with separate pods for backend, frontend, and event consumers.
- Store relational data in **Azure Database for MySQL** and AI insights in **Azure Cosmos DB** for efficient querying.

### 🚀 CI/CD Pipeline
- A **GitHub Actions** pipeline builds, tests, and deploys Docker images to AKS.
- Includes automated tests for the REST API (**Spring Boot Test**) and frontend (**Jest/React Testing Library**).

### 📈 Monitoring & Scalability
- Monitor performance with **Azure Monitor** and **Application Insights** (e.g., API response times, AKS cluster health).
- Enable **Horizontal Pod Autoscaling (HPA)** in AKS to handle traffic spikes.

## 📚 Teaching Value
This project teaches:
- **Backend Development**: Building REST APIs, using Spring Data JPA, and implementing event-driven architecture with Spring Boot.
- **Frontend Development**: Creating a React dashboard for AI insights and notifications.
- **Cloud-Native Practices**: Containerization (Docker), orchestration (Kubernetes), and Azure service integration.
- **DevOps**: Setting up CI/CD with GitHub Actions and monitoring with Azure tools.
- **AI Integration**: Using Azure AI and OpenAI for data-driven insights.
- **Real-World Application**: Applying these technologies to pet health management.

## 📝 Follow Along
Explore the details in this README and find step-by-step guides on:
- [dev.to/rod_schneider](https://dev.to/rod_schneider/) for posts like “Setting up AKS” or “Integrating Azure AI.”
- [rodschneider.com](https://www.rodschneider.com/) for additional insights and tutorials.

Ready to build a smarter pet clinic? Clone this repo, open your IDE, and start exploring! 🐕

## Interesting Spring Petclinic branches and forks

The Spring Petclinic "main" branch in the [spring-projects](https://github.com/spring-projects/spring-petclinic)
GitHub org is the "canonical" implementation based on Spring Boot and Thymeleaf. There are
[quite a few forks](https://spring-petclinic.github.io/docs/forks.html) in the GitHub org
[spring-petclinic](https://github.com/spring-petclinic). If you are interested in using a different technology stack to implement the Pet Clinic, please join the community there.

## Contributing

The [issue tracker](https://github.com/rodschneider/azure-ai-pet-clinic/issues) is the preferred channel for bug reports, feature requests and submitting pull requests.

For pull requests, editor preferences are available in the [editor config](.editorconfig) for easy use in common text editors. Read more and download plugins at <https://editorconfig.org>. All commits must include a __Signed-off-by__ trailer at the end of each commit message to indicate that the contributor agrees to the Developer Certificate of Origin.
For additional details, please refer to the blog post [Hello DCO, Goodbye CLA: Simplifying Contributions to Spring](https://spring.io/blog/2025/01/06/hello-dco-goodbye-cla-simplifying-contributions-to-spring).

## License

The Azure AI PetClinic is released under version 2.0 of the [Apache License](https://www.apache.org/licenses/LICENSE-2.0).
