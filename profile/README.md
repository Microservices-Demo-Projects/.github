# Microservices-Demo-Projects with Kubernetes and SpringBoot / SpringCloud

This organization explores the various **microservice architectures** and **cross-cutting concerns** by creating proof of concept or prototype/demo applications. In all the demo projects developed here the primary platform to deploy all the microservices will be **Kubernetes** and the primary framework that is used for creating the microservices will be **SpringBoot / SpringCloud**.

## Table of Contents

### 1. **[Configuration Management and Updates](https://github.com/Microservices-Demo-Projects/Configuration-Management-And-Updates  "readme")** 
- **Demo-1**: External Property Management and Dynamic Refresh with Kubernetes Config Map :heavy_check_mark:
- **Demo-2**: Secrets Management with Dynamic Secret Generation and Dynamic Secrets Refresh with Hashicorp Vault.

### 2. **[Logging and Distributed Tracing](https://github.com/Microservices-Demo-Projects/logging-and-distributed-tracing)** :heavy_check_mark:

### 3. **[Monitoring Application Metrics](https://github.com/Microservices-Demo-Projects/microservices-metrics-and-monitoring)**
   
### 4. **Securing Microservice APIs**
**This can be split into two categories:**
4.1. **Cross-cutting concerns that are better handled with generic tools/solutions without modifying the application code such as:**
    - **Network Policies (AllowList and DenyList)**
    - **mTLS**
    - **OAuth(Client Credentials Flow and Authorization Code Flow - PKCE)**
    - **Rate Limiting**
4.2. **The domain-specific solutions that require the application code changes such as:**
   - **Resilience (Circuit Breaking)**

### 5. **Databases and Caching (I/O)**

### 6. **Event Driven Services - Messaging Queues**
   
### 7. **Leader Election with Kubernetes**

### 8. **Types of APIs**
- **Web Sockets**
- **Server-Sent Events**
- **Reactive Streams (Non blocking & No back pressure)**
- **gRPC (Protocol Buffers)**
- **GraphQL**
