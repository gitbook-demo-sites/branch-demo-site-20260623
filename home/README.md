---
description: Fast payments, workforce wallets, PayAdmin operations, and partner APIs in one Branch documentation experience.
icon: house
layout:
  width: wide
  cover:
    visible: false
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: false
  pagination:
    visible: false
---

# Welcome to Branch

{% columns %}
{% column width="50%" %}
Branch delivers faster, more flexible options for businesses to pay their workers, support instant access to earnings, and manage workforce payments across apps, cards, direct deposits, tips, mileage, and partner workflows.

<button type="button" class="button primary" data-action="ask" data-icon="gitbook-assistant">Ask the Branch docs</button>

<button type="button" class="button secondary" data-action="ask" data-query="How do I help a worker with a missing payout?" data-icon="circle-dollar-to-slot">Missing payout</button> <button type="button" class="button secondary" data-action="ask" data-query="How should a PayAdmin user review a payout issue?" data-icon="user-gear">PayAdmin</button> <button type="button" class="button secondary" data-action="ask" data-query="How do I create a payout through the API?" data-icon="code">API</button>
{% endcolumn %}

{% column width="50%" %}
{% hint style="success" icon="gitbook" %}
**Demo experience**

This Branch demo uses the public support portal as the customer-help source, adds a PayAdmin operator section, and includes an OpenAPI-backed dummy API reference for partner and embedded-finance conversations.

{% if !visitor.claims.unsigned.persona %}
<i class="fa-users" style="color:$info;">:users:</i> You're viewing as default audience.

Switch to the partner view to see adaptive content in PayAdmin:

<a href="https://branch.gitbook.io/branch-workforce-payments-demo/nbQSAvbYkMxWs2pWTy4d/?visitor.persona=partner" class="button secondary" data-icon="handshake-angle">Partner</a>
{% endif %}

