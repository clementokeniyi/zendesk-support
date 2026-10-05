# Tagging Taxonomy
**CJays Solutions | Zendesk Support Instance**

---

## Overview

Tags in Zendesk are used to drive reporting, trigger conditions, and workflow logic. This document defines all tags in use, their purpose, and where they are applied.

---

## Tag Reference

| Tag | Applied By | Purpose |
|-----|-----------|---------|
| `billing` | Routing trigger | Identifies billing-related tickets for group assignment |
| `technical` | Routing trigger | Identifies technical tickets for group assignment |
| `general` | Routing trigger | Identifies general enquiries for group assignment |
| `escalated` | Agent (manual) | Flags ticket as escalated — triggers senior agent assignment |
| `escalation-resolved` | Senior agent (manual) | Marks escalated ticket as resolved — used in weekly review |
| `vip` | Agent (manual) | High-value customer — prioritize response |
| `refund-requested` | Agent (manual) | Customer has requested a refund — flags for billing review |
| `follow-up-sent` | Automation | Applied when 48hr follow-up message is sent |
| `pending-close` | Automation | Applied before auto-close — for audit trail |
| `csat-low` | Agent (manual) | Applied when CSAT score of 1 or 2 received |
| `first-contact` | Trigger | Applied on ticket creation — tracks new contacts |
| `api-created` | API/Integration | Applied to tickets created via REST API or integration |

---

## Tagging Rules

1. **Never apply conflicting category tags** — a ticket should have only one of: `billing`, `technical`, `general`
2. **Escalation tags must be paired** — `escalated` must always be followed by `escalation-resolved` once closed
3. **`vip` tag is permanent** — once applied, do not remove even after resolution
4. **Automation tags are system-managed** — do not manually remove `follow-up-sent` or `pending-close`

---

## Reporting Use

The following tags are used as filters in Explore dashboards:
- `escalated` — tracks escalation rate over time
- `csat-low` — tracks dissatisfaction trends
- `billing`, `technical`, `general` — tracks volume by team

---

*Last updated: October 2026*
