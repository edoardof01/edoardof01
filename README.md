# Edoardo Fanciullacci

**Software Engineer** with an unconventional path: from Management Engineering to Computer Engineering, both with **110/110 with Honours** — a background that blends systems thinking with technical rigour.

I specialise in **distributed systems**, **cloud-native infrastructures**, and **applied AI**. I'm not just interested in making things work: I want to understand *why* they work, build with formal rigour, and leave behind code that stands the test of time.

> 📍 Florence, Italy · Open to remote and hybrid opportunities

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Edoardo_Fanciullacci-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/edoardo-fanciullacci)
[![Email](https://img.shields.io/badge/Email-edoardofanciullacci01@gmail.com-D14836?style=flat&logo=gmail)](mailto:edoardofanciullacci01@gmail.com)

---

## 🎓 Education

| Degree | University | Grade |
|---|---|---|
| **Master's Degree** — Computer Engineering | University of Florence | 110/110 with Honours |
| **Bachelor's Degree** — Management Engineering | University of Florence | 110/110 with Honours |

---

## 🚀 Featured Projects

### 📐 [Master's Thesis] Evaluation and Refactoring of SAGA Topologies
> *Framework for stochastic consistency analysis in microservices architectures*

Microservices architectures promise scalability, but hide a subtle problem: **how do you guarantee eventual consistency when a distributed transaction partially fails?**

I built a theoretical and empirical framework to analyse and optimise **Time to Consistency** in SAGA patterns with parallel (AND) and conditional (XOR) branches.

**Key contribution:** a Greedy refactoring algorithm based on **stochastic dominance of CDFs**, which minimises recovery times by choosing the optimal execution order for compensating transactions.

```
Stack: Java (Sirio/Eulero) · Kubernetes · Apache Kafka
Results: +15.29% performance · MAE < 0.02 (empirical validation)
```

---

### 🌐 [Platform Project](https://github.com/edoardof01/Platform_Project) — Cloud-Native Microservices Platform
> *Production-grade microservices architecture with GitOps, observability, and Infrastructure as Code*

An end-to-end platform that goes beyond business logic: it covers the full lifecycle of a cloud-native system — from application code, to orchestration, monitoring, and infrastructure provisioning.

Three Spring Boot microservices (API Gateway, Product Service, Order Service) orchestrated on **Kubernetes** with declarative deployments and automatic reconciliation via **ArgoCD** (Self-Heal + Prune). Secret management is handled with **Bitnami Sealed Secrets** — asymmetric encryption that allows secrets to be versioned in Git without exposing credentials.

- 🔄 **GitOps-first:** every commit to `k8s/` is automatically synced to the cluster by ArgoCD
- 🛡️ **Resilience:** Circuit Breaker and Time Limiter (Resilience4j) on the API Gateway to prevent cascading failures
- 📊 **Observability:** Prometheus Operator with ServiceMonitor + Grafana for custom metrics (Micrometer/Actuator)
- 🔐 **Secrets management:** Sealed Secrets with `kubeseal` — safely versionable encrypted secrets
- 🏗️ **IaC:** Terraform for VM provisioning on ARM64 on OCI (Oracle Cloud Always Free Tier)
- ⚙️ **CI/CD:** GitHub Actions with build matrix, Maven caching, and automatic push to Docker Hub

```
Stack: Java 21 · Spring Boot 4 · Spring Cloud Gateway · PostgreSQL · Flyway
Infrastructure: Kubernetes (Minikube) · ArgoCD · Prometheus · Grafana · Docker · Terraform (OCI)
Security: Bitnami Sealed Secrets · RBAC · Liveness/Readiness Probes
```

---

### 🤖 [cf_ai_rag](https://github.com/edoardof01/cf_ai_rag) — Advanced Hybrid RAG System
> *Production-grade RAG system, fully self-hosted on Kubernetes*

A Retrieval-Augmented Generation system that goes beyond simple vector search. The hybrid design combines **two retrieval paradigms** to maximise response quality:

- 🔍 **Dense retrieval** (semantic) via **Milvus**
- 📖 **Sparse retrieval** (lexical) via **BM25 on Redis**
- 🎯 **Cross-Encoder reranking** for final selection
- 🧠 **Multi-strategy conversational memory**: Sliding Window · Summary · Vector Memory
- ✍️ **Contextual Query Rewriting** + dynamic token budget management

```
Infrastructure: Minikube · Ollama (Qwen 2.5) · Milvus · Redis
Deployment: fully automated with data persistence
```

---

## 🛠 Other Projects

### [SessionBuilder](https://github.com/edoardof01/sessionBuilder) — Java Desktop App with Strict TDD
Application developed with end-to-end engineering discipline: every line of code covered by tests before being written.

- Complete **CI/CD pipeline** with GitHub Actions
- **Static analysis** with SonarCloud + **Mutation Testing** with PIT
- **MVC + Service Layer architecture** with custom transactional management via `ThreadLocal`

### [Multi-Label Emotion Classifier](https://github.com/edoardof01/fml-laboratory) — NLP with DistilBERT
Multi-label emotion classifier that tackles the often-overlooked problem of **label noise**.

- **Confident Learning** (CleanLab) for automatic cleaning of noisy annotations
- **Optuna** for Bayesian hyperparameter optimisation
- **LIME** for prediction explainability (XAI)

---

## 🧰 Tech Stack

| Area | Technologies |
|---|---|
| **Languages** | Java (Spring, JPA/Hibernate), Python (PyTorch, LangChain, Pandas), SQL (Postgres), C |
| **Cloud & DevOps** | Docker, Kubernetes, Apache Kafka, GitHub Actions, Maven, ArgoCD, Terraform |
| **AI & Data** | Vector DBs (Milvus), Redis, RAG Architectures, LLM Self-hosting (Ollama), NLP, XAI |
| **Observability** | Prometheus, Grafana, Micrometer, Spring Boot Actuator |
| **Software Engineering** | TDD, Design Patterns, Microservices, DDD, GitOps |

---

## 📚 Continuous Learning

Building systems isn't enough: you need to understand the *why* behind every choice. That's why I study systematically and continuously — textbooks, papers, technical blogs, original documentation. Some areas I'm currently exploring:

- **Distributed Systems** — *Designing Data-Intensive Applications* (Kleppmann), papers on consensus algorithms
- **AI/ML** — papers on advanced RAG architectures, agentic systems, model evaluation
- **Software Design** — *A Philosophy of Software Design* (Ousterhout), architectural patterns

I believe software engineering is a craft that demands constant intellectual humility: the landscape shifts, and keeping up means never stopping being a student.

---

*I find that the intersection of formal rigour and creative engineering is the most stimulating place to build software — and the Management → Computer Engineering trajectory has given me the tools to inhabit both sides.*
