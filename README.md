<p align="center">
  <b>Senior Backend Engineer · Go</b><br/>
  Event-driven microservices · high-load systems · consistency in distributed systems
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/oleg-potapov-dev/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-oleg--potapov--dev-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <img alt="Location" src="https://img.shields.io/badge/Yerevan%2C%20Armenia-remote%20%2F%20hybrid-2ea44f?style=flat-square">
  <img alt="Experience" src="https://img.shields.io/badge/backend-3.5%2B%20years-00ADD8?style=flat-square&logo=go&logoColor=white">
</p>

---

I build backend systems in Go that move money, people and events between dozens of services — payroll, HR and analytics platforms at **Wildberries** and **M.Video**, where correctness under retries and peak load matters more than anything else.

- **Event-driven architecture** — Kafka, Transactional Outbox, idempotent consumers, sagas, CQRS
- **High load** — services sustaining tens of thousands of RPS at 99.9% uptime
- **End-to-end ownership** — from requirements with business stakeholders to Kubernetes, Grafana dashboards and alerting
- **Team** — coordinated a team of 4, interviewed Go candidates, mentored interns
- **LLM / AI integrations** in backend services

## Production work

> Closed-source, so here is what was built and what it changed.

| | |
|---|---|
| **M.Video**<br/><sub>2025 – 2026</sub> | Built the internal **HR platform from scratch** (Go, PostgreSQL, Kafka) — the employee source of truth for a 50,000-person retailer, absorbing ~11k HR events/month and serving **20+ downstream services** over gRPC and HTTP. Transactional Outbox + Redis-backed idempotent consumers from day one: no dual writes, no duplicates under retries. Rebuilt the org-structure hierarchy from Kafka event streams during a live migration off the legacy source. Hiring backend for **20 warehouses / ~1,000 hires a month**. |
| **Wildberries Tech**<br/><sub>2024 – 2025</sub> | End-to-end **payroll platform**: source-data collection → accruals and gross-to-net → payments via payment gateways and accounting. Designed a **high-load accruals analytics system** — tens of thousands of RPS at peak, 99.9% uptime, became the primary tool in its area. Split a distributed monolith into bounded contexts and moved business-critical service-to-service traffic onto Kafka. |
| **Tutu**<br/><sub>2023 – 2024</sub> | Travel platform: new modules end-to-end, integrations with **10+ external systems**, customer booking notifications, automated testing in CI/CD. |

## Featured projects

| Project | What it demonstrates |
|---|---|
| [**awesome-chat-backend**](https://github.com/D1sordxr/awesome-chat-backend) | Real-time chat: WebSocket gateway → Redis Streams → batched, ack-after-commit writes to PostgreSQL; Transactional Outbox → Kafka; voice messages in MinIO |
| [**awesome-chat-proto**](https://github.com/D1sordxr/awesome-chat-proto) | Contract-first API: Protobuf + Buf, gRPC-Gateway, `protovalidate`, breaking-change checks in CI |
| [**simple-bank**](https://github.com/D1sordxr/simple-bank) | Event-driven banking: CQRS over gRPC, event store + outbox in one transaction, idempotent Kafka consumers |
| [**image-processor**](https://github.com/D1sordxr/image-processor) | Async image pipeline: Kafka jobs, MinIO (S3) storage, status tracking in PostgreSQL |
| [**delayed-notifier**](https://github.com/D1sordxr/delayed-notifier) | Scheduled notifications: horizontally scalable workers (`FOR UPDATE SKIP LOCKED`), RabbitMQ with TTL + dead-letter queues, Redis read cache |
| [**url-shortener**](https://github.com/D1sordxr/url-shortener) | OpenAPI-first URL shortener: non-blocking redirects with async visit tracking, SQL analytics (daily stats, unique visitors, user agents) |

## Stack

<p>
  <img src="https://skillicons.dev/icons?i=go,postgres,kafka,redis,rabbitmq,kubernetes,docker,grafana,githubactions,linux,python,ts,react&perline=13" alt="Go, PostgreSQL, Kafka, Redis, RabbitMQ, Kubernetes, Docker, Grafana, GitHub Actions, Linux, Python, TypeScript, React" />
</p>

- **Core:** Go · PostgreSQL · Apache Kafka · Redis · gRPC / Protobuf
- **Infrastructure:** Kubernetes · Docker · CI/CD · Grafana · distributed tracing · MinIO / S3 · RabbitMQ
- **Practices:** DDD & Clean Architecture · Transactional Outbox · Saga · CQRS · idempotency · contract-first APIs · code generation

## Contact

The best way to reach me is [LinkedIn](https://www.linkedin.com/in/oleg-potapov-dev/).
