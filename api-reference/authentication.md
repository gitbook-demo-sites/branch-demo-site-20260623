---
description: Sandbox credentials, bearer tokens, idempotency keys, and API-version headers.
icon: key
---

# Authentication

Branch partner APIs use bearer tokens scoped to a partner workspace and environment.

{% tabs %}
{% tab title="cURL" %}
```bash
curl https://sandbox.api.branchapp.example/v1/payouts \
  -H "Authorization: Bearer $BRANCH_API_KEY" \
  -H "Idempotency-Key: payout-demo-001" \
  -H "Branch-Version: 2026-06-01"
```
{% endtab %}

{% tab title="Node" %}
```js
const res = await fetch('https://sandbox.api.branchapp.example/v1/payouts', {
  headers: {
    Authorization: `Bearer ${process.env.BRANCH_API_KEY}`,
    'Idempotency-Key': 'payout-demo-001',
    'Branch-Version': '2026-06-01'
  }
});
```
{% endtab %}
{% endtabs %}

{% hint style="info" icon="rotate" %}
Use idempotency keys for payout creation so retries do not create duplicate disbursements.
{% endhint %}
