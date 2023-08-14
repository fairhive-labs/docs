---
description: >-
  In this very first part, the user submits a form, providing data which will be
  used to generate a unique token (JWT).
---

# step #1 — Registration

**Token** will be **used to generate a secured link** which will be **sent by email**. It will be **used to authenticate the user** in activation part.

Email will also **include** **a unique hash** (based on token’s claims).

{% hint style="success" %}
This approach **prevents our system from saving temporary state** or data.
{% endhint %}
