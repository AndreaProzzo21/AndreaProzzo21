# 👋 Hi, I'm Andrea | Cloud-Native & Automation Engineer

<p align="left">
  <a href="https://www.linkedin.com/in/andrea-prozzo-02884826b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:and.prozzo@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

### 🎯 Overview

I am a Management Engineering graduate currently specializing in Digital Automation Engineering. My passion lies in building the "glue" between the physical world and the cloud. I design and develop systems that securely gather data from Edge and IoT devices, and manage it reliably within scalable, containerized cloud environments. My core focus is on building resilient infrastructures, full-stack observability, and process automation.

---

### ☸️ The Kubernetes & Cloud-Native Shift
I am currently evolving my stack toward the **Cloud-Native ecosystem**, focusing on:
* **Orchestration & Autoscaling:** Managing K8s resources (Deployments, StatefulSets, Services) and actively exploring Event-Driven Autoscaling with **KEDA**.
* **Observability:** Building full-stack telemetry and centralizing logs using **Prometheus**, **Loki**, and **Grafana** (PLG stack).
* **IaC & Configuration Management:** Automating infrastructure and application deployments using a pragmatic mix of **Terraform** and **Ansible**.
* **Security:** Implementing RBAC, Secret management, and secure API Gateways with **JWT & HttpOnly Cookies**.

---

### 🛠️ Tech Stack

| Domain | Tools & Technologies |
| :--- | :--- |
| **Cloud & Orchestration** | ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat-square&logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat-square&logo=amazon-aws&logoColor=white) ![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=flat-square&logo=terraform&logoColor=white) |
| **Backend & APIs** | ![Python](https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi) ![Flask](https://img.shields.io/badge/flask-%23000.svg?style=flat-square&logo=flask&logoColor=white) |
| **IoT & Edge** | ![MQTT](https://img.shields.io/badge/MQTT-3C5280?style=flat-square&logo=mqtt&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=flat-square&logo=Raspberry-Pi) ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white) |
| **Data & Monitoring** | ![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat-square&logo=InfluxDB&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/postgres-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white) ![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=flat-square&logo=grafana&logoColor=white) |
| **Automation** | ![n8n](https://img.shields.io/badge/n8n-FF6D5B?style=flat-square&logo=n8n&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=flat-square&logo=githubactions&logoColor=white) |

---

## 📌 Featured Projects

### 📡 [EdgeHub: Distributed Edge Control Plane](https://github.com/AndreaProzzo21/edge-hub)

*A centralized Command & Control platform for monitoring telemetry, hardware health, and containerized workloads across distributed edge nodes in industrial or agricultural settings.*

* **Full contained Go Agent:** Developed a cross-compiled, lightweight telemetry agent in Go leveraging gopsutil. It natively monitors host OS metrics (CPU, Thermal sensors, Swap, Disk I/O) and introspects container runtimes (Docker/K8s) in both bare-metal and cloud VMs.
* **Async FastAPI Backend:** Built a scalable backend with FastAPI and SQLAlchemy using stateless JWT authentication. Engineered a bidirectional C&C pipeline that enables seamless, remote JWT rotation (over-the-air) before token expiration, ensuring continuous and secure fleet connectivity with zero manual intervention at the edge.
* **Smart Alert Engine:** Engineered an intelligent background notification system for Discord/Slack. It features HTTP 429 Rate-Limit handling, custom payload evaluation, and stateful anti-spam cooldowns tracked securely via PostgreSQL JSON columns.

---

### ☸️ [K8s Cloud Gateway](https://github.com/AndreaProzzo21/k8s-cloud-gateway)

*A secure, self-hosted control plane for managing multi-cluster Kubernetes fleets with zero-trust RBAC and integrated Helm operations.*

* **Zero-Trust & Security:** Engineered a robust proxy architecture where Kubernetes credentials (`ca.crt`, Service Account tokens) never reach the client. Sensitive data is encrypted at rest in a SQLite database using **AES-128 (Fernet)**, with sessions secured by **HttpOnly JWTs**.
* **Advanced Helm Engine:** Built a universal package management system capable of processing native `.tgz` archives, custom `.zip` uploads, and remote repositories. Features real-time linting, subchart awareness, and one-click rollbacks via **FastAPI**.
* **Fleet Observation & Audit:** Designed a centralized Admin Console to monitor cluster health, node/pod telemetry, and compliance rules across the entire fleet in real-time.
* **Dynamic RBAC Scoping:** Implemented profile-based delegation that seamlessly maps team roles to specific K8s permissions. The UI intelligently adapts to the user's authorized scope, ensuring safe resource management without sharing `kubeconfig` files.
* **Enterprise Onboarding:** Developed an interactive, production-ready `curl-to-bash` bootstrap script for one-minute deployment via **Docker Compose**, featuring automated cryptographic key generation and smart defaults.

---

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

---

### 🌱 Currently Learning & Improving
*   **Advanced K8s Networking:** Deep diving into Service Meshes and advanced Ingress controllers.
*   **GitOps:** Implementing CI/CD pipelines for automated infrastructure deployments.
*   **SRE Principles:** Focus on scalability, reliability, and monitoring of distributed systems.
