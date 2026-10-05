# User Roles & Permissions
**CJays Solutions | Zendesk Support Instance**

---

## Overview

Zendesk uses a role-based access model. This document defines the roles in use at CJays Solutions, their permissions, and when each role is assigned.

---

## Role Definitions

### Administrator
**Who:** Support Operations Manager, Zendesk instance owner  
**Access:** Full access to all Zendesk configuration — triggers, automations, SLA policies, groups, channels, integrations, billing  
**Restrictions:** None  
**Assigned to:** Clement Okeniyi

---

### Agent
**Who:** Front-line support staff  
**Access:**
- View and respond to tickets in their assigned group
- Apply macros and tags
- Access Help Center (read)
- View their own CSAT scores

**Restrictions:**
- Cannot access Admin settings
- Cannot view other agents' tickets outside their group
- Cannot modify triggers, automations, or SLA policies

---

### Light Agent
**Who:** Internal stakeholders (sales, finance, operations) who need ticket visibility  
**Access:**
- View tickets (read-only)
- Add internal notes
- Cannot send public replies

**Use case:** Finance team monitoring billing tickets. Operations team tracking order-related issues.

---

### End User (Customer)
**Who:** External customers submitting support requests  
**Access:**
- Submit tickets via email, chat, or Help Center
- View and reply to their own tickets only
- Access Help Center articles

---

## Group Membership

| Group | Members | Ticket Types |
|-------|---------|-------------|
| Billing Support | Billing agents | Billing, refunds, payment issues |
| Technical Support | Technical agents | Access, bugs, technical errors |
| General Support | General agents | Inquiries, feature requests, other |

---

## Permission Governance

- Role changes require Admin approval
- New agents are onboarded as Agent role only after completing SOP-03
- Light Agent access is reviewed quarterly — unused accounts are deactivated
- Admin credentials are not shared — each admin has individual login

---

*Last updated: October 2026*
