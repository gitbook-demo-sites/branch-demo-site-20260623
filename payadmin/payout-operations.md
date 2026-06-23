---
description: Triage and resolve employer-side payout exceptions in PayAdmin.
icon: triangle-exclamation
---

# Payout operations

Use this runbook when a worker reports a missing paycheck, tip, mileage payout, advance issue, instant transfer delay, or payout reversal.

{% tabs %}
{% tab title="Missing payout" %}
1. Search the worker by phone, email, external worker ID, or employer ID.
2. Check the expected pay date, funding state, and payout method.
3. Confirm whether the payout was pending, sent, returned, cancelled, or blocked.
4. Add the support case reference before changing anything.
{% endtab %}

{% tab title="Delayed transfer" %}
1. Check transfer rail and destination status.
2. Review bank holiday and cutoff time warnings.
3. Confirm whether debit-card instant transfer or ACH timing applies.
4. Provide the worker-facing ETA and next action.
{% endtab %}

{% tab title="Failed payout" %}
1. Review failure reason and retry eligibility.
2. Confirm whether worker account details need updating.
3. Decide whether to retry, reroute, or escalate.
4. Record the operational decision in the case timeline.
{% endtab %}
{% endtabs %}

{% if visitor.claims.persona === "payadmin" %}
{% hint style="warning" icon="lock" %}
**Admin-only checklist**

Before reissuing funds, check duplicate payout risk, funding balance, previous retries, worker identity confidence, and whether the employer has approval requirements enabled.
{% endhint %}
{% endif %}

{% if visitor.claims.persona === "partner" %}
{% hint style="info" icon="webhook" %}
**Partner integration note**

If the payout was created through the API, compare PayAdmin status with the `payout.updated` webhook delivery log before telling the partner to retry.
{% endhint %}
{% endif %}
