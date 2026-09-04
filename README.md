<div align="center">

# DAMI

### CLOUD PLATFORMS · AUTOMATION · DEVELOPER EXPERIENCE

I build the paved roads that let engineering teams move quickly without making
reliability, security, or operability somebody else’s problem.

<a href="https://github.com/dhamsey3">GitHub</a> · <a href="https://github.com/dhamsey3?tab=repositories">Projects</a>

<br>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1400&color=39D353&center=true&vCenter=true&width=760&lines=%24%20terraform%20apply;Apply%20complete.%2012%20added%2C%200%20destroyed.;%24%20kubectl%20get%20pods%20-n%20prod;web-7f9d4c%20%20%201%2F1%20%20%20Running;%24%20aws%20s3%20sync%20.%2Fdist%20s3%3A%2F%2Fprod%2F;%24%20echo%20%27shipping%20with%20confidence%27" alt="Typing SVG showing rotating DevOps terminal commands" />

</div>

<br>

```text
01  PLATFORM ENGINEERING     self-service infrastructure that scales with the team
02  CLOUD AUTOMATION          repeatable delivery, clean interfaces, fewer handoffs
03  OPERABILITY               systems that are observable before they are on fire
```

## A little context

I’m a cloud-native engineer working at the intersection of infrastructure,
software delivery, and developer enablement. My favorite work turns a fragile
manual process into a dependable system with a useful interface.

I care about:

- Infrastructure that is reproducible, secure, and easy to evolve
- Delivery systems that make the right path the easiest path
- Platform APIs and tooling that give developers useful autonomy
- Observability and incident response built into the design

## Tools I reach for

**Cloud & Infrastructure**
<p>
  <img src="https://img.shields.io/badge/AWS-161616?style=flat-square&logo=amazon-aws&logoColor=FF9900" alt="AWS" />
  <img src="https://img.shields.io/badge/Azure-161616?style=flat-square&logo=microsoft-azure&logoColor=0078D4" alt="Azure" />
  <img src="https://img.shields.io/badge/Terraform-161616?style=flat-square&logo=terraform&logoColor=7B42BC" alt="Terraform" />
  <img src="https://img.shields.io/badge/Kubernetes-161616?style=flat-square&logo=kubernetes&logoColor=326CE5" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/Docker-161616?style=flat-square&logo=docker&logoColor=2496ED" alt="Docker" />
  <img src="https://img.shields.io/badge/Ansible-161616?style=flat-square&logo=ansible&logoColor=EE0000" alt="Ansible" />
</p>

**CI/CD & Source Control**
<p>
  <img src="https://img.shields.io/badge/Jenkins-161616?style=flat-square&logo=jenkins&logoColor=D24939" alt="Jenkins" />
  <img src="https://img.shields.io/badge/GitHub_Actions-161616?style=flat-square&logo=github-actions&logoColor=2088FF" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/Git-161616?style=flat-square&logo=git&logoColor=F05032" alt="Git" />
  <img src="https://img.shields.io/badge/Bash-161616?style=flat-square&logo=gnu-bash&logoColor=4EAA25" alt="Bash" />
</p>

**Languages**
<p>
  <img src="https://img.shields.io/badge/Python-161616?style=flat-square&logo=python&logoColor=FFD343" alt="Python" />
</p>

**Observability & Incident Response**
<p>
  <img src="https://img.shields.io/badge/Splunk-161616?style=flat-square&logo=splunk&logoColor=65A637" alt="Splunk" />
  <img src="https://img.shields.io/badge/Snowflake-161616?style=flat-square&logo=snowflake&logoColor=29B5E8" alt="Snowflake" />
  <img src="https://img.shields.io/badge/PagerDuty-161616?style=flat-square&logo=pagerduty&logoColor=06AC38" alt="PagerDuty" />
</p>

## The loop I actually work in

```mermaid
flowchart TD
    Plan([Plan]) --> Code([Code])
    Code --> Build([Build])
    Build --> Test([Test])
    Test --> Release([Release])
    Release --> Deploy([Deploy])
    Deploy --> Operate([Operate])
    Operate --> Monitor([Monitor])
    Monitor -.->|feedback| Plan

    classDef stage fill:#161616,stroke:#39D353,stroke-width:1px,color:#39D353;
    class Plan,Code,Build,Test,Release,Deploy,Operate,Monitor stage;
```

## Selected builds

- **[pg-slot-sentinel](https://github.com/dhamsey3/pg-slot-sentinel)** — Monitors Postgres replication slots for orphaned WAL retention before it fills RDS storage. Ships with a docker-compose demo that reproduces the failure mode end to end.
- **[PipelineForge](https://github.com/dhamsey3/pipelineforge-aws-devops-platform)** — An AWS-native delivery platform with CodePipeline, CodeBuild, ECR, and ECS Fargate.
- **[Distributed Load Testing](https://github.com/dhamsey3/distributed-load-testing)** — Distributed performance testing for understanding how systems behave under load.
- **[Internal Developer Platform API](https://github.com/dhamsey3/internal-developer-platform-api)** — A repeatable API for provisioning infrastructure and supporting Kubernetes deployments.
- **[OpenStreetMap on AWS](https://github.com/dhamsey3/openstreetmap-aws-cloud-deployment)** — Terraform, ECS/Fargate, RDS, and CI/CD assembled as a production-style deployment.
- **[ELK SIEM Sandbox](https://github.com/dhamsey3/siem-sandbox-elk)** — A Docker lab for log analysis, detection engineering, and security experiments.
- **[Automation with Python](https://github.com/dhamsey3/Automation-with-Python)** — Small operational tools that remove repetitive work and sharpen daily workflows.

## The pipeline that eats its own output

Regenerated nightly by a scheduled GitHub Action that walks my contribution
graph — the same automation habit, pointed at a README instead of a
production system.

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dhamsey3/dhamsey3/output/github-contribution-grid-snake-dark.svg" />
  <img alt="a snake animation eating the GitHub contribution graph" src="https://raw.githubusercontent.com/dhamsey3/dhamsey3/output/github-contribution-grid-snake.svg" />
</picture>

</div>

## Current direction

```text
cloud infrastructure  /  internal platforms  /  delivery automation
security-minded ops    /  useful abstractions  /  fewer manual rituals
```

<div align="center">

<sub>Build systems people can trust. Keep learning in public.</sub>

</div>
