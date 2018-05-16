---
title: IslandCoin White Paper
---

Persons: Hugo, Sawyer, Kate, Jack


## Motivation

Blockchain is changing the world around us redistributing value in
a fair and decentralized way. The island's barter economy is
holding back progress. We want to disrupt the economy by
introducing a novel cryptographic currency - IslandCoin.


## Consensus

The consensus algorithm for IslandCoin is based on a consortium of 4 members [H, S, K, J]. 
It is a permissioned leader-based
algorithm that is tolerant to Byzantine behavior [1] of up to 1/3
of the network. The algorithm requires a majority vote of over 50%
of consortium members to approve a block. All members have equal
voting rights.

Block time is approximately 24 hours. Blocks are published by the
leader which is selected using a round robin mechanism.


## Transaction and Block Specification

### Transaction format

[SENDER ADDRESS, NONCE, RECIPIENT ADDRESS, AMOUNT, SIGNATURE]


### Block format

[BLOCK NUMBER, TRANSACTIONS 1..N, BALANCES 1..4, SIGNATURES 1..4]


### Genesis block

[1, [], [100,100,100,100], [H, S, K, J]]


## References

[1] L. Lamport, R. E. Shostak, and M. C. Pease. The byzantine generals problem. ACM, 4(3):382–401, 1982.


