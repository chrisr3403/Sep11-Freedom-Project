Entry 3
2/9/25

## Section 1: What I learned So Far:
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. I am using this tool Kaboom a game development tool for platformer-style games. With this tool you can make games that can be pixelated or customizable. My learning of it has grown so much about it I have conducted many tests, such as making levels. One of the features I’ve learned is creating certain levels for the player and enemies.

A level is a static type of mesh or a brush mesh for players to walk on it is the thing to make a mission or objective to work in certain parts.
For example if you load in a level it will make it so you the player can walk on it levels are also very useful for platformer games.

I used a sprite from sonic sky sanctuary as a example down below.

![image](https://github.com/user-attachments/assets/8d6ecfaf-fb22-4873-8051-9024af92367c)

So what you are wondering how I did this what did I tinker to make the sky sanctuary block function in the game? I will share all this in what I tinkered so far.

## Section 2: So what I tinkered with this code so far:

loadSprite("skySanctuary.Low", "/sprites/SkySanctuaryLow.png");
^ this is the started up code this code registers the sprite of skysanctuary block so it may register in game.
A follow up to this is the code must be registered like I said before so to do this is the code below.
```
setGravity(2400);

const level = addLevel([
    "=",
```
Fun fact we have learned this recently with javascript for the mario pyrmid this is very similar to that matter.
const level register the level provided here is a preview down below.

![20250209_195034](https://github.com/user-attachments/assets/25d5dba4-04d4-47b6-b5af-02b2b8c4383c)

if increasing the add level symbol `"=",` to `"========",` the level will increase which I will use for my platformer 

Here is the result below.

![image](https://github.com/user-attachments/assets/a3d93f05-ad8e-4538-90e2-97acfac0c89c)

With the level blocks you can also make traps of some sort a spike trap.
Spike traps or traps or obsticles in general makes a full level playable for players to avoid.
What I did was instead of making a sprite I made a boost jumpad with it when I tinkered with it.

![20250209_201155](https://github.com/user-attachments/assets/3213b9c6-910f-4bdc-b259-c838fabb6573)

what I did was look at the code for the obsticle and instead of it giving you a game over sign you can make jumpads
so the player can do a super jump if needed to navigate.


Section 2: My Engineering Design Process:
At the moment I think I am in the reserching part of this project level 2 overtime I will research more and more on how to make locations more accurate instead of just randomizing my location values. I will make it so my research will progress me to learn my tool further and make it to know new things for games. For now I must research.

Section 3: My Skills on Kaboom So Far.
I will go over the two skills I have learned and gained while using Kaboom:

Skill 1. A Skill I gathered so far is creativity, I never thought of making a customizable sprites so it can make animations or change the color and skin. This will be very good for the future because with amounts of creativity I can do I can make a full custom game.

Skill 2. Another skill I have gathered so far is debugging, when I was tinkering I had issues with making a sprite have it's own skin I always noticed how the issue was being made as the skin png itself was missing and so I created it for the skin to appear instead of getting a error.
