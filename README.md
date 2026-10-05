# SRE Copilot Fleet

Autonomous incident-response fleet on GKE — agentic AI (LangGraph) + GitOps remediation.

A full-stack demo app (React → FastAPI → Postgres) running on GKE, monitored by
detector bots that emit incidents, with a LangGraph agent that diagnoses issues
and remediates by opening pull requests against this GitOps repo. Argo CD is the
only writer to the cluster; every fix is an auditable commit.

Status: **Week 1 — foundation (cluster + GitOps + app)**
