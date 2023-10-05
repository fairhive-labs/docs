---
description: >-
  Upon project completion or failure, rewards and fees are allocated. Initiators, fellowships, and the community receive or forfeit amounts based on project outcomes, ensuring accountability.
---

# Reward and Fee Distribution

In the decentralized world of PoLN, the act of compensating contributors for their efforts is paramount. This reward and fee distribution phase seeks to ensure that all stakeholders, be it initiators, fellowships, or the broader community, are fairly remunerated for their roles. Here, we delve into the intricacies of how value is allocated and distributed across the protocol, ensuring that there's skin in the game, commitment is sustained, and quality is continuously delivered. The system is meticulously designed, integrating a robust reward matrix for initiators based on project duration and a well-structured distribution plan for protocol fees. By doing so, PoLN creates a harmonious ecosystem where contributors are incentivized to align with the platform's objectives, leading to better outcomes for all. Dive in to understand the precision with which PoLN has crafted its reward and fee distribution mechanism.

## Success Scenario

Upon the successful completion of a project, the distribution system activates:

* Fellowship: The fellowship retrieves its staked tokens, and in addition, they are awarded the protocol fees as their primary remuneration.
* Initiator: The initiator gets rewarded from a predefined token pool based on the project's duration and the associated unit. The reward calculation is based on a matrix/grid system that considers both the project's duration and its time unit. As an example, for an 8 months long project, the initiator would receive 65536 $POLN.

## Unsuccessful Scenario

In the event a project is deemed unsuccessful:

* Fellowship: The fellowship loses its staked tokens as they are burnt, which incurs a financial loss for them. They also miss out on the protocol fees.
* Initiator: The initiator does not receive any reward.
* Community: The protocol fees, which would have otherwise gone to the fellowship, are redirected to the broader community. These funds are used for operations like training, helpdesk and support, mediation, KYC, development, maintenance, and refilling the initiator rewards pool.

## Aborted Projects

If a project is terminated before its set deadline:

* Fellowship: The fellowship's staked tokens are burnt.
* Initiator: The initiator can claim back the remaining payment that was locked for the contractor since they will no longer be getting paid. However, the initiator does not receive any rewards, and any protocol fees already paid are not refunded.
* Community: The community receives the protocol fees for their continued operational support.

## Halving Mechanism for Initiator Rewards

To ensure the sustainability of the reward system, there's a halving mechanism in place. As the token pool for initiator rewards depletes and reaches a reduction of 50%, the reward rates for initiators will be halved. This ensures that even as the available tokens in the pool reduce, the system can continue rewarding initiators for a longer period, thereby maintaining the attractiveness and viability of the PoLN platform.

{% hint style="success" %}
This mechanism ensures that all the stakeholders in a project, be it the initiator, the fellowship, or the community, have a clear understanding of the potential gains or losses. It emphasizes both the rewards for successful completion and the penalties for failures, thereby motivating all parties to maintain high standards of work and commitment.
{% endhint %}