# Felipe Veas

## Senior Site Reliability Engineer — Platform Reliability & Operations

**Most reliability problems are organizational, not technical.**

Senior SRE with 8+ years in production operations. I specialize in taking unstable production environments and building the infrastructure, observability, and operational practices to make them reliable.

Most recently, I operated a B2B SaaS platform serving **100+ developers** (~60 services, 29M+ requests/day). I reduced critical incidents from daily occurrences to 1–2/month, migrated **1,200+ resources across 4 cloud providers** to Terraform, and built the observability and incident response frameworks from scratch. Previously, I maintained high-concurrency platforms serving **1M+ users** with a 99.9% SLA.

I write operational tooling in Python and Go.

---

## 🛠 Tech Stack & Expertise

- **Platform & Containers:** Kubernetes (GKE, k3d), ArgoCD, Helm, Kyverno
- **Infrastructure as Code:** Terraform, Packer
- **Cloud Providers:** GCP, AWS, Azure, DigitalOcean
- **Observability:** Datadog, Elastic Stack (ELK), Prometheus/Grafana
- **Languages:** Python, Go, Bash
- **CI/CD & Automation:** GitHub Actions, GitLab CI, GitOps

---

## 🏗 What I Actually Run

### Kubernetes Platform (GitOps + Terraform)

Production-style platform showing how infrastructure and workloads can be operated safely and independently.

[→ felipe-veas/homelab-platform](https://github.com/felipe-veas/homelab-platform)

#### Key properties & Outcomes

- App-of-apps GitOps deployment model (ArgoCD) for declarative workload delivery
- Policy enforcement (Kyverno) and security scanning (Trivy)
- Reproducible cluster bootstrap with clear ownership boundaries
- Safer change management and drift detection

---

## ⚙️ Operational Tooling

I build internal CLI tools to improve operational visibility, accelerate incident resolution, and reduce manual work. Most of this tooling is private, but here is what it covers:

### Diagnostics & Observability (Python)

- **Multi-node uWSGI monitor** — TUI with real-time worker status, emergency kill, Datadog integration, and multi-country infrastructure support.
- **Cloud SQL query tracker** — Real-time view of active, idle, and blocked queries via IAP tunneling, with Slack alerting.
- **GCP Load Balancer log analyzer** — Traffic classification, P95/P99 latency, and monthly trend reports.

### LLM-powered tools (Python & Go)

- **SQL-to-Django-ORM reverse mapper** — Indexes Django codebase and predicts which ORM functions generate a given SQL query.
- **Infrastructure reporting** — Automated weekly Datadog/GCP reports with capacity recommendations and cost optimization estimates.
- **Code review bot** (Go) — Hybrid static rules + LLM analysis for PR review in CI/CD pipelines.

### Public tools

- **dotctl** — CLI for managing and versioning dotfiles across machines [→ felipe-veas/dotctl](https://github.com/felipe-veas/dotctl)
- **homebrew-tap** — Standardized tool distribution [→ felipe-veas/homebrew-tap](https://github.com/felipe-veas/homebrew-tap)

---

## 📚 Production Reliability Notes

I maintain repositories documenting how real production systems behave and how teams operate them under pressure. These are not tutorials — they are operational reliability notes.

- **[Operating Production Systems](https://github.com/felipe-veas/operating-production-systems)**
- **[Handling Production Incidents](https://github.com/felipe-veas/handling-production-incidents)**
- **[Reducing Operational Toil](https://github.com/felipe-veas/reducing-operational-toil)**
- **[Platform Engineering Model](https://github.com/felipe-veas/platform-engineering-model)**
- **[Observability in Production](https://github.com/felipe-veas/observability-in-production)**

---

## 🧠 Operating Philosophy

Production reliability is achieved through safer operational systems, not stronger infrastructure.

### Failures usually come from

- Unclear ownership
- Unsafe change processes
- Alerting that does not guide action
- Poor incident coordination

**I design systems where the correct operational action is the easiest action.**

---

## 📫 Contact

[→ linkedin.com/in/felipe-veas](https://linkedin.com/in/felipe-veas)
