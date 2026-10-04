# AI Sales Prep Copilot

> From a prospect's name to a meeting brief and follow-up draft in two minutes.

![status](https://img.shields.io/badge/status-planned-lightgrey) ![phase](https://img.shields.io/badge/sprint-Weeks%209--10-blue)

**Category:** AI Agents & Automation · **Domain:** B2B Sales · **Stack:** Python · LLM agents · n8n · CRM API

Project 05/08 of my *Data & AI × Business Consulting* portfolio. 🚧 **Design stage, no implementation yet.**

## Overview

An agent that does a salesperson's homework: researches the prospect company, enriches the data, identifies likely pain points, writes a meeting brief, and drafts the follow-up email. n8n orchestrates the workflow and nothing is sent externally without human approval.

## Business problem

Sales teams spend hours on prospect research, meeting prep, note-taking and follow-up writing instead of selling.

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

## Status

- [x] Scope and README
- [ ] Data
- [ ] Implementation
- [ ] Evaluation & business impact
- [ ] Demo and write-up

---

*Author: Amine Charrou · Final-year Data Science & AI engineering student, ENSA Agadir*
