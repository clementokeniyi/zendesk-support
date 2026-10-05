# SOP: Change Management Process
**CJays Solutions Support Operations**

## Purpose
Ensure that changes to Zendesk configuration (triggers, macros, views, SLA, routing) are made safely without disrupting live support operations.

## Scope
Any change to: triggers, automations, macros, views, SLA policies, ticket forms, groups, or integrations.

## Change Categories

| Category | Examples | Approval Required |
|----------|----------|-------------------|
| Minor | Edit macro wording, rename a view | Agent self-service |
| Standard | New trigger, new SLA rule, new view | Team Lead approval |
| Major | New integration, routing overhaul, new ticket form | Admin approval + testing |

## Process

### Step 1 — Document the Change
- Write down: what is changing, why, expected impact, rollback plan

### Step 2 — Get Approval
- Minor: no approval needed, document in changelog
- Standard/Major: post in team Slack or email for approval before making change

### Step 3 — Test First
- Make the change in a test ticket or off-peak hours
- Verify the trigger/automation fires correctly on a sample ticket

### Step 4 — Deploy
- Make the change in Zendesk admin panel
- Monitor for 30 minutes to catch unexpected behavior

### Step 5 — Document
- Add an entry to the team changelog:
  `[Date] | [What changed] | [Who made it] | [Why]`

## Rollback
- Zendesk does not have native rollback — before major changes, screenshot current settings
- To revert: manually restore previous settings using the screenshot as reference
