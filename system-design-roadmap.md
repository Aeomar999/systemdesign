# System Design Roadmap

The line diagram below is designed to display directly in Notion without Mermaid. Its `☐` symbols are visual; use the interactive task list below it to track your progress.

## Visual map

```text
☐ SYSTEM DESIGN
│
├── ☐ Introduction
│   ├── ☐ What is System Design?
│   └── ☐ How to approach System Design?
│
├── ☐ Performance and Scalability
│   ├── ☐ Performance vs Scalability
│   └── ☐ Latency vs Throughput
│
├── ☐ Availability and Consistency
│   ├── ☐ CAP Theorem
│   │   ├── ☐ AP - Availability + Partition Tolerance
│   │   └── ☐ CP - Consistency + Partition Tolerance
│   └── ☐ Consistency Patterns
│       ├── ☐ Weak Consistency
│       ├── ☐ Eventual Consistency
│       └── ☐ Strong Consistency
│
├── ☐ Availability Patterns
│   ├── ☐ Fail-Over
│   │   ├── ☐ Active-Active
│   │   └── ☐ Active-Passive
│   ├── ☐ Replication
│   │   ├── ☐ Master-Slave
│   │   └── ☐ Master-Master
│   └── ☐ Availability in Numbers
│       ├── ☐ 99.9% Availability - three 9s
│       ├── ☐ 99.99% Availability - four 9s
│       └── ☐ Availability in Parallel vs Sequence
│
├── ☐ Background Jobs
│   ├── ☐ Event-Driven
│   ├── ☐ Schedule Driven
│   └── ☐ Returning Results
│
├── ☐ Networking and Application Architecture
│   ├── ☐ Domain Name System
│   │   └── ☐ Content Delivery Networks
│   │       ├── ☐ Pull CDNs
│   │       └── ☐ Push CDNs
│   ├── ☐ Load Balancers
│   │   ├── ☐ LB vs Reverse Proxy
│   │   ├── ☐ Load Balancing Algorithms
│   │   ├── ☐ Layer 7 Load Balancing
│   │   ├── ☐ Layer 4 Load Balancing
│   │   └── ☐ Horizontal Scaling
│   └── ☐ Application Layer
│       ├── ☐ Microservices
│       └── ☐ Service Discovery
│
├── ☐ Databases
│   ├── ☐ SQL vs NoSQL
│   ├── ☐ RDBMS
│   │   ├── ☐ Replication
│   │   ├── ☐ Sharding
│   │   ├── ☐ Federation
│   │   ├── ☐ Denormalization
│   │   └── ☐ SQL Tuning
│   └── ☐ NoSQL
│       ├── ☐ Key-Value Store
│       ├── ☐ Document Store
│       ├── ☐ Wide Column Store
│       └── ☐ Graph Databases
│
├── ☐ Caching and Asynchronism
│   ├── ☐ Caching Strategies
│   │   ├── ☐ Refresh Ahead
│   │   ├── ☐ Write-behind
│   │   ├── ☐ Write-through
│   │   └── ☐ Cache Aside
│   ├── ☐ Types of Caching
│   │   ├── ☐ Client Caching
│   │   ├── ☐ CDN Caching
│   │   ├── ☐ Web Server Caching
│   │   ├── ☐ Database Caching
│   │   └── ☐ Application Caching
│   └── ☐ Asynchronism
│       ├── ☐ Back Pressure
│       ├── ☐ Task Queues
│       └── ☐ Message Queues
│
├── ☐ Operations
│   ├── ☐ Idempotent Operations
│   ├── ☐ Communication
│   │   ├── ☐ HTTP / TCP / UDP
│   │   └── ☐ RPC / gRPC / REST / GraphQL
│   ├── ☐ Performance Antipatterns
│   │   ├── ☐ Improper Instantiation / Busy Database / Busy Frontend
│   │   ├── ☐ Monolithic Persistence / Noisy Neighbor / Chatty I/O
│   │   └── ☐ Synchronous I/O / Retry Storm / Extraneous Fetching / No Caching
│   └── ☐ Monitoring
│       ├── ☐ Health / Availability / Performance Monitoring
│       ├── ☐ Security / Usage Monitoring
│       └── ☐ Instrumentation / Visualization & Alerts
│
├── ☐ Cloud Design Patterns
│   ├── ☐ Design & Implementation
│   │   ├── ☐ Strangler Fig / Sidecar / Static Content Hosting
│   │   ├── ☐ Leader Election / CQRS / Pipes & Filters / Ambassador
│   │   └── ☐ Gateway patterns / External Config Store / BFF / Anti-Corruption Layer
│   ├── ☐ Data Management
│   │   └── ☐ Valet Key / Sharding / Materialized View / Index Table / Event Sourcing / CQRS / Cache-Aside
│   └── ☐ Messaging
│       └── ☐ Sequential Convoy / Queue-based Load Leveling / Pub/Sub / Priority Queue / Pipes and Filters / Competing Consumers / Choreography / Claim Check / Async Request Reply
│
└── ☐ Reliability Patterns
    ├── ☐ Availability
    │   └── ☐ Deployment Stamps / Geodes / Throttling / Health Endpoint Monitoring / Queue-Based Load Leveling
    ├── ☐ High Availability
    │   └── ☐ Deployment Stamps / Geodes / Bulkhead / Health Endpoint Monitoring / Circuit Breaker
    ├── ☐ Resiliency
    │   └── ☐ Bulkhead / Circuit Breaker / Compensating Transaction / Health Endpoint Monitoring / Leader Election / Queue-Based Load Leveling / Retry / Scheduler Agent Supervisor
    └── ☐ Security
        └── ☐ Federated Identity / Gatekeeper / Valet Key
```

