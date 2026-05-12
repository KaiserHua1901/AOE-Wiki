# Modern Industrialization ![MI](img/mi_logo.png){width=128; align=right}
_A Mod about LOGISTICS and AUTOMATION for {--FABRIC 1.18--} EVER!_

## Frequently Asked Questions

### Fission Reactors

You may find Warbaque's fantastic [Reactor Planner](https://warbaque.github.io/MI-Reactor-Planner) is helpful and fun.
It's [README.md](https://github.com/warbaque/MI-Reactor-Planner/blob/main/README.md) also has good reactor plan solutions for various optimisation goals.

### High Pressure Loop: Advanced Boiler<sup>*</sup> :material-repeat: Heat Exchanger

_<sup>*</sup> or Fission Reactor... which is a pretty advanced way to boil water, don't you think?_

![High Pressure Loop](img/MI HP loop.png#only-light)
![High Pressure Loop](img/MI HP loop.dk.png#only-dark)
///caption
Fuel and Water go in, Steam comes out, and HP water re-circulates
///

A pressurizer is needed to initially prime the loop with HP water.
It won't take much, as 125mB of HP water takes up _16 times_ as much volume when turned to HP steam (2,000mB).

!!! tip
	If you are running (and thus boiling) HP water or HP heavy-water through a fission reactor, a small portion will be converted to Deuterium or Tritium, and this amount will need to be continually replaced.

## Early game
speedrun half a stack of copper and a stack of iron to make the mining drill
then mine around for coal/lignite just to fuel the drill
then get a bunch of early game materials (copper is abundant, so mostly whatever iron and tin you find), and a few diamonds for the macerators
then you can go back up and actually start making the basic machines like compressor, boiler, mixer
mixer 2nd is probably worth it for the better bronze ratio
still not many materials to leave anything running, so now make a fast entrance to a cave system (dig a hole down), and can soon start mining with silk touch on bc you have a macerator
don't fool yourself into "ah i'll stockpile steel before making machines with steel" just make a wall asap
having bolts on hand is so nice now
double ingot everything you do manually (early on) too
abuse forge hammering (it's fast), spend your first steel on hatches to speed up multis, abuse gunpowder. automate rubber and batch solder, don't be scared to spam bronze boilers, batch craft a lot, don't mine ore that you don't need (tungsten, monazite)
<!-- organize all this mess from Ramidz and Dino -->

## Pipes & Barrels
basically use one item pipe to connect everything.
Slot lock machines (EMI has a button for this, to make it easy)
One machine per recipe.
It’s nice to have each machine autoexport to its own neighboring MI barrel, which will display how much of its product it has, and act as an output buffer.
export from that barrel to the same one-item-pipe “network”
How does stuff stop and not over produce? Easy—if nothing is consuming its output, the barrel will fill and the machine will backup and stop.
But also… MI resource production is limited only by power provided to it, and some basic consumable, like a drill, that you also automate…
At base level, MI pipes move 16 items every 3 seconds. (they always operate on a 3 second/60 tick "clock"... that's part of how an extensive factory wide pipe can be not laggy.)

Adding motors to them will move more.

What gets moved depends on what can go where.

For example, if a macerator's input slot has any say, raw iron, in it when the pipe does it's thing, it can't only more raw iron will get moved into it's input slot.
For macerators, there's two things you can do about this...
<!-- from blue -->
### fluid pipe priority 
tank 1: I/O, priority 10, (full)
tank 2: I/O, priority 5, (full)
tank 3: In, priority 0, (empty)
fluid pipe network 10 pipes (10k mb/t)

1) extract 10k fluid from tank 1 into fluid pipe network
2) extract 0k fluid from tank 2 into fluid pipe network (network is full)
3) insert 10k fluid from fluid pipe network to tank 1 (tank 1 is full again)
4) insert 0k fluid from fluid pipe network to tank 2 (network is empty)
5) insert 0k fluid from fluid pipe network to tank 3 (network is empty)
- from Warbaque
### Item pipe Priority 
[item pipe pic](img/MI_item_pipe_priority.png)
the orange transfer happens first then the green transfer happens btw

explanation of the image:

    the priorities in brackets aren't applicable (they do nothing)
    the orange numbers say in which order items are inserted from the barrel with the orange square
    the green numbers say in which order items are inserted from the barrel with the green square
- from Triangular
---
