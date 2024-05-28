# non-mandatoryflips


### IIP: Non-mandatory flip creation

**Author:** hlolve

**Status:** Draft

**Type:** Standard

### Non-mandatory flip creation to participate in validation ceremony

### Motivation

Whit influx of many candidates interested to get a validated ID in Idena network for use in other networks, at present we see many users
that can validate correctly during ceremony but leave the network because their commitment is not with Idena network and they are not
interested in rewards, so not interested in creating flips or running a node.

Creating flips is not a way to prove humannes with current rules. You can create 1-2-3-4 flips and still be a validator that secure the network.


### Rationale

Flips are one of the most important part for Idena security.
We need people creating flips that know the rules and interested in the risk of AI solving flips to make correct use of reporting.
Not interested people will never reach this kind of knowledge.

The proposal consist is separate in 2 groups people for validation ceremony.
In group #1 (same as current) will be the creators and only this group will also be able to report the flips.
In group #2 will participate only "solving" flips, they can't report flips. This group receives flips made by group #1.
In group #2 there isn't any committee, they only select left/right and the correct answers is determined by committees in group #1.
To be part of group #1 when submitting long session answers will choose or not to submit flips for next ceremony.

Remove IIP-7 to increase flip rewards, but 4th flip will receive 3x of flip rewards and 5th flips will receive 5x of flip rewards.
To avoid high participation of pools, only IDs with stake above vote discrimination (or a multiply of that amount) will be able to submit flips.
Only people that submitted flips and not reported will be able to mine in that epoch.
I think if 300 IDs apply for submitting flips will be enough, about 1000 flips.

Suppose you have many candidates for group #2 (20.000) and only 300 in group#1 submitting 1000 flips.
That 1000 flips will be distributed to others 20.000 IDs in group#2,
the risk is only a pool controlling many invites and try to solve that 1000 flips, but they will know results only after group#1 get consensus.
I am not worried by group #2 if we have correct incentives in group #1 and good flip creators and reporters in that group.

Additionally all "humans" in group#1 will receive 3 invitations and 1 more if 100% score, and "verified" only 1 if 100% score.
In group#2 only "humans" with high score to complete 50% of network size invitations.

Maybe invite rewards for inviter and invitee can be increased if new participant success in next validations as not reported validator of gropu#1
This means adjust also IIP-6 not only considering stake (as currently) but also quality of invitee.

I think sharding validation should not be affected, but maybe their number of participants in each shard can be increased with this two groups of validators model.

### Backwards Compatibility

This proposal requires changes to flip lottery and assignment of words pairs to create flips.
Maybe also changes to IIP-6 and remove IIP-7

### Security Considerations

The risk is not counting with enough flips, because not many apply to submit flips for next validation.
Is not a problem for group #1 because is same as current rules but in group #2 small set of flips could be an opportunity for farm pools to try to easy solve many accounts at ceremony.
In that case if at calculating results not many selected the option to be creators, that epoch will be same as current rules, mandatory for all validated IDs.
