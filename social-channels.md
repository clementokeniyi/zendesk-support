# Social Messaging Channels
**CJays Solutions | Zendesk Support Instance**

---

## Overview

Zendesk Messaging enables support teams to manage customer conversations from social and messaging platforms directly inside the Zendesk agent workspace. This document outlines the social channel strategy for CJays Solutions.

---

## Channels in Scope

### WhatsApp Business
**Status:** Planned  
**Integration method:** Zendesk Messaging via WhatsApp Business API  
**Setup requirements:**
- WhatsApp Business Account (verified)
- Facebook Business Manager access
- Zendesk Messaging enabled on the instance

**How it works:**
- Customer sends a WhatsApp message to the CJays Solutions business number
- Message appears as a ticket in Zendesk with channel type: WhatsApp
- Agent responds from Zendesk — reply delivers to customer's WhatsApp
- Full conversation history stored in the ticket

**Use cases:** Order status queries, shipping updates, quick resolution of simple issues

---

### Instagram Direct Messages
**Status:** Planned  
**Integration method:** Zendesk Messaging via Meta Business Suite  
**Setup requirements:**
- Instagram Business Account connected to Facebook Page
- Zendesk Social Messaging integration enabled

**How it works:**
- Customer sends an Instagram DM to the CJays Solutions account
- DM routes into Zendesk as a new ticket
- Agent responds from Zendesk — reply appears in customer's Instagram DMs
- Conversations are tracked and reportable in Explore

**Use cases:** Brand mentions, product enquiries, complaint handling from social

---

## Agent Workspace Configuration

When social channels are active:
- All channels (email, chat, WhatsApp, Instagram) appear in the unified agent workspace
- Channel type is visible on every ticket — agents can see at a glance how the customer contacted
- Routing triggers can be configured to assign social tickets to a dedicated social support group
- SLA policy applies to social tickets the same as email

---

## Governance

- Social channels are monitored during business hours only (09:00–18:00)
- Outside hours: AI agent handles first contact and sets expectation for next-day response
- Agents do not share personal contact details on social channels — all communication stays within Zendesk
- Screenshots of sensitive conversations must not be shared externally

---

*Last updated: October 2026*
