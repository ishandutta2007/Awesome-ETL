# Awesome-ETL

# Top Background Job Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Background Jobs, Durable Workflows, Task Queues, Event-Driven Functions, Retries, Scheduling & Long-Running Processes*
**Last updated: August 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Background Job** and durable execution systems. These tools reliably run asynchronous work — emails, webhooks, data processing, AI pipelines, scheduled tasks, and multi-step workflows — with retries, state persistence, and observability.

**Examples** include Trigger.dev, Inngest, Hatchet, Temporal Cloud, QStash, Cloud Tasks, Sidekiq Enterprise, BullMQ Pro, IronWorker, and Restate (the category leaders).

**Open-source emphasis**: This section is heavily expanded. Many leading platforms (Temporal, Trigger.dev, Inngest, Hatchet, Sidekiq, BullMQ) offer strong open-source cores, making self-hosted, production-grade background job systems widely accessible.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Trigger.dev](https://trigger.dev/)**  
  TypeScript-first background jobs and AI workflow platform with long-running task support, checkpoint-resume, and excellent developer experience (open-source core available).

- **[Inngest](https://www.inngest.com/)**  
  Event-driven durable functions and step-workflow platform that runs on your existing infrastructure or managed cloud, with strong TypeScript/Python support.

- **[Hatchet](https://hatchet.run/)**  
  High-throughput open-source task orchestration platform focused on reliability, concurrency control, and AI/data pipelines (managed offering available).

- **[Temporal Cloud](https://temporal.io/)**  
  Managed service of the Temporal workflow engine — the enterprise standard for durable, long-running, multi-language orchestration.

- **[QStash (Upstash)](https://upstash.com/qstash)**  
  Serverless message queue and scheduling service designed for HTTP-based background jobs and durable workflows.

- **[Google Cloud Tasks](https://cloud.google.com/tasks)**  
  Fully managed task queue service for asynchronous execution of HTTP or App Engine tasks on Google Cloud.

- **[Sidekiq Enterprise](https://sidekiq.org/)**  
  Commercial offering built on the popular open-source Sidekiq Ruby background job framework, adding advanced features and support.

- **[BullMQ Pro](https://bullmq.io/)**  
  Commercial enhancements and support for the widely used open-source BullMQ Redis-based job queue.

- **[IronWorker](https://www.iron.io/)**  
  Cloud-based background job and worker platform supporting multiple languages and containerized workloads.

- **[Restate](https://restate.dev/)**  
  Durable execution and workflow platform focused on reliability, recovery, and developer-friendly orchestration primitives.

## Open-Source GitHub Projects
- **[Temporal](https://github.com/temporalio/temporal)**  
  Leading open-source durable workflow and microservice orchestration platform with SDKs for Go, Java, TypeScript, Python, and more.

- **[Trigger.dev](https://github.com/triggerdotdev/trigger.dev)**  
  Open-source background jobs framework for TypeScript, supporting long-running tasks, AI workflows, and self-hosting.

- **[Inngest](https://github.com/inngest/inngest)**  
  Open-source event-driven durable execution engine with step functions, retries, and observability.

- **[Hatchet](https://github.com/hatchet-dev/hatchet)**  
  Open-source, high-performance task queue and workflow orchestration system designed for scale and developer experience.

- **[BullMQ](https://github.com/taskforcesh/bullmq)**  
  Fast, reliable, Redis-based (and PostgreSQL-capable) distributed job queue for Node.js and multiple other languages.

- **[Sidekiq](https://github.com/sidekiq/sidekiq)**  
  The dominant open-source background job framework for Ruby, known for performance and simplicity.

- **[Celery](https://github.com/celery/celery)**  
  Mature, widely used open-source distributed task queue for Python with support for multiple brokers.

- **[RQ (Redis Queue)](https://github.com/rq/rq)**  
  Simple, lightweight open-source Python library for queueing and processing background jobs with Redis.

- **[Faktory](https://github.com/contribsys/faktory)**  
  Language-agnostic open-source background job server from the creators of Sidekiq.

- **[APScheduler](https://github.com/agronholm/apscheduler)**  
  Advanced open-source Python task scheduling and job queue library supporting persistent storage and multiple backends.

### Additional Strong Open-Source Options
- Bee-Queue, Agenda, and other Node.js Redis/Mongo-backed job libraries.
- Dramatiq and alternative Python task queues focused on simplicity and reliability.
- Laravel Horizon / queues and PHP ecosystem job processors.
- Restate open-source components and emerging durable-execution engines.
- Classic message brokers (RabbitMQ, NATS, Kafka) used as foundations for custom job systems.
- Cron-like schedulers and repeatable job libraries across languages.

**Frameworks for building custom systems**: For durable multi-step workflows choose **Temporal** or **Inngest**; for high-throughput queues use **BullMQ**, **Sidekiq**, or **Hatchet**; for serverless/TypeScript-first jobs use **Trigger.dev**. Pair any of them with Redis, PostgreSQL, or cloud message services, add a monitoring UI (Bull Board, Sidekiq Web, Temporal UI, etc.), and instrument with OpenTelemetry for full visibility. Self-hosting these open-source cores gives complete control over cost and data.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- Background job systems are critical infrastructure. Open-source solutions are production-proven at massive scale but still require careful configuration of retries, dead-letter queues, monitoring, and capacity planning.
- Always design for failure: jobs must be idempotent, and poison messages must be handled gracefully.

---
**Made for backend engineers, platform teams, and developers building reliable asynchronous systems.**
Let's make background jobs and durable workflows more open, observable, and resilient.
