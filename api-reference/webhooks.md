---
description: Subscribe to payout, transfer, card, and dispute events.
icon: webhook
---

# Webhooks

Branch sends webhook events when payout and worker states change.

```mermaid
sequenceDiagram
    participant Partner
    participant Branch
    participant Worker
    Partner->>Branch: POST /payouts
    Branch->>Worker: Funds available through Branch
    Branch-->>Partner: payout.created
    Branch-->>Partner: payout.settled
```

## Recommended subscriptions

| Event | Use when |
| --- | --- |
| `payout.created` | A payout request is accepted. |
| `payout.failed` | A payout needs retry or operator review. |
| `payout.settled` | Funds are available or settled. |
| `dispute.opened` | A transaction dispute was created. |

{% hint style="warning" icon="shield-check" %}
Validate webhook signatures and retry delivery with exponential backoff.
{% endhint %}
