Entry 1
11/3/24
Section 1: What I learned So Far:
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. I am using this tool Kaboom a game development tool for platformer-style games. With this tool you can make games that can be pixelated or customizable. My learning of it has grown so much about it I have conducted many tests, such as making levels. One of the features I’ve learned is creating certain levels for the player and enemies.

const bean = add([ sprite("bean", {// start with animation "idle" anim: "idle", }),])
This code is used for things such as idle animations in fact I am best known for doing idle animations for games and such. The idle makes it so the AI is in it's idle pose or static pose rather then just moving at all. The original code will run for the AI or player to be a idle like this:

image

The idle makes it stay in one position or in most cases a animation while staying idle.

So what I tinkered with this code so far:

const bean = add([ sprite("bean", {// start with animation "run" anim: "run", }),])
^ instead of it taking the idle it's doing the running animation, when running its triggered when the player or AI wants to do that animation. So it any case the running will go into a forward direction and not stay static idle which is good in most game scenario.

I started learning how to do animations due to creating AI and player cosmetics I realized I need to make the AI move at points of interest. So I looked through Kaboom and found the code add:

([sprite("ghosty"),pos(x, y),])
Here a example that shows in random points in time a sprite or a AI will move in any direction as shown in the video below:

2024-12-02 21-29-11

But In my own tinkering instead of it going to random locations on a area the AI/Sprite must go to a location I forced it to go to. Instead of the blank positioning I applied numbers on the grid to simulate how I want the player or sprite to spawn as it shows here in the code down below first the player location. Here a example that I tinkered below:

const player = add([
	sprite("optimus"),   
	pos(50, 50),    
	anchor("center")
2024-12-0305-42-00-ezgif com-video-to-gif-converter

In this short video it demonstrates how the sprite itself is moving which can be useful for moving a sprite or a player to get to level 2 or final level in a game which I myself have replicated multiple times which is very easy when switching the values of the location.

During the location test I have done so far I got the picture on locations using the position which is very hard to do but it manage. It still needs room for improvement as the location must be accurate and for AI movement. My result was at first nothing happened but realized the AI was off the map. I would advice to keep on tinkering with the locations for you to know how to give a understanding on how they work.

Another part I tinkered with my Kaboom platformer is the skin of a sprite. This will be very useful in future game updates. What is it that I tinkered with? This code for the sprite / Load a sprite asset from "sprites/bean.png", with the name "bean"

loadSprite("optimus", "104-1047414_optimus-prime-pixel-art-transformers-optimus-prime-clipart.png")
This by default will load in a sprite being registered by a jpeg, png or even a gif. The code can also be connected to the animations if you want a character to have a running pose or a standing pose. Here is a preview of the tinkering on how to make the skin/sprite you want. (this goes for AI sprites too.)

image

Image outcome image

You need to also create your own png file so the sprite can be able to register it's skin.

image

Without the skin it will appear as a error on your screen make sure everything on it. Everything must be registered also to the sprite name as well Example being: sprite("optimus") the sprite must register the name "optimus" for the sprite character to load.

I used Replit to give me a reference on how to make the sprites load in as the person in the video used replit and did the same method to make the images as sprites by the code of:

loadSprite("name", "name.png")
Section 2: My Engineering Design Process:
At the moment I think I am in the reserching part of this project level 2 overtime I will research more and more on how to make locations more accurate instead of just randomizing my location values. I will make it so my research will progress me to learn my tool further and make it to know new things for games. For now I must research.

Section 3: My Skills on Kaboom So Far.
I will go over the two skills I have learned and gained while using Kaboom:

Skill 1. A Skill I gathered so far is creativity, I never thought of making a customizable sprites so it can make animations or change the color and skin. This will be very good for the future because with amounts of creativity I can do I can make a full custom game.

Skill 2. Another skill I have gathered so far is debugging, when I was tinkering I had issues with making a sprite have it's own skin I always noticed how the issue was being made as the skin png itself was missing and so I created it for the skin to appear instead of getting a error.
