---
description: PayAdmin operations for Branch workforce payments, employer support, payout review, and exception workflows.
icon: user-gear
---

# PayAdmin

PayAdmin is the employer and operations workspace for reviewing worker payouts, resolving payment exceptions, managing workforce payment settings, and coordinating support handoffs.

{% if visitor.claims.unsigned.persona === "payadmin" %}
{% hint style="success" icon="user-gear" %}
**Admin mode enabled.** This view adds operational runbooks, exception handling, funding status, audit trails, and role-based access guidance.
{% endhint %}
{% endif %}

{% if visitor.claims.unsigned.persona === "partner" %}
{% hint style="info" icon="handshake-angle" %}
**Partner mode enabled.** This view emphasizes integration handoffs, API-created payouts, webhook events, and platform support boundaries.
{% endhint %}
{% endif %}

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody>
<tr><td><h3><i class="fa-triangle-exclamation" style="color:$primary;">:triangle-exclamation:</i></h3></td><td><strong>Payout operations</strong></td><td>Triage missing pay, delayed deposits, failed transfers, and holiday timing.</td><td><a href="payout-operations.md">payout operations</a></td></tr>
<tr><td><h3><i class="fa-headset" style="color:$primary;">:headset:</i></h3></td><td><strong>Worker support review</strong></td><td>Move from public help-center issue to employer-side investigation.</td><td><a href="worker-support-review.md">worker support review</a></td></tr>
<tr><td><h3><i class="fa-shield-check" style="color:$primary;">:shield-check:</i></h3></td><td><strong>Access and controls</strong></td><td>Roles, permissions, audit history, approvals, and compliance boundaries.</td><td><a href="access-and-controls.md">access and controls</a></td></tr>
</tbody></table>

## Daily operating loop

{% stepper %}
{% step %}
### Review exception queues
Check failed payout attempts, missing worker details, funding holds, returned transfers, and unresolved direct deposit questions.
{% endstep %}

{% step %}
### Confirm worker and employer context
Validate the worker identity, employer location, payroll cycle, payment method, and whether the case started in app support.
{% endstep %}

{% step %}
### Resolve or escalate
Resolve simple data issues in PayAdmin. Escalate compliance, dispute, fraud, or bank-partner dependent cases with the supporting evidence attached.
{% endstep %}
{% endstepper %}
