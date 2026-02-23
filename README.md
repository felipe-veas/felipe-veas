# Felipe Veas

Site Reliability Engineer — Platform Reliability & Operations

**Most reliability problems are organizational, not technical.**

SRE with 8+ years in production operations. I specialize in taking unstable production environments and building the infrastructure, observability, and operational practices to make them reliable. Most recently operated a B2B SaaS platform (~60 services, 29M+ requests/day, 4 cloud providers) — reduced critical incidents from daily occurrences to 1–2/month, migrated all infrastructure to Terraform, and built the observability and incident response frameworks from scratch.

I write operational tooling in Python and Go.

---

## What I Actually Run

### Kubernetes Platform (GitOps + Terraform)

Production-style platform showing how infrastructure and workloads can be operated safely and independently.

[→ felipe-veas/homelab-platform](https://github.com/felipe-veas/homelab-platform)

#### Key properties

- App-of-apps GitOps deployment model (ArgoCD)
- Declarative workload delivery
- Policy enforcement (Kyverno)
- Ingress, certificates, and operational services
- Observability stack (metrics + logs)

#### Operational outcomes

- Reproducible cluster bootstrap
- Safer change management
- Drift detection
- Clear ownership boundaries
- Operational visibility of cluster state

---

## Operational Tooling

I build internal CLI tools to improve operational visibility, accelerate incident resolution, and reduce manual work. Most of this tooling is private, but here is what it covers:

#### Diagnostics & Observability (Python)

- **Multi-node uWSGI monitor** — TUI with real-time worker status, emergency kill, Datadog integration, and multi-country infrastructure support
- **Cloud SQL query tracker** — real-time view of active, idle, and blocked queries across production databases via IAP tunneling, with Slack alerting for long-running queries
- **GCP Load Balancer log analyzer** — traffic classification (internal vs external), P95/P99 latency, status code breakdown, and monthly trend reports

#### LLM-powered tools (Python & Go)

- **SQL-to-Django-ORM reverse mapper** — indexes Django codebase and predicts which ORM functions generate a given SQL query, ranked by confidence
- **Infrastructure reporting** — automated weekly Datadog/GCP reports with capacity recommendations and MIG cost optimization estimates
- **Code review bot** (Go) — hybrid static rules + LLM analysis for PR review in CI/CD pipelines, specialized in Django ORM patterns

#### Public tools

- **dotctl** — CLI for managing and versioning dotfiles across machines [→ felipe-veas/dotctl](https://github.com/felipe-veas/dotctl)
- **homebrew-tap** — standardized tool distribution [→ felipe-veas/homebrew-tap](https://github.com/felipe-veas/homebrew-tap)

---

## Production Reliability Notes

I maintain repositories documenting how real production systems behave and how teams operate them under pressure.
These are not tutorials — they are operational reliability notes.

**Operating Production Systems**
[→ felipe-veas/operating-production-systems](https://github.com/felipe-veas/operating-production-systems)

**Handling Production Incidents**
[→ felipe-veas/handling-production-incidents](https://github.com/felipe-veas/handling-production-incidents)

**Reducing Operational Toil**
[→ felipe-veas/reducing-operational-toil](https://github.com/felipe-veas/reducing-operational-toil)

**Platform Engineering Model**
[→ felipe-veas/platform-engineering-model](https://github.com/felipe-veas/platform-engineering-model)

**Observability in Production**
[→ felipe-veas/observability-in-production](https://github.com/felipe-veas/observability-in-production)

---

## What I Work On

- Platform reliability and proactive capacity planning
- Incident response, postmortem processes, and on-call operations
- Kubernetes platform standardization and self-service enablement
- Infrastructure as Code at scale (Terraform, Packer, multi-cloud)
- Observability design (Datadog, Elastic Stack) and alerting strategy
- CI/CD pipeline design for safe, autonomous deployments
- Building diagnostic and operational tooling (Python, Go)
- Reducing operational toil and converting tribal knowledge into runbooks

---

## Operating Philosophy

Production reliability is achieved through safer operational systems, not stronger infrastructure.

#### Failures usually come from

- Unclear ownership
- Unsafe change processes
- Alerting that does not guide action
- Poor incident coordination

I design systems where the correct operational action is the easiest action.

---

## Contact

[→ linkedin.com/in/felipe-veas](https://linkedin.com/in/felipe-veas)
