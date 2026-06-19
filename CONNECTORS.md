---
version: 2
plugin: campaign-copy-generator
last_updated: 2026-04-01
status: active
purpose: connector_registry
---

# Connectors

This file defines the connector placeholders used by `campaign-copy-generator`.

Use the placeholder that best matches the source material you need. If the best connector is unavailable, continue with uploaded briefs, pasted notes, exports, or approved source links instead of blocking.

## Placeholder Map

### `[[docs]]`

```yaml
category: docs
display_name: Docs
output_label: Docs
allowed_connectors:
  - google_drive
  - notion
default_connector: google_drive
capabilities:
  - search
  - read
  - write
```

### `[[crm]]`

```yaml
category: crm
display_name: CRM
output_label: CRM
allowed_connectors:
  - hubspot
  - salesforce
default_connector: hubspot
capabilities:
  - search
  - read
```

### `[[chat]]`

```yaml
category: chat
display_name: Team Chat
output_label: Chat
allowed_connectors:
  - slack
  - teams
default_connector: slack
capabilities:
  - search
  - read
```

### `[[design]]`

```yaml
category: design
display_name: Design
output_label: Design
allowed_connectors:
  - canva
  - figma
  - adobe_express
  - adobe_photoshop
  - adobe_acrobat
default_connector: figma
capabilities:
  - search
  - read
```

### `[[email]]`

```yaml
category: email
display_name: Email
output_label: Email
allowed_connectors:
  - gmail
  - outlook_email
default_connector: gmail
capabilities:
  - search
  - read
```

### `[[calendar]]`

```yaml
category: calendar
display_name: Calendar
output_label: Calendar
allowed_connectors:
  - google_calendar
  - outlook_calendar
default_connector: google_calendar
capabilities:
  - search
  - read
```

### `[[email_marketing]]`

```yaml
category: email_marketing
display_name: Email Marketing
output_label: Email Marketing
allowed_connectors:
  - hubspot
  - mailchimp
  - customer_io
  - klaviyo
default_connector: hubspot
capabilities:
  - search
  - read
  - write
```

### `[[marketing_automation]]`

```yaml
category: marketing_automation
display_name: Marketing Automation
output_label: Marketing Automation
allowed_connectors:
  - hubspot
  - marketo
default_connector: hubspot
capabilities:
  - search
  - read
  - write
```

### `[[marketing_analytics]]`

```yaml
category: marketing_analytics
display_name: Marketing Analytics
output_label: Marketing Analytics
allowed_connectors:
  - amplitude
  - google_analytics
default_connector: amplitude
capabilities:
  - search
  - read
```

## Fallback Rules

- Treat attached apps as an evidence accelerator, not a requirement.
- Prefer campaign briefs, brand guides, approved examples, and performance readouts over generic filler.
- If connector results conflict with uploaded materials, surface the mismatch instead of silently blending them.
- `business-context.md` should point to durable source material; it should not replace stronger request-scoped instructions.
