## Hi, I'm Ozan 👋

Senior DevOps / Site Reliability / Platform Engineer with 10+ years of experience, based in Turkey and working remotely.

I build and run cloud platforms for high-traffic fintech and iGaming products: multi-cluster **Amazon EKS** with disaster recovery, **GitOps with Argo CD**, **Terraform / Terragrunt** for everything, and observability with **Prometheus, Grafana, Loki and VictoriaMetrics**. Lately I've been adding LLM-assisted tooling to incident response.


### 📌 Featured projects

| Project | What it shows |
|---|---|
| [terraform-aws-eks-platform](https://github.com/ozy31/terraform-aws-eks-platform) | Production-style EKS platform: VPC, EKS, Karpenter, platform add-ons and Argo CD bootstrap; Terragrunt live layout for dev / prod / prod-dr |
| [terraform-azure-aks-platform](https://github.com/ozy31/terraform-azure-aks-platform) | Self-service AKS platform: Entra ID + namespace-scoped Azure RBAC, workload identity, Node Auto-Provisioning, Flux via the AKS extension, Istio Gateway API, Gatekeeper policies tested with gator, one-file team onboarding |
| [bicep-azure-aks-platform](https://github.com/ozy31/bicep-azure-aks-platform) | The same private AKS platform in Bicep: hub-spoke networking, Entra ID-only cluster, workload identity, private Key Vault and ACR, managed Prometheus alerts, deployed as a deployment stack with deny settings; security baseline tests on the compiled template, OIDC what-if in CI |
| [terraform-azure-landing-zone](https://github.com/ozy31/terraform-azure-landing-zone) | Azure landing zone: CAF management groups, policy-as-code by management group, hub with Azure Firewall + DNS Private Resolver, subscription vending with azapi from one YAML file per team |
| [terraform-aws-eks-ai-cluster](https://github.com/ozy31/terraform-aws-eks-ai-cluster) | GPU / LLM inference on EKS: Karpenter GPU NodePools, NVIDIA device plugin + DCGM alerts, S3 model store via Mountpoint, vLLM scaled by KEDA on request queue depth |
| [k8s-postgres-platform](https://github.com/ozy31/k8s-postgres-platform) | PostgreSQL on Kubernetes with CloudNativePG: three zones, quorum commit, PgBouncer, PITR, major upgrades and a Helm chart for tenant databases; failover (~16 s, zero lost writes) measured in CI |
| [rds-to-k8s-migration](https://github.com/ozy31/rds-to-k8s-migration) | RDS PostgreSQL -> CloudNativePG under live writes: logical replication, cutover with ~2 s of frozen writes and checksum checks, a rollback through reverse replication that loses nothing, and a point-in-time restore drill; RDS MySQL -> MOCO through a GTID relay in progress |
| [k8s-supply-chain-security](https://github.com/ozy31/k8s-supply-chain-security) | Only images our pipeline built, scanned and signed get to run: SBOM and vulnerability attestations with cosign, Kyverno 1.20 CEL policies that refuse unsigned, re-tagged, stale-scan and CRITICAL-CVE images, keyless GitHub release with SLSA provenance; 12 admission cases tested on kind in CI |
| [terraform-cloudflare-edge](https://github.com/ozy31/terraform-cloudflare-edge) | Cloudflare edge as code: WAF + OWASP, geo-fencing with partner bypass, rate limits, Logpush to tiered S3 and OpenSearch, Tunnel + Access for internal tools and a self-hosted LLM, AI Gateway |
| [cloudflare-edge-platform](https://github.com/ozy31/cloudflare-edge-platform) | Cloudflare in front of Kubernetes with no public load balancer: outbound-only Tunnel with kind e2e checks, WAF and rate-limit rules as reviewed YAML with 29 Terraform tests, Logpush to R2 queried with DuckDB, incident runbooks |
| [edge-llm-gateway](https://github.com/ozy31/edge-llm-gateway) | OpenAI-compatible LLM gateway on Cloudflare Workers: per-team keys, rate limits and monthly token budgets in Durable Objects, fallback with circuit breakers, streaming usage metering, PII redaction; 62 tests in the Workers runtime, Terraform for the edge |
| [eks-to-onprem-repatriation](https://github.com/ozy31/eks-to-onprem-repatriation) | Phased EKS -> on-prem migration: Talos, Cilium BGP, Rook-Ceph, CloudNativePG logical replication with a rollback path, Strimzi MirrorMaker 2, Cloudflare weighted traffic shift, TCO model |
| [gitops-multicluster-dr](https://github.com/ozy31/gitops-multicluster-dr) | Argo CD ApplicationSet matrix generators across environments and clusters, plus `drswitch`, a Go CLI for single-switch DR failover |
| [aiops-incident-assistant](https://github.com/ozy31/aiops-incident-assistant) | Alertmanager webhook → logs and metrics context → LLM incident summary in Slack, with secret redaction |
| [postgres-ops-agent](https://github.com/ozy31/postgres-ops-agent) | Read-only MCP server and Claude Code skill for Postgres incident triage: least-privilege identities, human-approved actions with an audit log, fault-injection evals |
| [platform-ci-templates](https://github.com/ozy31/platform-ci-templates) | Reusable GitHub Actions, GitLab CI, Bitbucket Pipelines and Jenkins templates: OIDC to AWS, SBOM, image signing, GitOps promotion |
| [k8s-observability-stack](https://github.com/ozy31/k8s-observability-stack) | GitOps-ready Prometheus, Grafana, Loki and VictoriaMetrics with SLO burn-rate alerts, rule unit tests and dashboards |
| [tf-modules](https://github.com/ozy31/tf-modules) | Small, readable Terraform modules: VPC, EKS, add-ons with IRSA, Argo CD and RDS with External Secrets |

### 🧰 Toolbox

**Cloud:** AWS (EKS, EC2, VPC, IAM, MSK, RDS), Azure (AKS, Azure DevOps, Azure Policy, Azure Firewall), Cloudflare
**Kubernetes:** EKS, AKS, Helm, Karpenter, KEDA, Cilium, Argo CD
**IaC:** Terraform, Terragrunt, OpenTofu
**CI/CD:** GitHub Actions, Bitbucket Pipelines, GitLab CI, Jenkins, TeamCity, Octopus Deploy
**Observability:** Prometheus, Grafana, Loki, VictoriaMetrics, Elasticsearch, PagerDuty
**Data and messaging:** Kafka, RabbitMQ, MongoDB, PostgreSQL (CloudNativePG), SQL Server
**Languages:** Python, Go, Bash

**Certifications:** HashiCorp Terraform Associate · CKAD · AWS Cloud Practitioner

### 📫 Contact

[LinkedIn](https://linkedin.com/in/a-ozan-gazi) · aogazi31@gmail.com