## Completion checklist

- [ ] **Introduction**
  - [ ] What is System Design?
  - [ ] How to approach System Design?
- [ ] **Performance and scalability**
  - [ ] Performance vs Scalability
  - [ ] Latency vs Throughput
- [ ] **Availability and consistency**
  - [ ] CAP Theorem
    - [ ] AP - Availability + Partition Tolerance
    - [ ] CP - Consistency + Partition Tolerance
  - [ ] Consistency Patterns
    - [ ] Weak Consistency
    - [ ] Eventual Consistency
    - [ ] Strong Consistency
- [ ] **Availability patterns**
  - [ ] Fail-Over
    - [ ] Active-Active
    - [ ] Active-Passive
  - [ ] Replication
    - [ ] Master-Slave
    - [ ] Master-Master
  - [ ] Availability in Numbers
    - [ ] 99.9% Availability - three 9s
    - [ ] 99.99% Availability - four 9s
    - [ ] Availability in Parallel vs Sequence
- [ ] **Background jobs**
  - [ ] Event-Driven
  - [ ] Schedule Driven
  - [ ] Returning Results
- [ ] **Networking and application architecture**
  - [ ] Domain Name System
  - [ ] Content Delivery Networks
    - [ ] Pull CDNs
    - [ ] Push CDNs
  - [ ] Load Balancers
    - [ ] LB vs Reverse Proxy
    - [ ] Load Balancing Algorithms
    - [ ] Layer 7 Load Balancing
    - [ ] Layer 4 Load Balancing
    - [ ] Horizontal Scaling
  - [ ] Application Layer
    - [ ] Microservices
    - [ ] Service Discovery
- [ ] **Databases**
  - [ ] SQL vs NoSQL
  - [ ] RDBMS
    - [ ] Replication
    - [ ] Sharding
    - [ ] Federation
    - [ ] Denormalization
    - [ ] SQL Tuning
  - [ ] NoSQL
    - [ ] Key-Value Store
    - [ ] Document Store
    - [ ] Wide Column Store
    - [ ] Graph Databases
