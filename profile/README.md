# Microservices-Demo-Projects with Kubernetes and SpringBoot / SpringCloud

This organization explores the various **microservice architectures** and **cross-cutting concerns** by creating proof of concept or prototype/demo applications. In all the demo projects developed here the primary platform to deploy all the microservices will be **Kubernetes** and the primary framework that is used for creating the microservices will be **SpringBoot / SpringCloud**.

## Table of Contents

### 1. [Configuration Management and Updates](https://github.com/Microservices-Demo-Projects/configuration-management-and-updates "open readme.md")
- **Externalized Configuration**: Using Kubernetes ConfigMaps and Secrets with environment variables, property files, etc. for storage and retrieval of environment specific configs.
- **Securing Secrets**: Using _HashiCorp Vault_ or _SealedSecrets_ for securely storing secrets in encrypted formats.
- **Dynamic Secret Management**: Auto-generation and rotation of short-lived credentials during application startup.
- **Dynamic Configuration Reloading**: Updating/refreshing application configurations without downtime.

### 2. [Logging and Distributed Tracing](https://github.com/Microservices-Demo-Projects/logging-and-distributed-tracing "open readme.md") 
- **Log traceIds and spanIds**: Automatically adding common traceIds in the application logs to monitor the chain of API calls made among the microservice applicatoins.
- **Structured Logging**: Logging with JSON format for better observability.
- **Centralized Log Aggregation**: Collecting and retaining logs from the applications in a single datastore for debugging.
- **Log Visualization and Monitoring**: Setting up dashboards using tools like Loki, or Kibana.
- **Log-Based Alerting**: Configuring alerts based on log patterns (e.g., using Prometheus Alertmanager or ELK Stack).

### 3. [Microservices Metrics and Monitoring](https://github.com/Microservices-Demo-Projects/microservices-metrics-and-monitoring "open readme.md")
- **Application Metrics Collection**: Using Micrometer, Prometheus, or OpenTelemetry for collecting application-level metrics.
- **Visualization and Dashboards**: Grafana and Prometheus for monitoring CPU, memory, and request latency.
- **Anomaly Detection & Alerts**: Alerting based on metric thresholds (e.g., using Alertmanager).
- **Auto-Scaling Based on Metrics**: HPA (Horizontal Pod Autoscaler) and KEDA (Kubernetes Event-Driven Autoscaler).

### 4. Security
- **mTLS Configuration with Auto Certificate Rotation**: Using Istio or Linkerd for mutual TLS with auto-renewing certificates.
- **OAuth2 & OIDC Authentication**: Client Credentials Flow, Authorization Code Flow - PKCE, JWT validation using an auth server like Keycloak, Okta, Auth0, etc.
- **Rate Limiting**: Using API Gateway for throttling requests.
- **Network Policies**: Defining Kubernetes Network Policies for isolating traffic.
- **RBAC & Service Accounts**: Kubernetes Role-Based Access Control (RBAC) for service authorization.

### 5. Fault Tolerance and Resilience
- **Circuit Breaking & Retry Mechanisms**: Implementing Resilience4J, or with Istio.
- **Graceful Shutdown & Readiness/Liveness Probes**: Ensuring zero-downtime deployments.
- **Bulkhead and Fallback Strategies**: Preventing cascading failures.
- **Chaos Engineering**: Testing failures using Chaos Mesh or LitmusChaos.

### 6. Database and Caching
- **Database Connection Pooling**: Using HikariCP for managing database connections efficiently.
- **Database Scaling & Sharding**: Horizontal partitioning strategies and Kubernetes StatefulSets.
- **Caching Strategies**: Implementing caching solution with Redis for reducing database load.
- **Transactional Event-Driven Architecture**: SAGA, Outbox Pattern, Change Data Capture (CDC), etc.

### 7. Event-Driven Systems
- **Message Brokers**: Using Kafka, or RabbitMQ for event-driven communication.
- **Event Sourcing and CQRS**: Implementing event-driven persistence models.
- **Dead Letter Queues (DLQ) & Retry Mechanisms**: Handling failed messages effectively.

### 8. Batch Processing Systems
- **Spring Batch for Large-Scale Data Processing**
- **Kubernetes CronJobs for Scheduled Jobs**
- **Parallel Processing & Chunk-Based Processing**
- **Retry and Failure Handling in Batch Jobs**

### 9. Stream Processing Systems
- **Kafka Streams, Flink, or Spark Streaming**
- **Processing Real-Time Data with Stateful Applications**
- **Windowing Strategies & Aggregation Techniques**
- **Handling Late Arriving Data & Event-Time Processing**

### 10. Leader Election with Kubernetes
- **Implementing Leader Election using Kubernetes Lease API**
- **Ensuring High Availability of Stateful Applications**
   - Use Cases: Distributed Locks & Singleton Processing in Microservices

### 11. API Development
- **REST API Best Practices**: Designing scalable RESTful services.
- **gRPC Communication**: Implementing high-performance binary-based APIs.
- **GraphQL APIs**: Querying flexible data models with Apollo or Spring GraphQL.
- **Server-Sent Events (SSE) & WebSockets**: Real-time bidirectional communication.
- **API Gateway Implementation**: Istio Ingress Gateway or Kubernetes Gateway API.


   
### 7. **Leader Election with Kubernetes**

### 8. **Types of APIs**
- **Web Sockets**
- **Server-Sent Events**
- **Reactive Streams (Non blocking & No back pressure)**
- **gRPC (Protocol Buffers)**
- **GraphQL**
