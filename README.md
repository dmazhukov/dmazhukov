# Dmitrii Zhukov — Senior DevOps / Platform / SRE Engineer

Infrastructure engineer focused on **Kubernetes reliability**, **observability stacks**, and **PostgreSQL HA operations**. 20+ years in tech — 14 as a .NET developer and tech lead, 6+ in DevOps and cloud infrastructure.

Based in Vietnam 🇻🇳 · Remote worldwide · GMT+7

---

## What I work on

- **Kubernetes** — Production clusters across GKE, kubeadm and Rancher — cloud and on-premise including offline-tolerant ship environments (ships with satellite connectivity — not your typical infra problem).
- **Observability** — Prometheus, Grafana, Istio service mesh with distributed tracing.
- **PostgreSQL** — HA clusters with Patroni, streaming replication, failover testing, performance tuning.
- **IaC** — Terraform, Ansible, Helm. Infrastructure treated the same as application code: PR reviews, tested pipelines, no manual snowflakes.
- **CI/CD** — Jenkins, GitLab CI, GitHub Actions, Codefresh. Pre-deployment validation, staged rollouts, observability-driven rollback gates.

---

## Featured

### 🛡️ [cronguard](https://github.com/dmazhukov/cronguard) — Kubernetes operator (Go)

SLO-style observability for Kubernetes CronJobs. Wraps `batch/v1.CronJob` workloads with a `CronJobMonitor` CRD that declares per-CronJob SLOs (schedule, max duration, max consecutive failures, missed-run tolerance), surfaces them as `cronguard_*` Prometheus metrics, and ships a default `PrometheusRule` with five alerts and runbooks.

- ~1500 lines Go on kubebuilder v4 + controller-runtime
- Coverage: 82.9% controller · 95.0% schedule · 95.8% history · 94.9% metrics
- Multi-arch image · Helm chart on OCI + GitHub Pages · listed on Artifact Hub
- kind-based e2e on every push + nightly schedule

### 📊 [prometheus-alerting-rules](https://github.com/dmazhukov/prometheus-alerting-rules)

Production-grade Prometheus alerting rules for Kubernetes, PostgreSQL/Patroni, and SLO burn rate alerting — with runbooks.

Covers:
- Pod crash-loop, OOM, PVC fill-up, deployment rollout stuck
- Patroni cluster health, replication lag, XID wraparound
- Multi-window SLO burn rate (Google SRE method)
- Node disk, network, clock skew

---

## Stack

```
Orchestration   Kubernetes (GKE · kubeadm · Rancher) · Docker · Helm
Cloud           GCP · AWS · DigitalOcean · Yandex.Cloud · Alibaba Cloud
Observability   Prometheus · Grafana · Istio · ELK · Dynatrace
Databases       PostgreSQL · Patroni · MS SQL · Oracle
IaC             Terraform · Ansible
CI/CD           Jenkins · GitLab CI · GitHub Actions · Codefresh
Scripting       Python · Bash · Go
```

---

## By the numbers

| Achievement | Result |
|---|---|
| Production release failures | −90% (from ~10 to ~1/year) |
| System uptime | 99.8% for cruise operations |
| Cloud migration | Zero downtime · −30% cost |
| CI/CD speed | −75% deployment time |
| IAM security incidents | −60% after RBAC reorganization |
| PostgreSQL HA | 99.95% uptime · <30s failover |

---

## Connect

- 💼 [LinkedIn](https://www.linkedin.com/in/dmitrii-zhukov-senior-devops/)
- 📬 dmitry0983@gmail.com
- 💬 Telegram: @dmazhukov
