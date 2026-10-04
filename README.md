# AI Sales Prep Copilot

> From a prospect's name to a meeting brief and follow-up draft in two minutes.

![status](https://img.shields.io/badge/status-design%20stage-lightgrey) ![sprint](https://img.shields.io/badge/sprint-Weeks%209--10-blue) ![project](https://img.shields.io/badge/portfolio-05%2F08-0891b2)

| | |
|---|---|
| **Category** | AI Agents & Automation |
| **Domain** | B2B Sales |
| **Stack** | Python · LLM agents · n8n · CRM API |
| **Status** | 🚧 Scoped — implementation not started |

## Overview

An agent that does a salesperson's homework: researches the prospect company, enriches the data, identifies likely pain points, writes a meeting brief, and drafts the follow-up email. n8n orchestrates the workflow and nothing is sent externally without human approval.

## Business problem

Sales teams spend hours on prospect research, meeting prep, note-taking and follow-up writing instead of selling.

## What this project demonstrates

- Agentic workflows orchestrated with n8n
- Tool use and data enrichment
- Governance: no external action without human approval
- Measuring automation value as time saved

## Key points

- n8n workflow triggered by a webhook or a new CRM lead
- Agent tools: company research, data enrichment, summarisation, pain-point analysis
- Standardised one-page meeting brief template
- Follow-up email drafts with an approve / edit / reject step
- Governance rule: AI generates → human reviews → human approves → system executes
- KPIs: prep time saved per meeting, prospects processed, approval rate, workflow success rate

## Planned architecture

```text
New lead / webhook
   ↓
n8n workflow
   ↓
Research & enrichment agent
   ↓
Pain-point analysis → meeting brief
   ↓
Human approval
   ↓
Follow-up draft → CRM update / notification
```

## Planned deliverables

- [ ] Agent with research, enrichment and summarisation tools
- [ ] n8n workflow (exported JSON)
- [ ] Meeting brief template
- [ ] Follow-up generator with approval step
- [ ] Demo video
- [ ] ROI estimate and architecture diagram

## Success metrics

- Prep time saved per meeting
- Prospects processed
- Human approval rate
- Workflow success rate

## Planned structure

```text
src/agent/  n8n/  templates/  docs/
```

## Roadmap

- [x] Scope and README
- [ ] Data collection / generation
- [ ] Core implementation
- [ ] Evaluation and business-impact estimate
- [ ] Demo, write-up and interview notes

---

Part of my **Data & AI × Business Consulting** portfolio, a 16-week sprint of 8 projects going from data and BI to ML, GenAI, agents, automation and AI strategy. See all projects on my [GitHub profile](https://github.com/Amine-Charrou).

*Amine Charrou · Final-year Data Science & AI engineering student, ENSA Agadir · [LinkedIn](https://www.linkedin.com/in/amine-charrou/)*
