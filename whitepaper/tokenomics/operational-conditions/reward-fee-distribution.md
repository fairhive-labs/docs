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

{% hint style="info" %}
In understanding the Initiator Rewards Pool's longevity for the $POLN token, it's crucial to determine how many projects can benefit from this pool before depletion. 
{% endhint %}

Specifically, we wish to derive both the minimum and maximum number of potential beneficiaries.

### Assumptions

1. Each time 50% of the remaining pool is used up, the reward amount is halved.
2. Projects continuously draw from the pool until it's empty.
2. There's no other mechanism influencing the reward amount other than the halving.
3. The Initiator Rewards Pool starts with a capacity of $$I$$ tokens, where $$I = 40,000,000$$ $POLN.
4. The reward $$R$$ given to a project, which varies based on the project's duration.

### Number of projects is constant per halving cycle

> Within the context of PoLN, a halving cycle is the phase where, after 50% of the remaining tokens in the Initiator Rewards pool have been distributed, the reward size for future projects is reduced by half. 

#### Initially - before first halving:
- Allocation for projects: $$A = \frac{I}{2} = 20,000,000$$
- Reward: $$R$$

Number of projects before the first halving:
$$
\frac{I}{2} \div R = \frac{I}{2R}
$$

#### After the first halving:
- Allocation for projects: $$A = \frac{I}{2} \div 2 = \frac{I}{4} = 10,000,000$$ 
- Reward: $$\frac{R}{2}$$ 

Number of projects during the first halving:
$$
\large \frac{\frac{I}{4}}{\frac{R}{2}} = \frac{I}{2R}
$$

#### Observations

Despite the reward reductions, the number of projects funded per cycle remains steadfast at $$\frac{I}{2R}$$.

#### Demonstration
The function $$a(n)$$ denotes the token allocation in the $$n^{th}$$ halving cycle:
$$
a(n) = \frac{I}{2^{n+1}}
$$

The function $$r(n)$$ denotes the reward in the $$n^{th}$$ halving cycle:
$$
r(n) = \frac{R}{2^n}
$$

The function $$p(n)$$ denotes the number of projects rewarded in the $$n^{th}$$ halving cycle:
$$
\large p(n) = \frac{a(n)}{r(n)} 
$$
$$
\large  \equiv p(n) = \frac{\frac{I}{2^{n+1}}}{\frac{R}{2^n}}\\
$$
$$
\large \equiv p(n) = \frac{I}{2^{n+1}} \times \frac{2^n}{R}\\
$$
$$
\large \equiv p(n) = \frac{I}{2R}
$$

{% hint style="success" %}
**Conclusion:**

The number of projects $$P$$ is constant per halving cycle:
$$
P = \frac{I}{2R}
$$
{% endhint %}

### Number of halving cycles

The number of halving cycles, $$N$$, is based on how many times we can halve the initial pool amount $$I$$:

$$
2^N = I
$$
$$
\equiv N = \log_2 I
$$

{% hint style="success" %}
**Conclusion:**

The number of halving cycles $$N$$ is:
$$
N = \log_2 I
$$
{% endhint %}

### Cumulative number of projects

{% hint style="info" %}
To compute the cumulative number of projects $$T$$ that can benefit from the pool until its depletion, we'll sum up the number of projects funded during each halving cycle. 
{% endhint %}

Given:
- $$N$$ is the number of halving cycles.
- $$P$$ is the number of projects for each halving cycle.
- $$I$$ is the initial allocation of the Initiator Rewards pool.
- $$R$$ represents the reward amount for a specific project duration (e.g., day, half-year).

The total number of projects across all halving cycles $$T$$ can be expressed as:

$$
T = N \times P
$$
$$
\equiv T = \log_2 I \times \frac{I}{2R}
$$

Since $$P$$ is constant across all cycles, the total number of projects that can be funded from the pool is simply the number of projects per cycle multiplied by the number of cycles.

{% hint style="success" %}
**Conclusion:**

For a specific reward $$R$$, the total number of projects $$T$$ that can benefit from the pool until its depletion is:
$$
\frac{I}{2R} \times \log_2 I
$$
{% endhint %}

### Determining the bounds

####  Lower Bound - Minimum Number of Projects

This corresponds to the case where the reward amount, $$R$$, is at its maximum, i.e., for long-term projects. 

For simplicity, let's say this is a half-year reward. 

If $$R_{\text{half-year}}$$ is the reward for a half-year project, then the total minimum number of projects $$T_{\text{min}}$$ that can be funded is:

$$
T_{\text{min}} = \frac{I}{2R_{\text{half-year}}} \times \log_2 I
$$

#### Upper Bound - Maximum Number of Projects

This corresponds to the case where the reward amount, $$R$$, is at its minimum, i.e., for short-term projects. 

Let's say this is a day reward. 

If $$R_{\text{day}}$$ is the reward for a day project, then the total maximum number of projects $$T_{\text{max}}$$ that can be funded is:

$$
T_{\text{max}} = \frac{I}{2R_{\text{day}}} \times \log_2 I  
$$

#### Conclusion

Given the nature of the halving mechanism, the total number of projects that can be funded from the Initiator Rewards Pool will always fall within the range:

$$ 
T_{\text{min}} \leq T \leq T_{\text{max}}
$$

Where:
- $$T_{\text{min}}$$ corresponds to the scenario when all projects claim the maximum reward (e.g., half-year projects).
- $$T_{\text{max}}$$ corresponds to the scenario when all projects claim the minimum reward (e.g., day projects).

In the context of the Initiator Rewards Pool $$I$$, for the maximum potential number of projects $$T_{\text{max}}$$, where each project claims the minimum reward (per day):

$$
T_{\text{max}} = \frac{I}{2R_{\text{day}}} \times \log_2 I  
$$

Plugging in $$I = 40,000,000$$ and $$R_{\text{day}} = 8$$:
$$
T_{\text{max}} \approx 63,133,741
$$

In the context of the Initiator Rewards Pool $$I$$, for the minimum potential number of projects $$T_{\text{min}}$$, where each project claims the maximum reward (per half-year):

$$
T_{\text{min}} = \frac{I}{2R_{\text{half-year}}} \times \log_2 I
$$

Plugging in $$I = 40,000,000$$ and $$R_{\text{half-year}} = 32768$$:
$$
T_{\text{min}} \approx 15,413
$$

{% hint style="success" %}
Therefore, we can conclude that the total number of projects, $$T$$, that can benefit from the Initiator Rewards Pool falls within the following bounds:

$$
15,413 \eq T \eq 63,133,741
$$
{% endhint %}

***

{% hint style="success" %}
This mechanism ensures that all the stakeholders in a project, be it the initiator, the fellowship, or the community, have a clear understanding of the potential gains or losses. It emphasizes both the rewards for successful completion and the penalties for failures, thereby motivating all parties to maintain high standards of work and commitment.
{% endhint %}
