---
description: Move a worker-facing support issue into PayAdmin without losing context.
icon: headset
---

# Worker support review

Worker support usually starts in the Branch app or help center. PayAdmin adds employer-side context when the issue depends on payroll setup, payout timing, or workforce records.

```mermaid
sequenceDiagram
    participant Worker
    participant Support as Branch Support
    participant PayAdmin
    participant Payroll as Employer payroll
    Worker->>Support: Reports missing pay or account issue
    Support->>PayAdmin: Opens employer-side review
    PayAdmin->>Payroll: Checks pay cycle, worker record, funding
    PayAdmin-->>Support: Adds resolution or escalation note
    Support-->>Worker: Sends worker-facing update
```

## Review questions

* Is the worker's Branch account active and matched to the right employer?
* Is the payout expected, sent, pending, returned, cancelled, or blocked?
* Is there a known bank holiday, cutoff, funding, or employer-file delay?
* Is the support response worker-facing, employer-facing, or both?

{% if visitor.claims.persona === "payadmin" %}
{% hint style="success" icon="clipboard-check" %}
**Suggested PayAdmin response**

Attach the payout ID, employer ID, worker external ID, status reason, funding state, next action, and confidence level before handing back to support.
{% endhint %}
{% endif %}
