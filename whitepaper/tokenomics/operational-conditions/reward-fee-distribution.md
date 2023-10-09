---
description: >-
  Upon project completion or failure, rewards and fees are allocated.
  Initiators, fellowships, and the community receive or forfeit amounts based on
  project outcomes, ensuring accountability.
cover: ../../.gitbook/assets/rewards_fees_distribution.png
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

# Reward and Fee Distribution

In the decentralized world of PoLN, the act of compensating contributors for their efforts is paramount.

This reward and fee distribution phase seeks to ensure that all stakeholders, be it initiators, fellowships, or the broader community, are fairly remunerated for their roles.

Here, we delve into the intricacies of how value is allocated and distributed across the protocol, ensuring that there's skin in the game, commitment is sustained, and quality is continuously delivered.

The system is meticulously designed, integrating a robust reward matrix for initiators based on project duration and a well-structured distribution plan for protocol fees.

By doing so, PoLN creates a harmonious ecosystem where contributors are incentivized to align with the platform's objectives, leading to better outcomes for all.



## Success Scenario

Upon the successful completion of a project, the distribution system activates:

* **Fellowship**: The fellowship retrieves its staked tokens, and in addition, they are awarded the protocol fees as their primary remuneration.
* **Initiator**: The initiator gets rewarded from a predefined token pool based on the project's duration and the associated unit. The reward calculation is based on a matrix system that considers both the project's duration and its time unit. As an example, for an 8 months long project, the initiator could receive 65536 $POLN.

<figure><img src="../../.gitbook/assets/project succeeds.jpg" alt="" width="563"><figcaption></figcaption></figure>

## Unsuccessful Scenario & Aborted Projects

In the event a project is deemed unsuccessful:

* **Fellowship**: The fellowship loses its staked tokens as they are burnt, which incurs a financial loss for them. They also miss out on the protocol fees.
* **Initiator**: The initiator does not receive any reward.
* **Community**: The protocol fees, which would have otherwise gone to the fellowship, are redirected to the broader community. These funds are used for operations like training, helpdesk and support, mediation, KYC, development, maintenance, and refilling the initiator rewards pool.

<figure><img src="../../.gitbook/assets/project fails.jpg" alt="" width="563"><figcaption><p>Failed projects benefit the broader community</p></figcaption></figure>

If a project is terminated before its set deadline:

* **Fellowship**: The fellowship's staked tokens are burnt.
* **Initiator**: The initiator can claim back the remaining payment that was locked for the contractor since they will no longer be getting paid. However, the initiator does not receive any rewards, and any protocol fees already paid are not refunded.
* **Community**: The community receives the protocol fees for their continued operational support.

### Cycling Failure into Community Prosperity

When a project fails, the fees reserved for it are redirected to benefit the broader community by channeling them to the DAO.

Instead of being a mere setback, these funds become instrumental in the continuous enhancement and evolution of the ecosystem.

They are strategically allocated to vital operations, including but not limited to:

* **Training:** Investing in the education and upskilling of the community, ensuring everyone remains abreast of the latest trends and methodologies.
* **Helpdesk and Support:** Maintaining a robust support system to assist users, resolve queries, and ensure a seamless experience for everyone involved.
* **Mediation:** Offering dispute resolution mechanisms, ensuring fairness, and maintaining trust within the ecosystem.
* **KYC Procedures:** Ensuring the integrity and security of the community by verifying the identity of its members, safeguarding against potential malfeasance.
* **Development and Maintenance:** Channeling resources towards the continuous improvement of the platform's infrastructure, tools, and features.
* **Refilling the Initiator Rewards Pool:** Ensuring that incentives remain in place to attract new project initiators to the platform.
* **Liquidity Pools:** Creating and replenishing liquidity pools, ensuring the smooth trading of tokens and bolstering overall market stability.

By transforming the outcome of failed projects into tangible benefits, the protocol not only preserves community trust but also reinforces its commitment to growth, adaptability, and long-term sustainability.

## Halving Mechanism for Initiator Rewards

To ensure the sustainability of the reward system, there's a halving mechanism in place.

<figure><img src="../../.gitbook/assets/PoLN - initiators rewards + halving.jpg" alt="" width="563"><figcaption></figcaption></figure>

As the token pool for initiator rewards depletes and reaches a reduction of 50%, the reward rates for initiators will be halved.

This ensures that even as the available tokens in the pool reduce, the system can continue rewarding initiators for a longer period, thereby maintaining the attractiveness and viability of the PoLN platform.

In understanding the Initiator Rewards Pool's longevity for the $POLN token, it's crucial to determine how many projects can benefit from this pool before depletion. 

Specifically, we wish to derive both the minimum and maximum number of potential beneficiaries.

### Assumptions

1. Each time 50% of the remaining pool is used up, the reward amount is halved.
2. Projects continuously draw from the pool until it's empty.
2. There's no other mechanism influencing the reward amount other than the halving.
3. The Initiator Rewards Pool starts with a capacity of $ P $ tokens, where $ P = 40,000,000 $ $POLN.
4. The reward $ R $ given to a project, which varies based on the project's duration.

### **Step 1: Demonstrate that the number of projects is a constant in each halving cycle**:

At the beginning:
- Pool = $ P $
- Reward = $ R $

Number of projects before the first halving:
\[ \frac{P}{2} \div R = \frac{P}{2R} \]

After the first halving:
- Remaining pool = $ \frac{P}{2} $
- Reward = $ \frac{R}{2} $

Number of projects during the first halving:
\[ \frac{P/2}{2 \times R/2} = \frac{P}{2R} \]

Thus, for each halving cycle, the number of projects funded remains constant at $ \frac{P}{2R} $.

### **Step 2: Compute the number of halving cycles**:

The number of halving cycles, $ n $, is based on how many times we can halve the initial pool amount:

\[ n = \log_2(40,000,000) \]

### **Step 3: Determine total projects for a specific reward $ R $**:

Given $ n $ halving cycles and that each cycle funds $ \frac{P}{2R} $ projects:

\[ \text{Total projects} = n \times \frac{P}{2R} \]

### **Step 4: Conclusion - Determining Min and Max Projects**:

Substitute $ R $ with $ H $ for half-year reward and $ D $ for day reward:

\[ \text{Min projects} = \frac{P}{2H} \times \log_2(40,000,000) \]
\[ \text{Max projects} = \frac{P}{2D} \times \log_2(40,000,000) \]

By inserting specific values for $ P $, $ H $, and $ D $, we'll determine the exact range for the number of projects that can be funded before the pool is depleted.

***

{% hint style="success" %}
This mechanism ensures that all the stakeholders in a project, be it the initiator, the fellowship, or the community, have a clear understanding of the potential gains or losses. It emphasizes both the rewards for successful completion and the penalties for failures, thereby motivating all parties to maintain high standards of work and commitment.
{% endhint %}
