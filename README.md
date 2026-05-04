# 👋 Hi, I'm Andrea Prozzo | Cloud-Native & Automation Engineer

<p align="left">
  <a href="https://www.linkedin.com/in/andrea-prozzo-02884826b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:and.prozzo@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

### 🎯 Overview
I am a **Digital Automation Engineering** student specializing in the convergence of **Industrial IoT**, **Distributed Systems**, and **Cloud-Native Infrastructure**. I build bridge solutions that connect the physical world (Edge) to highly scalable and orchestrated environments (Cloud).

---

### ☸️ The Kubernetes & Cloud-Native Shift
I am currently evolving my stack toward the **Cloud-Native ecosystem**, focusing on:
*   **Orchestration:** Deploying and managing K8s resources (Deployments, StatefulSets, Services, Ingress).
*   **Security:** Implementing RBAC, Secret management, and secure API Gateways with **JWT & HttpOnly Cookies**.
*   **Automation (IaC):** Provisioning multi-cluster environments on **AWS** using **Terraform**.
*   **Observability:** Building full-stack monitoring pipelines with **Grafana**, **InfluxDB**, and custom exporters.

---

### 🛠️ Tech Stack

| Domain | Tools & Technologies |
| :--- | :--- |
| **Cloud & Orchestration** | ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat-square&logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat-square&logo=amazon-aws&logoColor=white) ![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=flat-square&logo=terraform&logoColor=white) |
| **Backend & APIs** | ![Python](https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white) |
| **IoT & Edge** | ![MQTT](https://img.shields.io/badge/MQTT-3C5280?style=flat-square&logo=mqtt&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=flat-square&logo=Raspberry-Pi) ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white) |
| **Data & Monitoring** | ![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat-square&logo=InfluxDB&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/postgres-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white) ![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=flat-square&logo=grafana&logoColor=white) |
| **Automation** | ![n8n](https://img.shields.io/badge/n8n-FF6D5B?style=flat-square&logo=n8n&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=flat-square&logo=githubactions&logoColor=white) |

---

## 📌 Featured Projects

### ☸️ [K8s Cloud Gateway](https://github.com/AndreaProzzo21/k8s-cloud-gateway)
*A stateless, multi-cluster management platform designed for granular, profile-based access to Kubernetes resources.*
- **Zero-Trust Architecture:** Implemented a stateless authentication system using **JWT** to encapsulate encrypted K8s Service Account tokens, ensuring credentials never reside on the client-side.
- **Dynamic Orchestration:** Built with **FastAPI** and the **Kubernetes Python Client** to manage Pods, scale Deployments, and perform rollout restarts across multiple clusters through a unified API.
- **Stateless Security:** Integrated **HttpOnly Cookies** and RBAC mapping to bridge the gap between simple web interfaces and complex K8s permission structures.
- **Infrastructure:** Fully containerized with **Docker Compose**, featuring an Nginx-backed frontend and a secure Python backend.

### 🏭 [Cloud-Native Predictive Maintenance Pipeline](https://github.com/AndreaProzzo21/Edge-Cloud-PdM-Pipeline)
*An E2E MLOps pipeline for industrial assets, transitioning from physical simulation to a fully containerized Digital Twin environment.*
- **Digital Twin Engine:** Developed high-fidelity Python simulators modeling **ISO 10816** vibration standards and non-linear degradation curves with a built-in **Chaos Engine** for stress testing.
- **Distributed Microservices:** Engineered a decoupled architecture using **MQTT (Mosquitto)**, **FastAPI**, and **InfluxDB 2.x** for real-time telemetry processing (100+ concurrent assets).
- **MLOps Workflow:** Designed an offline-to-online pipeline where **Random Forest** models are trained on historical InfluxDB data and hot-loaded into AWS-hosted inference services for real-time diagnostics.
- **IaC & DevOps:** Automated the entire AWS (EC2) ecosystem provisioning using **Terraform**.

### ☁️ [AWS IoT Industrial Hub](https://github.com/AndreaProzzo21/AWS-IoTCore-Industrial-Hub)
*A multi-site industrial data platform leveraging AWS IoT Core for secure, event-driven telemetry ingestion.*
- **Event-Driven Processing:** Implemented an **AWS Lambda Multiplexer** to intercept MQTT streams, evaluate dynamic thresholds, and trigger automated **SNS** alerts.
- **Industrial Security:** Enforced **X.509 certificate authentication** and mTLS encryption for every simulated device, ensuring strict topic isolation and identity management via Terraform.
- **Full-Stack Monitoring:** Orchestrated a Dockerized analytics stack on EC2 featuring **InfluxDB** for time-series persistence and **Grafana** for real-time factory dashboards.

### 🌐 [Modular IoT End-to-End Platform](https://github.com/AndreaProzzo21/End-to-End-IoT-Platform)
*A full-stack ecosystem bridging ESP32 edge devices with a modular Python monolith and AI-powered interfaces.*
- **Edge Layer:** Wrote robust **C++ firmware** for ESP32 with JSON-based protocols for bidirectional telemetry and remote actuator control (Servos/Fans).
- **Conversational UI:** Developed a **Telegram Bot** integrated with **n8n** and private Webhooks, allowing remote system orchestration and LLM-powered status queries.
- **Modular Monolith:** Built a scalable backend with FastAPI and Pydantic, featuring role-based **Bearer Token** security and InfluxDB integration.

---

### 🤖 AI & Automation Showreel (n8n & LLMs)
Beyond structured projects, I maintain a continuous laboratory of **autonomous workflows** using **n8n**:
- **AI Orchestration:** Integrating LLMs (OpenAI/Anthropic) with **STT (Speech-to-Text)** and **TTS (Text-to-Speech)** for voice-controlled automation.
- **API Mashups:** Custom integrations between Telegram, Google Services, and third-party SaaS to automate data processing and alerting.
- **Smart Agents:** Building event-driven agents that monitor web sources and generate AI-summarized insights directly to private channels.

### 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=AndreaProzzo21&show_icons=true&theme=react&rank_icon=github&border_radius=10&hide_border=true" alt="Andrea's Stats" height="192px" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AndreaProzzo21&layout=compact&theme=react&border_radius=10&hide_border=true" alt="Top Languages" height="192px" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=AndreaProzzo21&theme=react-dark&hide_border=true&area=true" alt="Andrea's Activity Graph" width="100%" />
</p>

---

### 🌱 Currently Learning & Improving
*   **Advanced K8s Networking:** Deep diving into Service Meshes and advanced Ingress controllers.
*   **GitOps:** Implementing CI/CD pipelines for automated infrastructure deployments.
*   **SRE Principles:** Focus on scalability, reliability, and monitoring of distributed systems.

---
<p align="center">
  <i>"I build resilient infrastructures for an automated future."</i>
</p>
