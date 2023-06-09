---
title:  "A New Objective: Metroid DNA"
tags: [Randomizer, Design Overview]
style: border
color: primary
description: Explaining my reasoning behind the new victory condition in *Metroid Dread*'s Randomizer.
attribution:
    - "*Metroid Dread* © 2021 Nintendo. All rights reserved." 
---

Randomizer design for metroidvanias has got to be among the most hyper-specific niches in game design. It's more or less unique to modding, though a handful of games have been adding official randos in recent years, and it needs to walk a very fine line: it needs to provide a unique experience every time it's played, while somehow remaining faithful to the unmodified game. Oftentimes, you can't have both, so compromises must be made.

While *Metroid Dread*'s rando was still experimental, we encountered a very serious design flaw. Most seeds felt pretty much the same! I was able to identify the biggest contributor to that outcome, which was the unmodified game's victory condition.  

{% include figure.html src="/assets/dread-dna/alttpr.png" caption="*A Link to the Past Randomizer*'s map screen shows which dungeons contains the required crystals."%}
Many games have victory conditions that lend themselves well to randomization. *A Link to the Past* has its crystals, requiring a random 7 of 10 dungeons to be completed before entering Ganon's Tower and beating the game. *Metroid Prime* has the Chozo Artifacts, dispersed randomly throughout the world and requiring all 12 to be found before gaining access to the final boss. *Dread* didn't have anything like that. All you needed was to navigate to the final boss and defeat him. This led to two distinct problems:

1. There was an extremely restrictive list of items required to beat the game. At an absolute minimum, exactly half of the major items were required in every seed - most seeds requiring several more than that. There was very little variance between seeds, as a result.
2. The objective was actually pretty unclear. The list of requirements was rather arbitrary, leaving players without an easily explained goal.

Solving #1 turned out to be surprisingly easy. Hanubia, the second-to-last area in the game, has two entrances, but one of them is blocked from the inside by a one-way gate. That gate was singlehandedly responsible for 7 of the 11 hard-required items, so removing it was virtually all that was needed. Doing so actually made it *too* easy to complete the game, but that was actually a fine problem to have.

See, this meant we suddenly had a very good reason to introduce additional requirements, and tie them into the new objective. There were a few things I wanted this objective to do:

1. Introduce more requirements, to patch up the hole left by removing the gate in Hanubia.
2. Randomize those requirements, to introduce variance between seeds.
3. Encourage the player to engage with parts of the game that were rarely visited with the original objective.


{% include figure.html src="/assets/dread-dna/experiment.webp" caption="Experiment Z-57 was a boss that was actually completely inaccessible in early versions of *Dread* rando!" %}
I started with #3 - which parts of the game were underutilized in rando? It didn't take long to come up with the answer. *Dread* was noteworthy for having some of the best boss fights in the series, but those bosses were rarely fought. So what if we made them required?

*Dread* had 6 major bosses, and 6 EMMIs (the antagonists on the cover art), adding up to a pool of 12 locations. These 12 locations, by chance, offered a good balance of requirements! 6 had no signficant additional requirements; 2 required the strongest beam upgrade; 2 required releasing the X parasites; and 2 required items which were otherwise next to useless. 

So now, in addition to reaching the final boss, we could introduce a requirement for a random selection of these bosses to be defeated in each seed. We tried a few different numbers, but after some playtesting we settled on 3 required bosses being a good default. This achieved the three things I was looking for from an objective, but it still needed to be communicated to the player, and ideally made a bit more thematic.

To inform the players of which bosses were required in their seed, we placed a hint at a guaranteed location in the mid-game. This hint actually serves the additional purpose of giving players a very clear early-game goal, before branching off to go defeat the bosses. 

Finally, to address the theming, I decided to call the items these required bosses drop "Metroid DNA", and justified it as the final boss being unwilling to fight you until you've collected them all. It's a pretty simple approach, but it's suitable for the *Metroid* universe. Most importantly, it doesn't get in the way of the gameplay. In a mod like rando, gameplay is paramount!

Today, collecting Metroid DNA remains the default and most popular objective for *Dread* rando. The original game's is still playable, but primarily for legacy's sake. Of course, when we first introduced this system, players weren't all super keen on it... but that's a story for another day.

