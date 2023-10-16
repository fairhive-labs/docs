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
Transparency stands as a cornerstone in the emerging world of web3 projects.
{% endhint %}

PoLN embodies this ethos, emphasizing the importance of openness and accountability. In a landscape where the trust of stakeholders is paramount, maintaining public visibility into source code becomes not just an ethical choice, but a strategic one.

{% hint style="success" %}
The choice to keep PoLN's source code in public repositories isn't merely about signaling honesty. It fosters a collaborative environment, encouraging community contributions, peer reviews, and shared innovation.
{% endhint %}

By doing so, PoLN aims to create a thriving ecosystem, underpinned by shared values and collaborative spirit.

In the broader context of blockchain and decentralized platforms, where trustless interactions are celebrated, PoLN's commitment to transparency further solidifies its position.

After all, in a realm where code often acts as the law, the ability for all to see, review, and understand that code becomes fundamental to the project's success and longevity.

***

## Roles / Categories

{% hint style="success" %}
The fairhive-labs Waitlist is a curated registry designed to streamline engagement within the PoLN ecosystem.

It recognizes and categorizes various individuals and entities keen on participating in PoLN project's journey.
{% endhint %}

This dynamic list is a testament to the diversity of roles and the synergy they bring:

### Initiator

<figure><img src=".gitbook/assets/PoLN - initiators.jpg" alt="" width="375"><figcaption></figcaption></figure>

An individual or entity that starts or triggers a specific action or process within the platform.

They set the ball rolling, often proposing new ideas, projects, or collaborations for the community to consider or adopt.

### Agent

<figure><img src=".gitbook/assets/PoLN - agents.jpg" alt="" width="375"><figcaption></figcaption></figure>

A representative or intermediary who takes actions on behalf of others.

In the context of the waitlist, they might manage or oversee certain processes, ensuring that tasks are carried out efficiently and effectively.

### Mentor

<figure><img src=".gitbook/assets/PoLN - mentors.jpg" alt="" width="375"><figcaption></figcaption></figure>

An experienced individual who offers guidance, support, and advice to less-experienced members.

They play a crucial role in nurturing talent within the community, sharing their knowledge, and helping others navigate challenges.

### Contractor

<figure><img src=".gitbook/assets/PoLN - contractors.jpg" alt="" width="375"><figcaption></figcaption></figure>

A person or entity hired to perform specific tasks or services for a limited period.

They might be involved in project execution, development tasks, or any other contracted work specific to the platform's needs.

### Investor

<figure><img src=".gitbook/assets/PoLN - investors.jpg" alt="" width="375"><figcaption></figcaption></figure>

Individuals or entities that financially support the project by investing in $POLN.

Real investors, in this context, are those who commit significant funds, typically more than $10,000.

Their investment often signifies a strong belief in the project's potential and a long-term commitment to its success.

### Contributor

<figure><img src=".gitbook/assets/PoLN - contributors.jpg" alt="" width="375"><figcaption></figcaption></figure>

Active members of the community who assist fairhive-labs in various capacities, from protocol development to marketing initiatives.

They provide invaluable support, often volunteering their time and expertise to drive the project forward.

### Advisor

<figure><img src=".gitbook/assets/PoLN - advisors.jpg" alt="" width="375"><figcaption></figcaption></figure>

Experienced professionals or enthusiasts who, while not directly involved in day-to-day operations, provide strategic insights, recommendations, and advice to fairhive-labs.

They have a genuine interest in the protocol's success and offer their expertise to help navigate challenges and seize opportunities.

***

## Detailed workflow

### Registration

The initial phase of the waitlist process starts when a user fills out the registration form. 

This form requires the user to provide several vital details:
- **Email Address**: A valid email for communications and further instructions.
- **Public Address**: The user’s blockchain address, linking future interactions to their identity.
- **Category Selection**: Based on the user's intended role in the ecosystem, be it as a contributor, investor, advisor, etc.
- **Sponsor's Public Address**: If introduced by an existing participant, the user can list the public address of their sponsor.

After submitting this form, the system creates a unique secure token, representing the user's provided data. 

This is known as a **JSON Web Token (JWT)**. Essentially, a JWT is a compact, URL-safe means of representation to claim between two parties.

{% hint style="success" %}
It offers a lightweight and stateless authentication mechanism that doesn't require storing session data on the server, making it inherently scalable.
{% endhint %}

This token serves a dual purpose. 

Firstly, it safeguards the system by eliminating the need to store user data temporarily, mitigating risks from both brute force and denial-of-service attacks. 

Secondly, the token ensures that the user provides a genuine email address. By sending an authentication link to the provided email address, the system ensures that only those with access to the email can proceed, verifying its authenticity. 

This strategy effectively prevents the use of fake or incorrect email addresses, as the registration process can't advance without accessing and authenticating through the sent link.

{% hint style="success" %}
In addition to the secured access link, the email also contains a distinct hash, generated from the token's attributes, enhancing security measures for the upcoming activation phase.
{% endhint %}

### Activation

Following the initial registration, the user receives an activation email containing a secured link and a unique hash. 

This link is their gateway into the PoLN ecosystem. When the user clicks on this link, they're prompted to submit the hash, solidifying their commitment.

Now, the PoLN system is thorough and vigilant. 

It starts by ensuring that users aren't bombarding it with excessive requests. 

With that assurance, it verifies the provided hash. Any discrepancy here, and the user is deemed unauthorized, halting the process.

Should the hash prove authentic, the system then turns its scrutiny towards the token, specifically its claims. 

An error at this stage again results in the user being marked as unauthorized, stopping the verification. 

But if everything checks out, the system extracts the user's data, encrypts it for safety—paying special attention to the email—and stores it securely.

To round off this intricate journey, a confirmation email is sent to the user, signaling the successful completion of the activation process. 

{% hint style="success" %}
Every step is designed to ensure user authenticity and the highest levels of data integrity.
{% endhint %}

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
