# System Design Learning Roadmap (For 2+ Years Experience)

This roadmap is designed for software engineers with 2+ years of experience who want to understand and articulate system design concepts effectively. It assumes basic hands-on knowledge of software engineering but no formal training in system design.

---

## ✅ Phase 1: Foundations (Core Concepts)

### 1. What is System Design?

* Difference between High-Level Design (HLD) and Low-Level Design (LLD)
* Functional vs Non-functional requirements
* Importance of scalability, reliability, maintainability, and availability

### 2. Scalability Basics

* Horizontal vs vertical scaling
* Elasticity
* Stateless vs stateful services

### 3. Performance Metrics

* Latency
* Throughput
* Availability (SLA, SLO, SLI)
* Error budgets

### 4. Monolith vs Microservices

* Pros and cons
* When to split services
* Communication patterns (REST, gRPC, async messaging)

### 5. CAP Theorem

* Consistency, Availability, Partition Tolerance
* Real-world implications and trade-offs

---

## 📈 Phase 2: Key Building Blocks

### 6. Client-Server & Network Fundamentals

* HTTP/HTTPS
* WebSockets vs polling vs long-polling
* DNS resolution

### 7. Load Balancing

* Round-robin, least connections, IP hash
* Layer 4 vs Layer 7 load balancers
* Global load balancing (GeoDNS)

### 8. Caching Strategies

* CDN, browser cache, application cache (Redis, Memcached)
* Cache eviction: LRU, LFU, FIFO
* Cache invalidation strategies

### 9. Databases

* SQL vs NoSQL
* ACID vs BASE
* Sharding, replication, partitioning
* Indexing, query optimization

### 10. Asynchronous Processing

* Message Queues: Kafka, RabbitMQ, SQS
* Pub/Sub patterns
* Event-driven architecture

### 11. Storage Systems

* Block vs File vs Object storage
* Systems: Amazon S3, Google Cloud Storage, HDFS
* Data durability and availability

### 12. Authentication & Authorization

* OAuth2, OpenID Connect
* JWT, sessions, API keys
* Role-based access control (RBAC), attribute-based access control (ABAC)

### 13. Rate Limiting & Throttling

* Token bucket, leaky bucket algorithms
* Global vs per-user rate limits

### 14. Observability

* Logging, metrics, tracing
* Tools: Prometheus, Grafana, ELK stack, Jaeger

---

## 📅 Phase 3: Real-World System Design Case Studies

Start with small systems and progress to more complex designs.

### 15. URL Shortener (e.g., bit.ly)

* Hashing, database choice
* Redirection flow
* Analytics (click tracking)

### 16. Rate Limiter Service

* Sliding window algorithm
* In-memory and distributed designs

### 17. News Feed (e.g., Facebook, LinkedIn)

* Fan-out on write vs read
* Feed ranking and caching

### 18. File Storage System (e.g., Google Drive)

* Chunking, metadata service
* Sharing and access control
* Syncing clients

### 19. Chat Application (e.g., WhatsApp)

* Message queues, delivery guarantees
* Presence tracking, read receipts

### 20. Ride-Sharing Platform (e.g., Uber)

* Location tracking, ETA calculation
* Matching algorithms
* Surge pricing and dispatch system

### 21. E-Commerce Platform (e.g., Amazon)

* Inventory, order processing
* Payment and fraud detection
* Search and recommendations

### 22. Video Streaming Platform (e.g., YouTube)

* Chunked video delivery (DASH, HLS)
* CDN, transcoding, live streaming

---

## 🧰 Phase 4: Advanced Topics

### 23. Distributed Systems Internals

* Leader election, consensus (Paxos, Raft)
* Vector clocks, gossip protocol
* Quorum-based systems

### 24. System Design Patterns

* Circuit breaker, bulkhead
* Saga pattern, event sourcing
* CQRS (Command Query Responsibility Segregation)

### 25. Containerization & Orchestration

* Docker fundamentals
* Kubernetes: pods, services, deployments
* Auto-scaling, health checks

### 26. Multi-region and Global Architectures

* Active-active vs active-passive
* Data replication strategies
* Latency and consistency trade-offs

---

## 📘 Bonus: Tips for Learning and Sharing

* **Create diagrams** using Excalidraw, Lucidchart, or draw\.io
* **Write blog posts** or LinkedIn articles for each topic
* **Present internally** at your company to strengthen recall
* **Engage with the community** via Reddit, Twitter, GitHub

---

Happy designing! 🚀
