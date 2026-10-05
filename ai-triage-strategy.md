# Intelligent Triage & AI Strategy
**CJays Solutions | Zendesk Support Instance**

---

## Overview

CJays Solutions uses Zendesk AI agents and intelligent triage to automate first contact, deflect repetitive queries, and route complex issues to the right human agent. This document outlines the AI architecture, deflection strategy, and governance model.

---

## AI Agent Configuration

### Active Channels
| Channel | Status | AI Role |
|---------|--------|---------|
| Messaging (Chat) | Active | First contact, FAQ deflection, ticket creation |
| Email | Active | Auto-acknowledgement, intent detection, routing suggestion |

### What the AI Handles
- Greeting and intent capture on first contact
- Common FAQ responses (password reset, order status, return policy)
- Ticket creation when human handoff is required
- Setting customer expectations on response time

### What the AI Escalates to Human Agents
- Billing disputes and refund requests
- Account security concerns
- Complaints with high negative sentiment
- Any query the AI cannot resolve with high confidence
- Explicit customer request for a human agent

---

## Intelligent Triage

Zendesk's intelligent triage uses machine learning to automatically detect:

| Signal | What It Does |
|--------|-------------|
| **Intent** | Detects what the customer wants (refund, status update, technical help) |
| **Sentiment** | Identifies frustrated or angry customers for priority handling |
| **Language** | Detects customer language for routing to language-capable agents |

These signals are used to:
- Set ticket priority automatically (negative sentiment → High priority)
- Pre-populate the Issue Category field
- Route to the correct skill-based group without agent intervention

---

## Deflection Strategy

The goal is to resolve common, repetitive queries without human agent involvement:

1. **Help Center integration** — AI surfaces relevant articles before the customer submits a ticket
2. **FAQ bot flows** — Structured conversation flows handle top 5 query types autonomously
3. **Order status** — AI prompts customer for order number and provides status from integrated Shopify data
4. **Escalation threshold** — If AI confidence drops below acceptable level, handoff to human agent is immediate

---

## Performance Metrics

| Metric | Target |
|--------|--------|
| Automated Resolution Rate (AR) | >20% of all contacts |
| Escalation Rate | <15% of AI-handled contacts |
| First Contact Resolution (AI) | >60% of deflected contacts |
| Customer Satisfaction (AI-handled) | >4.0 / 5.0 |

---

## Governance

- AI responses are reviewed monthly for accuracy and tone
- Any AI response generating a CSAT score of 1 is flagged for review
- New FAQ flows require Admin approval before deployment
- AI agents do not handle payment processing or account deletion — these always route to human agents

---

*Last updated: October 2026*
