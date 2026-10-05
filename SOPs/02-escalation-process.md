# SOP: Escalation Process
**CJays Solutions Support Operations**

## Purpose
Define when and how tickets are escalated to senior agents or management.

## Escalation Triggers
Escalate a ticket when ANY of the following apply:
- Issue cannot be resolved within one business day
- Customer has replied 3+ times without resolution
- Customer explicitly requests a manager
- Issue involves a potential refund over $500
- Data loss, security concern, or account compromise suspected
- CSAT score of 1 received and customer is still unhappy

## Escalation Steps

### Step 1 — Flag the Ticket
- Add tag: `escalated`
- Add internal note explaining: what was tried, why it needs escalation, customer sentiment

### Step 2 — Reassign
- Change assignee to senior agent or Team Lead
- Change ticket priority to High or Urgent

### Step 3 — Notify
- Send customer a message: "I've escalated your case to a senior member of our team who will follow up within [X] hours."
- Ping the senior agent directly via internal comment

### Step 4 — Senior Agent Takes Over
- Senior agent reviews the full ticket thread and internal notes
- Responds to customer within 2 business hours
- Documents resolution in internal note for team learning

### Step 5 — Close & Review
- After resolution, senior agent adds tag: `escalation-resolved`
- Team Lead reviews escalated tickets weekly to identify patterns
