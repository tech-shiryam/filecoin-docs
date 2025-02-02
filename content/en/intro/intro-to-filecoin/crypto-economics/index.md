---
title: "Crypto-economics"
description: "Crypto-economics is the study of how cryptocurrency can incentivize useages of a blockchain network. This page covers how Filecoin manages incentivization within the network."
lead: "Crypto-economics is the study of how cryptocurrency can incentivize useages of a blockchain network. This page covers how Filecoin manages incentivization within the network."
draft: false
images: []
type: docs
menu:
  intro:
    parent: "lorem"
    identifier: "crypto-economics-143c9881701c30993def24fb1f1619f8"
weight: 20
toc: true
---

## Native currency

The native currency of Filecoin, FIL, is a utility token used to incentivize persistent storage on the Filecoin network. Storage providers mine FIL by providing reliable storage service or committing storage capacity on the network. It has a maximum circulating supply of 2,000,000,000 FIL, meaning that no more than 2 billion Filecoin will ever be created.

As a utility token that aligns participants’ incentives with the long-term growth of the network, Filecoin issuance is aligned with the overall provable utility of the network. The majority of Filecoin supply would only be minted if the network achieved growth and utility targets at scale.

Specifically, Filecoin uses a [dual minting model](https://spec.filecoin.io/%23section-systems.filecoin_token.minting_model&sa=D&source=editors&ust=1674147484220325&usg=AOvVaw25eQbNyiZGSVUEtPqqoNs_) for block reward minting:

## Baseline minting

Up to 770M FIL tokens are minted based on the performance of the network. These tokens would only fully release if the Filecoin network reached a Yottabyte of storage capacity in under 20 years, estimated to be ~1000x larger than today’s cloud storage capacity.

## Simple minting

330M FIL tokens are released on a 6 year half-life based on time, meaning that 97% of these tokens will be released in approximately 30 years time.

Additionally, 300M FIL tokens are held back in the mining reserve to incentivize future types of mining.

## Vesting

Mining rewards undergo a vesting schedule to encourage long-term network alignment. For example, 75% of block rewards earned by miners vest linearly over 180 days, while 25% are made immediately available to improve miner cash flow and profitability. And the remaining FIL tokens are vested to Protocol Labs teams and Filecoin Foundation over 6 years and SAFT investors over 3 years, as shown in the [vesting table](https://spec.filecoin.io/systems/filecoin_token/token_allocation/filtokenallocation.png&sa=D&source=editors&ust=1674147484221810&usg=AOvVaw0APuLa2qxi8zOsOWsvv500) here.

## Collateral and slashing

To encourage good behavior from network participants, during block reward mining, storage providers must lock Filecoin tokens as [pledge collateral](https://spec.filecoin.io/%23section-systems.filecoin_mining.miner_collaterals.initial-pledge-collateral&sa=D&source=editors&ust=1674147484222187&usg=AOvVaw0peY2CM6khJetFkBnendi5) for consensus security, storage reliability, and contract guarantees. Pledge collateral is determined by projected block rewards that a miner would earn. Collateral and all earned rewards by storage providers are subject to slashing throughout the lifetime of a sector if the storage does not pass a reliability check.

## Total supply

FIL has a maximum circulating supply of 2,000,000,000 FIL, meaning that at most 2B Filecoin will ever be created. In practice, this max supply would never be reached since a considerable amount of FIL are burnt as gas fees, penalties etc., and are permanently removed from circulating supply.
