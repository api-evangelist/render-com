# Render (render-com)

Render is a unified cloud application platform (PaaS) for building, deploying, and scaling web services, static sites, private services, background workers, cron jobs, and one-off jobs alongside managed Postgres and Key Value (Redis-compatible) datastores. The Render REST API (`https://api.render.com/v1`) exposes almost all Render Dashboard capabilities - services, deploys, custom domains, environment variables and groups, persistent disks, Blueprints, projects and environments, metrics, and logs - authenticated with a Bearer API key. Render also documents a public WebSocket surface for real-time log streaming at `wss://api.render.com/v1/logs/subscribe`.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/apis.yml)

## Tags

- Cloud Hosting
- PaaS
- Deployment
- Web Services
- Databases
- DevOps

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Render Services API

Create, list, retrieve, update, and delete Render services (web services, static sites, private services, background workers, and cron jobs), plus scale, autoscale, restart, suspend, resume, purge cache, and spin up service previews.

- **Human URL:** [https://api-docs.render.com/reference/list-services](https://api-docs.render.com/reference/list-services)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Services
- Web Services
- Deployment

#### Properties

- [Documentation](https://render.com/docs/api)
- [API Reference](https://api-docs.render.com/reference/list-services)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Deploys API

Trigger, list, retrieve, and cancel deploys for a service, and roll a service back to a previous deploy. Each deploy captures the build and release of a commit or image for the service.

- **Human URL:** [https://api-docs.render.com/reference/create-deploy](https://api-docs.render.com/reference/create-deploy)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Deploys
- Builds
- Rollback

#### Properties

- [API Reference](https://api-docs.render.com/reference/create-deploy)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Custom Domains API

Add, list, retrieve, delete, and verify custom domains attached to a service, including the DNS records and automatic TLS certificate provisioning Render manages for each domain.

- **Human URL:** [https://api-docs.render.com/reference/list-custom-domains](https://api-docs.render.com/reference/list-custom-domains)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Custom Domains
- DNS
- TLS

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-custom-domains)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Environment Variables & Secret Files API

Manage per-service environment variables and secret files - list, replace the full set, and get, upsert, or delete individual keys and files that are injected into a service at build and runtime.

- **Human URL:** [https://api-docs.render.com/reference/get-env-vars-for-service](https://api-docs.render.com/reference/get-env-vars-for-service)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Environment Variables
- Secret Files
- Configuration

#### Properties

- [API Reference](https://api-docs.render.com/reference/get-env-vars-for-service)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Environment Groups API

Create and manage environment groups - reusable bundles of environment variables and secret files that can be linked to multiple services - and upsert or remove individual variables within a group.

- **Human URL:** [https://api-docs.render.com/reference/list-environment-groups](https://api-docs.render.com/reference/list-environment-groups)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Environment Groups
- Shared Config
- Secrets

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-environment-groups)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Postgres API

Provision and manage fully managed Render Postgres instances - create, list, retrieve, update, delete, fetch connection info, suspend and resume, run and list exports, and drive point-in-time recovery and failover.

- **Human URL:** [https://api-docs.render.com/reference/list-postgres](https://api-docs.render.com/reference/list-postgres)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Postgres
- Databases
- Managed Database

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-postgres)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Key Value API

Create and manage Render Key Value instances - a Redis-compatible in-memory datastore for caching and queues. List, create, retrieve, update, delete, and fetch connection info. The legacy Redis API is deprecated in favor of Key Value.

- **Human URL:** [https://api-docs.render.com/reference/list-key-value](https://api-docs.render.com/reference/list-key-value)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Key Value
- Redis
- Cache

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-key-value)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Jobs API

Create, list, and retrieve one-off jobs that run a command in a service's environment as an ephemeral instance, and manage runs of scheduled cron job services. Useful for migrations, batch tasks, and ad-hoc maintenance.

- **Human URL:** [https://api-docs.render.com/reference/list-jobs](https://api-docs.render.com/reference/list-jobs)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Jobs
- One-Off Jobs
- Cron Jobs

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-jobs)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Disks API

Add, list, retrieve, update, and delete persistent disks attached to services, plus list disk snapshots and restore a disk from a snapshot for durable per-service storage.

- **Human URL:** [https://api-docs.render.com/reference/list-disks](https://api-docs.render.com/reference/list-disks)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Disks
- Persistent Storage
- Snapshots

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-disks)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Blueprints API

Manage Blueprints - Render's infrastructure-as-code driven by a `render.yaml` file - by validating specs, listing, retrieving, updating, disconnecting Blueprints, and inspecting their sync history.

- **Human URL:** [https://api-docs.render.com/reference/list-blueprints](https://api-docs.render.com/reference/list-blueprints)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Blueprints
- Infrastructure as Code
- render.yaml

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-blueprints)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Projects & Environments API

Organize resources into projects and their environments (for example production, staging, development) - create, list, retrieve, update, and delete projects and environments and map services and datastores into them.

- **Human URL:** [https://api-docs.render.com/reference/list-projects](https://api-docs.render.com/reference/list-projects)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Projects
- Environments
- Organization

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-projects)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Workspaces & Members API

List and retrieve the workspaces (owners) your API key can access, manage workspace members and their roles, and read workspace and organization audit logs. Owner IDs scope most other resources in the API.

- **Human URL:** [https://api-docs.render.com/reference/list-owners](https://api-docs.render.com/reference/list-owners)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Workspaces
- Owners
- Members

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-owners)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Metrics API

Query time-series metrics for services and datastores - CPU, memory, bandwidth, instance count, HTTP request counts and latency, active connections, and disk usage - for dashboards, alerting, and capacity planning.

- **Human URL:** [https://api-docs.render.com/reference/get-cpu](https://api-docs.render.com/reference/get-cpu)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Metrics
- Observability
- Monitoring

#### Properties

- [API Reference](https://api-docs.render.com/reference/get-cpu)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Logs API

Query historical logs across services, datastores, jobs, and cron jobs with rich filters and timestamp pagination via `GET /logs`, and subscribe to real-time logs over a documented WebSocket at `wss://api.render.com/v1/logs/subscribe`.

- **Human URL:** [https://api-docs.render.com/reference/list-logs](https://api-docs.render.com/reference/list-logs)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Logs
- Streaming
- WebSocket

#### Properties

- [Documentation](https://api-docs.render.com/reference/list-logs)
- [API Reference](https://api-docs.render.com/reference/subscribe-logs)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/render-com-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Render Webhooks API

Register and manage outbound webhooks that Render calls when platform events occur (deploys, service and datastore lifecycle changes) - create, list, retrieve, update, and delete webhooks and inspect their delivered events.

- **Human URL:** [https://api-docs.render.com/reference/list-webhooks](https://api-docs.render.com/reference/list-webhooks)
- **Base URL:** `https://api.render.com/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [API Reference](https://api-docs.render.com/reference/list-webhooks)
- [OpenAPI](openapi/render-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/render-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/render-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/renderinc)
- [LinkedIn](https://www.linkedin.com/company/renderco)
- [Website](https://render.com)
- [Documentation](https://render.com/docs)
- [Plans](plans/render-com-plans-pricing.yml)
- [Rate Limits](rate-limits/render-com-rate-limits.yml)
- [Fin Ops](finops/render-com-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
