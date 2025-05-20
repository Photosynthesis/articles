---
title: A Game to Model Self-governing Economic Networks
post_date: 2020-03-01
---

*Note: the was first published on the [CadCad forum](https://community.cadcad.org/t/a-game-to-model-self-governing-economic-networks/137).*


**I want to answer this question: what are the necessary and sufficient conditions for an economic network to effectively govern itself?**

This post is about the possibility of designing an economic game (along the lines of the Iterated Prisoner’s Dilemma) that could help answer this question using transparency, reputation, and human nature to incentivize cooperation in relation to other participants and common resources.

Possible? Impossible? Please add your thoughts and comments to this thread. If you’re interested in collaborating let me know!

## Games, control hierarchies, the Wild West, and why this might be interesting

Simple [theoretical games](https://en.wikipedia.org/wiki/Game_theory) like the [prisoners dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma) and [public goods game 5](https://en.wikipedia.org/wiki/Public_goods_game) are widely studied, with putative implications ranging from [climate change mitigation](https://www.weforum.org/agenda/2018/06/the-moral-calculus-of-climate-change) to the [challenge of establishing trust](https://ncase.me/trust/), to the [origins of cooperation in biology](http://www-personal.umich.edu/~axe/research/Axelrod%20and%20Hamilton%20EC%201981.pdf).

Theoretical games are interesting for lots of reasons: as mathematical puzzles, as lenses on morality or ethics, as ways to test the rationality of humans, or as an encapsulation of reasonable intuitions about the real world. To me, they’re interesting as simplified models of the interaction between real-world systems and human nature.

For this objective, a game is valuable to the extent that aspects of behaviour within the game non-trivially reflect aspects of behaviour in some real system. If that is the case, then the game “world” can be used to understand behaviour in the real world, or design better strategies for improving it.

That’s what I’m hoping we can use an economic network game for.

## Classes of games

The classic IPD and the public goods game are [“non-cooperative” games 1](https://en.wikipedia.org/wiki/Non-cooperative_game_theory). In [“non-cooperative” games 1](https://en.wikipedia.org/wiki/Non-cooperative_game_theory), players compete with each other only, without an external authority enforcing cooperative behaviour. An “agreement” (cooperation) is only enforced by the parties to it (a [self-enforcing agreement 1](https://en.wikipedia.org/wiki/Self-enforcing_agreement)).

In “cooperative” games an external authority enforces agreements between players.

We can think of these two as the “Wild West” (it’s only your strategy in relation to other players that counts) and “Bureaucracy” (where a centralized authority enforces rules of behaviour).

In games, as in the real world, both of these structures encounter problems. The Wild West scenario lacks a mechanism to reward cooperators and deter defectors, making [Tit-for-Tat strategies 1](https://en.wikipedia.org/wiki/Tit_for_tat) optimal in most cases. In evolutionary IPDs, (in which AI players “evolve” by spreading their properties through the player population if they are successful), cooperative traits can gradually become very dominant (better results for all players). But, in these scenarios, if a defecting behaviour is introduced, it will win big in the population of cooperative “suckers”, and soon dominate the playing field, reverting to a Tit-for-Tat-as-optimal situation.

“Co-operative” games imply a central hierarchy to make and enforce the rules. Centrally enforcing the rules requires both a centralized coercive power, and centralized information about individual behaviour to determine when enforcement is necessary.

I think there’s something missing between these two classes. Neither of them seem to to a good job of modelling forms of human governance and economic structures that seem both possible and desirable.

**Could we design a simple, realistic game that used peer-to-peer reputation and transparency to make cooperation a winning strategy?**

**If so, could the game be a model for helping design actual economic systems?**

In many traditional societies, and (in a different way) in many online platforms, good behaviour is primarily enforced neither through strictly one-to-one “self-enforcing agreements” between parties, nor through centralized authority. Instead, it is enforced by reputation, or shared information about behaviour, leading to (in most cases) rewards and punishments of peer-to-peer inclusion or exclusion.

Digital economies make it possible to scale some patterns of reputation and social incentives that were previously limited to small groups in which individuals knew each other personally.

Would it be possible to design a game whose rules are not too much more complex than the IPD or the Public Goods Game, but which would capture the essential features of a collectively self-regulating decentralised economic system?

## Why a simple general network economy model might be useful

If such a game is possible, it would have at least three sorts of potential utility:

**Guiding the design of network economies**  
The most obvious application is to inform decisions about the design of economic networks. If the model is sound, can provide both a context for testing, and a reference design for network economies of the future.

**Basis for more detailed models**  
Again if the fundamentals of the model are sound, it can be built out with the details of specific economies to model their behaviour.

**Fixing economics**  
Mainstream economics is broken, and an example rigorously demonstrating that tragedies of the commons are not enevitable, and that centralized coercive control is not required to motivate pro-social behaviour could help with the project of fixing it.

## Possible models

### IPD with history

Possibly the simplest first step to test this would be to add transaction history to the IPD, so that the cooperate/defect history of a counterparty was known to the agent before initiating a transaction. This may have already been done, but if so I haven’t found it.

This wouldn’t model real-world situations particularly well, because in the real world, even if transactions are transparent it’s hard to obtain a transaction history from a counterparty that includes the necessary context to assess cooperate/defect behaviour.

### IPD with history and peer reputation

If players had access to the list of players a counterparty had transacted with, and could get those players’ assessment of the counterparty’s behaviour, the game would be closer to a real world marketplace like, for example, eBay or AirBnB.

But, this still wouldn’t allow reputational leverage when dealing with common pool resources.

### IPD with history, peer reputation and a commons (IPD+HPC)

We can add a sort of commons as a special player, with whom any player can transact. The commons player will always cooperate, as long as its balance is positive. If you cheat with the commons, you get ahead just as with any other form of cheating, but it also goes into your transaction history.

Here it gets tricky. We know, based on public goods game experiments, that humans will tend to punish or reward those who cheat and freeload, _even if meting out the punishment or reward is contrary to their economic self interest_. This makes sense from an evolutionary perspective, if we’re thinking in terms of selective pressures on groups, not just individuals.

In a IPD+HPC game, there probably isn’t a winning individual strategy that effectively deters pillaging the commons, _if we’re playing among rational computer agents_! If we’re playing among humans, there might be.

### Adding structure — IPD+HPC+S

There is a way that commons stewardship could become a rational strategy. If the game was not just a “blended soup”, but was a “sticky stew”, so that agents were to some extent grouped around commons, the dynamics would change. As soon as winning or losing is not measured relative to agents all transacting with the same commons, but to agents transacting with _another_ commons, the incentive to protect _your_ commons goes up.

This is in fact a more accurate representation of the world, at least in some respects!

A way this could work in practice is if there was an n-dimensional space in which players existed. Probability of being paired with another player, whether an individual or a commons, would be inversely proportional to distance. (The initial locations of player could be random, with some constraints to ensure a minimum distance between players. On some interval the “board” could be perturbated so proximities would change over the course of the game).

Another possibly simpler and mostly equivalent option: players are a vertices on a random graph, and degrees of separation predicts the likelihood of being paired for a transaction.

### Choice

In the classic IPD, a player only ever has one decision to make: cooperate or defect. Counterparties are randomly assigned, and there is no neutral or abstention option. This doesn’t really reflect reality. In fact the most common form of punishment in reputation systems is just to refuse to play. Those with bad reputations have to offer much more in order for others to be willing to transact with them.

–

An IPD-like game with peer reputation, commons players, some sort of structure, and the ability to choose whether to transact might go a long way toward making a useful model for real economic networks.

The IPD is certainly not the only, and likely not the most suitable, basic transaction structure on which to build this experiment. But, as a well studied and widely used model it makes a straightforward starting point. The dynamics of the basic IPD are well known, so it’s possible to assess tweaks and additions against an existing baseline.

A well designed implementation of this experiment would keep the transaction mechanics separate enough from the rest of the model that other formulas can be substituted for the IPD relatively easily.

## Questions

- Do versions of this exist already? If so, how do they work, and what are the results? If not, why not?
    
- What is this suggestion missing? Are there reasons it wouldn’t work in principle?
    
- What is the fastest technical approach to a good implementation? Would [Axelrod’s Python IPD library 4](https://github.com/Axelrod-Python/Axelrod) do it, or would it be better to possibly use some code from there and build with cadCAD (possibly with [MESA 2](https://github.com/projectmesa/mesa) or Networkx for agent modeling)?
    
- What is the best human process with which to validate, test, build, experiment, and document?
    
- Are there others pursuing or interested in similar things? If so who are they?
    

Thanks for reading!