# Hi, I'm Dami

**Cloud & DevOps Engineer** working on AWS and Azure: infrastructure as code, CI/CD pipelines and internal developer platforms.

I build systems that run unattended, raise an alarm when they break and keep a record of what they did. Teams ship faster when reliability, security and operability are built in from the start, not left as someone else's problem.

**Now:** running [voltcast](https://github.com/dhamsey3/voltcast) live on AWS. Next up: deploys from CI over OIDC and a public status page.

## Featured: [voltcast](https://github.com/dhamsey3/voltcast)

A live forecasting service. Every morning it forecasts tomorrow's German/Luxembourg day-ahead electricity price for all 96 quarter-hours, publishes before the 12:00 auction closes and grades itself against the cleared prices that afternoon.

- **Runs unattended** on EventBridge Scheduler, Step Functions and one Lambda, all in Terraform, for an estimated 2 USD a month.
- **Says when it breaks**: alarms for a missed deadline or a failed run, a runbook for each alarm and an incident log.
- **Refuses bad data**: a data contract stops the run when upstream prices look wrong, and every forecast records the code version and a hash of every input it read.

## More projects

- **[pg-slot-sentinel](https://github.com/dhamsey3/pg-slot-sentinel)**: catches a quiet way Postgres runs out of disk, a replication slot nobody reads any more, and pages before the retained WAL fills RDS storage. A docker-compose demo reproduces the failure end to end.<br>
  `Python` `Lambda` `Terraform` `CloudWatch`
- **[Klausel](https://github.com/dhamsey3/klausel)**: a self-hosted, GDPR-compliant contract reviewer for German legal text. It redacts personal data, splits documents by § and answers questions with cited sources, using local embeddings and a local LLM. No cloud APIs at runtime.<br>
  `Python` `Qdrant` `Ollama` `ZenML` `MinIO`
- **[Distributed Load Testing](https://github.com/dhamsey3/distributed-load-testing)**: a Terraform module that fans one k6 script out across parallel Fargate tasks and collects the results in S3. A lean take on AWS's reference solution.<br>
  `Terraform` `ECS Fargate` `Step Functions` `k6`
- **[Internal Developer Platform API](https://github.com/dhamsey3/internal-developer-platform-api)**: a self-service API that lets developers provision EKS environments. GitHub Actions runs Terraform with separate plan and apply roles over OIDC, and nothing is applied without an approval.<br>
  `Python` `FastAPI` `Terraform` `EKS` `Helm`
- **[OpenStreetMap on AWS](https://github.com/dhamsey3/openstreetmap-aws-cloud-deployment)**: the OpenStreetMap website on ECS Fargate and RDS Postgres, deployed with Terraform through GitHub Actions OIDC across dev, acceptance and production.<br>
  `Terraform` `ECS Fargate` `RDS` `Ansible`

Also: [PipelineForge](https://github.com/dhamsey3/pipelineforge-aws-devops-platform) (CodePipeline to ECS Fargate), [ELK SIEM sandbox](https://github.com/dhamsey3/siem-sandbox-elk), [Python automation](https://github.com/dhamsey3/automation-with-python).

## How I work

- **Infrastructure is code.** Every AWS project above is built with Terraform, so it can be reproduced, reviewed and torn down.
- **No long-lived keys.** Where CI deploys to AWS, it signs in through OIDC with short-lived credentials, not stored access keys.
- **The safe path is the easy path.** Developers get self-service, with guardrails such as separate plan and apply steps and approvals built in.
- **Operability is part of the design.** Alarms, runbooks and incident write-ups ship with the first release, not after the first outage.

## Tools

| Area | Tools |
|---|---|
| Cloud | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white) |
| Infrastructure as code | ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white) ![CloudFormation](https://img.shields.io/badge/CloudFormation-FF4F8B?style=flat-square&logo=amazon-aws&logoColor=white) ![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white) |
| Containers | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) |
| CI/CD | ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white) ![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white) ![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white) |
| Observability & on-call | ![Elastic](https://img.shields.io/badge/Elastic-005571?style=flat-square&logo=elastic&logoColor=white) ![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white) ![PagerDuty](https://img.shields.io/badge/PagerDuty-06AC38?style=flat-square&logo=pagerduty&logoColor=white) |
| Languages & data | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) |
