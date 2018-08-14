---
description: FlashFX Developer API documentation
---

# FlashFX API documentation

## General information

FlashFX API is [GraphQL](http://graphql.github.io/learn/queries/) based. It's easier than RESTful and quite developer friendly.

FlashFX API playground is located here: [https://api.flash-fx.com/](https://api.flash-fx.com/)

## Quick start

{% hint style="warning" %}
#### Warning - BETA

The API is in the **beta** stage right now. We are planning to do few breaking changes, especially around the `login` query.
{% endhint %}

1. Sign up for FlashFX account here: [https://www.flash-fx.com/](https://www.flash-fx.com/) You'd need to provide us your driver's license or passport. We'll start verification process immediately. Typically takes an hour.
2. Ask us for API access in the support chat on the bottom right or on the [main site](https://www.flash-fx.com/). Or send an email to support@flash-fx.com.au
3. After we enable you go to the [https://api.flash-fx.com/](https://api.flash-fx.com/) playground, click **"SCHEMA"** on the right to explore the possibilities.
4. Find there the `login` query. Execute it to obtain your access token. For example: `mutation { login(input: {email: "YOUR_EMAIL" password: "YOUR_PWD"}) {token message} }`
5. Click the **"HTTP HEADERS"** on the bottom and add this: `{"authorization": "Bearer YOUR_TOKEN"}`. Replace the `YOUR_TOKEN` with the token you just got.
6. Execute any other queries.

For more detailed instructions head to the [How to start](basics.md) page.

