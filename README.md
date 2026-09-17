# Hi, I'm Balaji K 

**Backend Engineer**

I build and operate high-throughput backend services. Currently a Software Engineer at **Myntra**, working on search and ranking systems that serve traffic at **120K+ RPM** — ranking pipelines, latency debugging, and the unglamorous production reliability work that keeps them up during sale events.

Most of what I enjoy sits at the boundary between correctness and performance: what happens to a system under concurrency, under fan-out, and under partial failure.

```
Java  ·  Spring Boot  ·  Distributed Systems  ·  Redis  ·  Kafka  ·  Kubernetes
```

---

##  Projects

###  Distributed Rate Limiter
`Java` `Spring Boot` `Redis` `Lua` `Caffeine` `Docker`

A standalone rate-limiting service with pluggable **token bucket**, **sliding window log**, and **sliding window counter** algorithms — usable both as an embeddable library and an HTTP API.

- Atomic **Redis Lua scripts** eliminate the check-then-set race that lets distributed clients overshoot a shared limit
- **Caffeine L1 cache** tier with a quantified accuracy bound, trading exactness for round-trips
- Configurable **fail-open / fail-closed** policy for Redis unavailability

###  Sharded Search & Ranking Service `WIP`
`Java 21` `Spring Boot` `Lucene` `Redis` `Kafka` `Kubernetes`

A distributed search engine built from the ground up — custom scatter-gather coordinator over Lucene-backed shards, deliberately avoiding an off-the-shelf engine so the hard parts stay mine to solve.

- Fan-out tail amplification: why coordinator p99 ≫ shard p99, and what to do about it
- **Adaptive per-shard timeouts**, hedged requests with cancellation, k-of-n partial results
- Two-stage retrieval + feature-based re-ranking with batched Redis lookups

###  Idempotent Payment Ledger `Planned`
`Java` `Spring Boot` `PostgreSQL` `Kafka` `Testcontainers`

Double-entry ledger with exactly-once semantics under concurrent retries — idempotency key arbitration, transactional outbox, and a property-based suite proving the ledger invariant holds under injected failure.

---

##  Tech

**Languages**
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)

**Backend & Data**
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat&logo=elasticsearch&logoColor=white)

**Infrastructure & Observability**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)

---
<sub>Open to conversations about distributed systems, search, and anything with an interesting failure mode.</sub>
