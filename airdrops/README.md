---
description: >-
  This article delves into the intricacies of the off-chain implementation of
  the PoLN pre-registration process, known as the waitlist.
cover: .gitbook/assets/ticket_validator.png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# ⛏ (WIP) Waitlist

{% hint style="info" %}
Transparency stands as a cornerstone in the emerging world of web3 projects.&#x20;
{% endhint %}

PoLN embodies this ethos, emphasizing the importance of openness and accountability. In a landscape where the trust of stakeholders is paramount, maintaining public visibility into source code becomes not just an ethical choice, but a strategic one.

{% hint style="success" %}
The choice to keep PoLN's source code in public repositories isn't merely about signaling honesty. It fosters a collaborative environment, encouraging community contributions, peer reviews, and shared innovation.&#x20;
{% endhint %}

By doing so, PoLN aims to create a thriving ecosystem, underpinned by shared values and collaborative spirit.

In the broader context of blockchain and decentralized platforms, where trustless interactions are celebrated, PoLN's commitment to transparency further solidifies its position.&#x20;

After all, in a realm where code often acts as the law, the ability for all to see, review, and understand that code becomes fundamental to the project's success and longevity.

***

## Roles / Categories

{% hint style="success" %}
The fairhive-labs Waitlist is a curated registry designed to streamline engagement within the PoLN ecosystem.

It recognizes and categorizes various individuals and entities keen on participating in PoLN project's journey.
{% endhint %}

This dynamic list is a testament to the diversity of roles and the synergy they bring:

### Initiator

An individual or entity that starts or triggers a specific action or process within the platform.

They set the ball rolling, often proposing new ideas, projects, or collaborations for the community to consider or adopt.

### Agent

A representative or intermediary who takes actions on behalf of others.

In the context of the waitlist, they might manage or oversee certain processes, ensuring that tasks are carried out efficiently and effectively.

### Mentor

An experienced individual who offers guidance, support, and advice to less-experienced members.

They play a crucial role in nurturing talent within the community, sharing their knowledge, and helping others navigate challenges.

### Contractor

A person or entity hired to perform specific tasks or services for a limited period.

They might be involved in project execution, development tasks, or any other contracted work specific to the platform's needs.

### Investor

Individuals or entities that financially support the project by investing in $POLN.

Real investors, in this context, are those who commit significant funds, typically more than $1,000.

Their investment often signifies a strong belief in the project's potential and a long-term commitment to its success.

### Contributor

Active members of the community who assist fairhive-labs in various capacities, from protocol development to marketing initiatives.

They provide invaluable support, often volunteering their time and expertise to drive the project forward.

### Advisor

Experienced professionals or enthusiasts who, while not directly involved in day-to-day operations, provide strategic insights, recommendations, and advice to fairhive-labs.

They have a genuine interest in the protocol's success and offer their expertise to help navigate challenges and seize opportunities.

***

## Detailed workflow

### Registration
In this very first part, the user submits a form, providing data which will be used to generate a unique token (JWT).

**Token** will be **used to generate a secured link** which will be **sent by email**. It will be **used to authenticate the user** in activation part.

Email will also **include** **a unique hash** (based on token’s claims).

{% hint style="success" %}
This approach **prevents our system from saving temporary state** or data.
{% endhint %}

### Activation

In this part, the previous token (JWT) is verified. User data is stored from extracted claims.

Finally, the user has to:

* open its favorite mail app and read our email,
* copy the unique hash,
* click on the secured link,
* paste the unique hash on activation form (_if it’s not already filled_) and last but not least, submit the form.

After multiple controls, preregistration flow is completed and a confirmation email is sent to the user 👍

### Sequences diagram

{% hint style="info" %}
For a comprehensive understanding, it is recommended to view the following schema in a new tab.
{% endhint %}

<figure><img src=".gitbook/assets/Pre-registration_Workflow_v2.0.png" alt=""><figcaption><p>complete pre-registration workflow</p></figcaption></figure>

***

## Future Improvements

User data can be stored on blockchain, generating incentives for users and sponsors.

Regarding the next **AirDrop**, /_activate_ **Response** may trigger an on-chain transaction, **saving user data in the blockchain** and **distributing free $POLN** **tokens** 💰 to users and sponsors.

{% hint style="info" %}
Keep posted :tada:
{% endhint %}