- [ ] **Caching**
  - [ ] Strategies
    - [ ] Refresh Ahead
    - [ ] Write-behind
    - [ ] Write-through
    - [ ] Cache Aside
  - [ ] Types of Caching
    - [ ] Client Caching
    - [ ] CDN Caching
    - [ ] Web Server Caching
    - [ ] Database Caching
    - [ ] Application Caching
- [ ] **Asynchronism**
  - [ ] Back Pressure
  - [ ] Task Queues
  - [ ] Message Queues
- [ ] **Idempotent operations**
- [ ] **Communication**
  - [ ] HTTP
  - [ ] TCP
  - [ ] UDP
  - [ ] RPC
  - [ ] gRPC
  - [ ] REST
  - [ ] GraphQL
- [ ] **Performance antipatterns**
  - [ ] Improper Instantiation
  - [ ] Busy Database
  - [ ] Monolithic Persistence
  - [ ] Busy Frontend
  - [ ] Noisy Neighbor
  - [ ] Chatty I/O
  - [ ] Synchronous I/O
  - [ ] Retry Storm
  - [ ] Extraneous Fetching
  - [ ] No Caching
- [ ] **Monitoring**
  - [ ] Health Monitoring
  - [ ] Availability Monitoring
  - [ ] Performance Monitoring
  - [ ] Security Monitoring
  - [ ] Usage Monitoring
  - [ ] Instrumentation
  - [ ] Visualization & Alerts
- [ ] **Cloud design patterns**
  - [ ] Design & Implementation
    - [ ] Strangler Fig
    - [ ] Sidecar
    - [ ] Static Content Hosting
    - [ ] Leader Election
    - [ ] CQRS
    - [ ] Pipes & Filters
    - [ ] Ambassador
    - [ ] Gateway Routing
    - [ ] Gateway Offloading
    - [ ] Gateway Aggregation
    - [ ] External Config Store
    - [ ] Compute Resource Consolidation
    - [ ] Backends for Frontend
    - [ ] Anti-Corruption Layer
  - [ ] Data Management
    - [ ] Valet Key
    - [ ] Static Content Hosting
    - [ ] Sharding
    - [ ] Materialized View
    - [ ] Index Table
    - [ ] Event Sourcing
    - [ ] CQRS
    - [ ] Cache-Aside
  - [ ] Messaging
    - [ ] Sequential Convoy
    - [ ] Scheduling Agent Supervisor
    - [ ] Queue-based Load Leveling
    - [ ] Publisher/Subscriber
    - [ ] Priority Queue
    - [ ] Pipes and Filters
    - [ ] Competing Consumers
    - [ ] Choreography
    - [ ] Claim Check
    - [ ] Async Request Reply
- [ ] **Reliability patterns**
  - [ ] Availability
    - [ ] Deployment Stamps
    - [ ] Geodes
    - [ ] Throttling
    - [ ] Health Endpoint Monitoring
    - [ ] Queue-Based Load Leveling
  - [ ] High Availability
    - [ ] Deployment Stamps
    - [ ] Geodes
    - [ ] Bulkhead
    - [ ] Health Endpoint Monitoring
    - [ ] Circuit Breaker
  - [ ] Resiliency
    - [ ] Bulkhead
    - [ ] Circuit Breaker
    - [ ] Compensating Transaction
    - [ ] Health Endpoint Monitoring
    - [ ] Leader Election
    - [ ] Queue-Based Load Leveling
    - [ ] Retry
    - [ ] Scheduler Agent Supervisor
  - [ ] Security
    - [ ] Federated Identity
    - [ ] Gatekeeper
    - [ ] Valet Key

## Related roadmaps

- [ ] Backend Roadmap
- [ ] DevOps Roadmap
- [ ] Software Design and Architecture

For the detailed roadmap and similar learning paths, see [roadmap.sh](https://roadmap.sh/).