{% if visitor.claims.unsigned.persona %}
<i class="fa-id-card-clip" style="color:$info;">:id-card-clip:</i> You are viewing as <code class="expression">visitor.claims.unsigned.persona</code>. [<mark style="color:$primary;">Reset</mark>](https://branch.gitbook.io/branch-workforce-payments-demo/nbQSAvbYkMxWs2pWTy4d/)
{% endif %}
{% endhint %}
{% endcolumn %}
{% endcolumns %}

{% if visitor.claims.unsigned.persona %}

***

## <i class="fa-sparkle" style="color:$info;">:sparkle:</i> Picked for you

{% endif %}

{% if visitor.claims.unsigned.persona === "worker" %}
{% hint style="info" icon="mobile-screen-button" %}
**Worker view.** Start with account access, card actions, direct deposit, transfers, advances, and dispute support.
{% endhint %}

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody>
<tr><td><h4><i class="fa-right-to-bracket" style="color:$primary;">:right-to-bracket:</i></h4></td><td><h4><strong>Account setup</strong></h4></td><td>Sign up, login, passcodes, phone changes, and account maintenance.</td><td><a href="https://app.gitbook.com/s/IDJQAVl8qYTXytlalrU6/">account setup</a></td></tr>
<tr><td><h4><i class="fa-money-bill-transfer" style="color:$primary;">:money-bill-transfer:</i></h4></td><td><h4><strong>Direct deposits</strong></h4></td><td>Set up direct deposit and understand paycheck, tip, and mileage timing.</td><td><a href="https://app.gitbook.com/s/IDJQAVl8qYTXytlalrU6/">direct deposits</a></td></tr>
<tr><td><h4><i class="fa-scale-balanced" style="color:$primary;">:scale-balanced:</i></h4></td><td><h4><strong>Disputes</strong></h4></td><td>When to file a dispute and what evidence helps the review process.</td><td><a href="https://app.gitbook.com/s/IDJQAVl8qYTXytlalrU6/">disputes</a></td></tr>
</tbody></table>
{% endif %}

{% if visitor.claims.unsigned.persona === "payadmin" %}
{% hint style="info" icon="user-gear" %}
**PayAdmin view.** Prioritize payout exceptions, worker lookup, funding status, compliance review, and support handoffs.
{% endhint %}

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody>
<tr><td><h4><i class="fa-gauge-high" style="color:$primary;">:gauge-high:</i></h4></td><td><h4><strong>PayAdmin overview</strong></h4></td><td>Understand the workspace, roles, and daily operating rhythm.</td><td><a href="https://app.gitbook.com/s/ksPiMtClGKP4tXIPmW2O/">payadmin</a></td></tr>
<tr><td><h4><i class="fa-triangle-exclamation" style="color:$primary;">:triangle-exclamation:</i></h4></td><td><h4><strong>Resolve payout exceptions</strong></h4></td><td>Triage missing payouts, failed transfers, holidays, and worker-impacting issues.</td><td><a href="https://app.gitbook.com/s/ksPiMtClGKP4tXIPmW2O/payout-operations">payout operations</a></td></tr>
<tr><td><h4><i class="fa-shield-check" style="color:$primary;">:shield-check:</i></h4></td><td><h4><strong>Admin access</strong></h4></td><td>Role-based permissions, audit history, and compliance-aware escalation.</td><td><a href="https://app.gitbook.com/s/ksPiMtClGKP4tXIPmW2O/access-and-controls">access controls</a></td></tr>
</tbody></table>
{% endif %}

{% if visitor.claims.unsigned.persona === "partner" %}
{% hint style="info" icon="handshake-angle" %}
**Partner view.** Focus on embedded payouts, onboarding, API credentials, webhooks, and exception callbacks.
{% endhint %}

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody>
<tr><td><h4><i class="fa-code" style="color:$primary;">:code:</i></h4></td><td><h4><strong>API reference</strong></h4></td><td>Dummy OpenAPI spec for payouts, workers, transfers, and webhooks.</td><td><a href="https://app.gitbook.com/s/B6kpkf125bYXSptQOGAX/">api</a></td></tr>
<tr><td><h4><i class="fa-key" style="color:$primary;">:key:</i></h4></td><td><h4><strong>Authentication</strong></h4></td><td>Sandbox credentials, idempotency, and partner integration keys.</td><td><a href="https://app.gitbook.com/s/B6kpkf125bYXSptQOGAX/authentication">authentication</a></td></tr>
<tr><td><h4><i class="fa-webhook" style="color:$primary;">:webhook:</i></h4></td><td><h4><strong>Webhooks</strong></h4></td><td>Subscribe to payout, card, worker, and dispute events.</td><td><a href="https://app.gitbook.com/s/B6kpkf125bYXSptQOGAX/webhooks">webhooks</a></td></tr>
</tbody></table>
{% endif %}

***

## Explore the docs

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody>
<tr><td><h3><i class="fa-life-ring" style="color:$primary;">:life-ring:</i></h3></td><td><strong>Support Center</strong></td><td>Worker-facing help center content reorganized for Branch app, card, deposit, transfer, advance, and dispute questions.</td><td><a href="https://app.gitbook.com/s/IDJQAVl8qYTXytlalrU6/">support</a></td></tr>
<tr><td><h3><i class="fa-user-gear" style="color:$primary;">:user-gear:</i></h3></td><td><strong>PayAdmin</strong></td><td>Admin operations for payout review, workforce support, roles, and escalation workflows.</td><td><a href="https://app.gitbook.com/s/ksPiMtClGKP4tXIPmW2O/">payadmin</a></td></tr>
<tr><td><h3><i class="fa-code" style="color:$primary;">:code:</i></h3></td><td><strong>API Reference</strong></td><td>OpenAPI-backed partner API reference with payout, worker, transfer, and webhook examples.</td><td><a href="https://app.gitbook.com/s/B6kpkf125bYXSptQOGAX/">api</a></td></tr>
</tbody></table>

## Common journeys

{% stepper %}
{% step %}
### Help a worker find their money
Start in **Support Center** with direct deposits, tips and mileage, transfers, and pending transactions. Move into **PayAdmin** when the case needs account lookup, payout status, or an employer-side review.
{% endstep %}

{% step %}
### Launch an employer payout workflow
Use **PayAdmin** to set roles, validate funding, review exception queues, and coordinate support. Use the API reference when a platform or marketplace wants to automate the same flow.
{% endstep %}

{% step %}
### Demo adaptive content
Open the PayAdmin persona URL and compare it to the default view. The same pages reveal admin-specific guidance without duplicating the entire support center.
{% endstep %}
{% endstepper %}
