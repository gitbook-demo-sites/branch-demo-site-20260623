---
description: How to demo adaptive content in the Branch PayAdmin section.
icon: wand-magic-sparkles
---

# Adaptive demo notes

Use these URLs after the site is published:

* Default view: no claims. The page says `You're viewing as default audience.`
* Partner view: `https://branch.gitbook.io/branch-workforce-payments-demo/nbQSAvbYkMxWs2pWTy4d/?visitor.persona=partner`
* Reset view: `https://branch.gitbook.io/branch-workforce-payments-demo/nbQSAvbYkMxWs2pWTy4d/?visitor.persona=`

## What changes

* The homepage and PayAdmin section show partner-specific guidance only when `visitor.persona=partner`.
* The default view stays ungated and says `You're viewing as default audience.`
* Partner visitors see the Uber welcome message plus integration and webhook guidance where the workflow touches API-created payouts.

{% hint style="info" icon="gitbook" %}
The default view remains complete. Adaptive content adds targeted operational detail rather than hiding the whole PayAdmin section.
{% endhint %}
