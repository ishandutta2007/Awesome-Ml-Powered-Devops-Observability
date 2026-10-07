# Awesome-Ml-Powered-Devops-Observability

## Top ML-Powered DevOps Observability Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on AIOps, Anomaly Detection & Self-Hosted Root Cause Analysis*  

**Last updated: October 2026**



This repository tracks notable **commercial ML-powered observability platforms** and **open-source projects** that apply machine learning to IT operations — detecting anomalies, correlating alerts, identifying root causes, and reducing mean time to resolution (MTTR) across cloud-native environments.



**Examples** include Amazon DevOps Guru, Dynatrace Davis, Datadog Watchdog/Bits AI, New Relic Lookout, Moogsoft, BigPanda, ScienceLogic, Splunk ITSI, and PagerDuty AIOps (the category leaders).



**Open-source emphasis**: ML-powered observability is a rapidly maturing open-source domain. **Coroot** leads with eBPF-based zero-instrumentation observability and AI-powered root cause analysis, trusted by SREs worldwide with 7,300+ GitHub stars and 25M+ downloads . **HolmesGPT** brings a CNCF sandbox AI SRE agent that investigates incidents across any stack . **Netdata** applies edge ML to every metric with 18 unsupervised models per dimension . **Apache SkyWalking** provides AI agent observability with distributed tracing . **observability-mcp** delivers MCP-native topology-aware reasoning . **Robusta** offers Kubernetes-native AIOps with pre-built playbooks . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Dynatrace Davis AI](https://www.dynatrace.com/platform/artificial-intelligence/)**

  **Topology-aware causal AI** — maps service dependencies and identifies root cause, not just symptoms . Automatic baselining with seasonality awareness . **The strongest automatic root-cause story** in the category, especially for enterprise-scale Java workloads . Davis CoPilot provides natural-language incident triage with topology context .



- **[Datadog Watchdog & Bits AI](https://www.datadoghq.com/product/platform/watchdog/)**

  **Anomaly detection on the same data that drives Datadog dashboards** . Bits AI provides natural-language incident triage and root-cause hypothesis with trace and log context . **Best for teams already in the Datadog ecosystem** .



- **[New Relic AI (Applied Intelligence & Lookout)](https://newrelic.com/platform/ai)**

  **AI bundled across the platform** — no separate SKU . Applied Intelligence handles alert correlation and noise reduction . Lookout provides per-entity anomaly views . **Best for New Relic users wanting AI without procurement friction** .



- **[Amazon DevOps Guru](https://aws.amazon.com/devops-guru/)**

  **AWS's ML-powered operations service** — detect operational issues and recommend remediation . **Best for AWS-native environments** .



- **[Moogsoft](https://www.moogsoft.com/)**

  **AIOps platform for event correlation and noise reduction** — ML-based alert deduplication . **Best for large-scale incident management** .



- **[BigPanda](https://www.bigpanda.io/)**

  **Event correlation and incident intelligence** — reduces alert noise with ML . **Best for enterprise AIOps** .



- **[ScienceLogic AI Platform](https://sciencelogic.com/)**

  **AIOps for hybrid cloud** — automated discovery, event correlation, and root cause analysis .



- **[Splunk ITSI](https://www.splunk.com/)**

  **IT Service Intelligence** — ML-powered service health monitoring and KPI tracking . **Best for Splunk users** .



- **[PagerDuty AIOps](https://www.pagerduty.com/platform/aiops/)**

  **Incident response with ML-powered alert grouping** — reduce noise and accelerate resolution . **Best for incident management** .



## Open-Source GitHub Projects



### Zero-Instrumentation Observability with AI



- **[Coroot](https://github.com/coroot/coroot)**

  **The leading open-source full-stack observability platform with AI-powered root cause analysis**, Apache-2.0 licensed with **7,300+ GitHub stars** and **25M+ downloads** . **Uses eBPF to capture metrics, logs, traces, and profiles with zero code changes** — no instrumentation required . **Service Map covers 100% of your system with no blind spots** . **AI-powered Root Cause Analysis** traces dependencies and suggests fixes instantly . **Automatically identifies over 80% of issues** . **Deployment tracking** discovers every application rollout and compares releases . **Cost monitoring** for AWS, GCP, and Azure down to specific applications . **The de facto open-source alternative to Dynatrace and Datadog for cost-conscious teams** — trusted by SREs and DevOps teams worldwide .



- **[Netdata](https://github.com/netdata/netdata)**

  **The most cost-aligned AI observability stack**, GPL-3.0 licensed with **70,000+ GitHub stars** . **18 unsupervised ML models per metric with consensus voting** — false positives suppressed at the source . **ML runs on the edge agent, not a SaaS backend** — sub-second detection latency . **Anomaly Advisor** correlates and ranks anomalies during incidents . **AI Co-Engineer (MCP-native)** integrates with Claude, ChatGPT, Gemini for natural-language triage . **Blast Radius detection** surfaces the scope of correlated impact .



### AI SRE Agents & Incident Investigation



- **[HolmesGPT](https://github.com/robusta-dev/holmesgpt)**

  **The CNCF SRE Agent for investigating production incidents**, MIT licensed with **1,235+ GitHub stars** . **Open-source AI agent that works with any stack** — Kubernetes, VMs, cloud providers, databases, and SaaS platforms . **Operator Mode** runs 24/7 in the background, spots problems before customers notice, and messages you in Slack with the fix . **Deep integrations**: Prometheus, Grafana, Datadog, Kubernetes, AWS, GCP, Azure, and many more . **Bidirectional alert integrations** — fetch from AlertManager, PagerDuty, OpsGenie, Jira and write findings back . **Any LLM provider**: OpenAI, Anthropic, Azure, Bedrock, Gemini . **A Cloud Native Computing Foundation sandbox project** originally created by Robusta.Dev with major contributions from Microsoft .



- **[observability-mcp](https://github.com/ThoTischner/observability-mcp)**

  **MCP-native observability with topology-aware reasoning**, Apache-2.0 licensed . **8 tools with full Streamable HTTP transport** — any MCP-speaking agent (Claude Code, etc.) can investigate . **Topology-aware reasoning** — `get_topology` and `get_blast_radius` over a generic kind/relation vocabulary . **Reproducible RCA benchmark in-tree** — `scripts/benchmark-rca.mjs` with raw JSON results . **Multi-backend**: Prometheus, Loki, Kubernetes, Tempo . **Local LLM support** via Ollama — no cloud calls required . **The best MCP-native option for agent-driven observability** .



- **[Robusta](https://github.com/robusta-dev/robusta)**

  **Kubernetes-native AIOps with pre-built playbooks**, MIT licensed . **Slack/web UI focus** for alert correlation and incident response . **Best for Kubernetes-heavy environments** .



- **[KubeIntellect](https://zenodo.org/records/22729414)**

  **LLM-orchestrated multi-agent framework for autonomous Kubernetes operations**, open-source . **Natural-language root-cause analysis** across kubectl, Prometheus, and Loki . **Human-in-the-loop-gated cluster operations** . **Best for autonomous Kubernetes operations** .



### Distributed Tracing & APM



- **[Apache SkyWalking](https://github.com/apache/skywalking)**

  **Application performance monitor for microservices and cloud-native architectures**, Apache-2.0 licensed . **Distributed tracing, service mesh telemetry, metrics aggregation, and alerting** . **AI Sessionizer** provides conversation-level observability for long-lived AI agents . **SkyWalking MCP Server** provides MCP access to observability data . **The most widely adopted open-source APM in Asia** .



- **[Apache SkyWalking AI Sessionizer](https://github.com/apache/skywalking-ai-sessionizer)**

  **Conversation-level observability for long-lived AI agents**, open-source . **Measures and explores conversations and sessions from AI agents** . **Part of the SkyWalking ecosystem** .



### Additional Strong Open-Source Options



- **Lumino MCP Server** — CI/CD pipeline intelligence with ML pattern detection and progressive event analysis .

- **Grafana ML** — Outlier detection, metric forecasting, and adaptive alerting on the LGTM stack . **AI features tier-locked on Grafana Cloud** .

- **Signoz** — Open-source observability platform with logs, traces, and metrics .

- **OpenObserve** — Open-source observability with logs, metrics, and traces .

- **Prometheus** — The de facto standard for metrics monitoring .

- **Jaeger** — Distributed tracing platform .

- **Grafana Tempo** — Distributed tracing backend .

- **OpenTelemetry** — Vendor-neutral instrumentation .



**Frameworks for building custom ML-powered observability solutions**: Combine **Coroot** for eBPF-based zero-instrumentation observability with AI-powered root cause analysis . Use **Netdata** for per-metric edge ML with sub-second detection latency . Deploy **HolmesGPT** for AI SRE agent-driven incident investigation across any stack . Integrate **observability-mcp** for MCP-native topology-aware reasoning with any agent . Choose **Apache SkyWalking** for distributed tracing and AI agent observability . Use **Robusta** for Kubernetes-native AIOps with Slack integration . Note that true enterprise AIOps with topology-aware causal AI, enterprise-scale baselining, and vendor-supported SLAs (Dynatrace Davis, Datadog Watchdog) remains primarily commercial territory; open-source stacks provide strong anomaly detection, root cause analysis, and agent-driven investigation foundations that require integration for complete ML-powered observability.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- ML-powered observability platforms process sensitive infrastructure and application telemetry. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **ML anomaly detection produces false positives** — tune thresholds and use consensus voting (Netdata) or predefined inspections (Coroot) to reduce noise .

- **Agent-driven investigation requires observability data access** — HolmesGPT and observability-mcp need read access to Prometheus, Loki, Kubernetes, and other backends . Ensure proper RBAC and least-privilege access.

- **License considerations**: Coroot uses Apache-2.0 , Netdata uses GPL-3.0, HolmesGPT uses MIT , observability-mcp uses Apache-2.0 , and SkyWalking uses Apache-2.0. Verify licensing against your use case before committing.

- The open-source ecosystem provides strong anomaly detection, root cause analysis, and agent-driven investigation foundations, but **topology-aware causal AI, enterprise-scale baselining, and vendor-supported SLAs** remain primarily commercial offerings.



---



**Made for SREs, DevOps engineers, and organizations seeking ML-powered observability sovereignty.**

Let's make ML-powered DevOps observability more open, transparent, and effective.
