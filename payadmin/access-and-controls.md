---
description: Roles, permissions, audit history, and compliance controls for PayAdmin.
icon: shield-check
---

# Access and controls

PayAdmin access should follow least privilege. Operators should have only the permissions needed for worker lookup, payout review, funding visibility, approvals, or admin configuration.

| Role | Typical access | Example tasks |
| --- | --- | --- |
| Support reviewer | Read-only worker and payout status | Confirm status, add notes, route cases |
| Payroll operator | Payout operations and retry actions | Review missing pay, retry eligible payouts |
| Finance admin | Funding and settlement visibility | Monitor funding state, reconcile batches |
| Compliance admin | Restricted review and audit | Fraud, dispute, and policy escalations |

{% if visitor.claims.unsigned.persona === "payadmin" %}
{% hint style="warning" icon="shield-halved" %}
**Admin-only control**

Require a second approval for payout reissue, destination-account changes, or actions that could create duplicate disbursement risk.
{% endhint %}
{% endif %}

## Audit trail

Every operational action should preserve who changed what, when it changed, why it changed, and which support or payroll case justified the action.
