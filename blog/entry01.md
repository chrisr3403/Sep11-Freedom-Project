# Entry 1
##### 11/3/24

## Section 1: What I learned So Far: 
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. 
I am using this tool [Kaboom](https://kaboomjs.com) a game development tool for platformer-style games. With this tool you can make games that can be pixelated or 
customizable. My learning of it has grown so much about it I have conducted many tests, such as programming AI to move to specific positions within the game.
One of the features I’ve learned is creating animations for sprites and AI.

```js
const bean = add([ sprite("bean", {// start with animation "idle" anim: "idle", }),])
```
This code is used for things such as idle animations in fact I am best known for doing idle animations for games and such. 
The idle makes it so the AI is in it's idle pose or static pose rather then just moving at all.
The original code will run for the AI or player to be a idle like this:

![image](https://github.com/user-attachments/assets/bcd1d5f8-8f05-48c2-98b1-26abc89eca31)

The idle makes it stay in one position or in most cases a animation while staying idle.

So what I tinkered with this code so far: 
```js
const bean = add([ sprite("bean", {// start with animation "run" anim: "run", }),])
```
^ instead of it taking the idle it's doing the running animation, when running its triggered when the player or AI wants to do that animation.
So it any case the running will go into a forward direction and not stay static idle which is good in most game scenario.

I started learning how to do animations due to creating AI and player cosmetics I realized I need to make the AI move at points of interest.
So I looked through Kaboom and found the code add:
```js
([sprite("ghosty"),pos(x, y),])
```
Here a example that shows in random points in time a sprite or a AI will move in any direction as shown in the video below:

![2024-12-02 21-29-11](https://github.com/user-attachments/assets/eb685641-71ba-42da-9138-7c05f880ba37)

But In my own tinkering instead of it going to random locations on a area the AI/Sprite must go to a location I forced it to go to.
Instead of the blank positioning I applied numbers on the grid to simulate how I want the player or sprite to spawn as it shows here in the code down below first the player location.
Here a example that I tinkered below:
```js
const player = add([
	sprite("optimus"),   
	pos(50, 50),    
	anchor("center")
```
![2024-12-0305-42-00-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/dd1014bc-3daa-4baf-8fd4-a9cf6d383ad6)

In this short video it demonstrates how the sprite itself is moving which can be useful for moving a sprite or a player to get to level 2 or final level
in a game which I myself have replicated multiple times which is very easy when switching the values of the location. 

During the location test I have done so far I got the picture on locations using the position which is very hard to do but it manage. It still needs room for improvement as the location must be accurate and for AI movement. My result was at first nothing happened but realized the AI was off the map. 
I would advice to keep on tinkering with the locations for you to know how to give a understanding on how they work.

Another part I tinkered with my Kaboom platformer is the skin of a sprite. 
This will be very useful in future game updates. What is it that I tinkered with?
This code for the sprite / Load a sprite asset from "sprites/bean.png", with the name "bean"
```js
loadSprite("optimus", "104-1047414_optimus-prime-pixel-art-transformers-optimus-prime-clipart.png")
```
This by default will load in a sprite being registered by a jpeg, png or even a gif.
The code can also be connected to the animations if you want a character to have a running pose or a standing pose.
Here is a preview of the tinkering on how to make the skin/sprite you want. (this goes for AI sprites too.)

![image](https://github.com/user-attachments/assets/218f52a3-9f82-4077-b61d-69301aaf34d0)

Image outcome 
![image](https://github.com/user-attachments/assets/dc816e8c-2b42-4feb-b33c-d1f88da0f567)

You need to also create your own png file so the sprite can be able to register it's skin.

![image](https://github.com/user-attachments/assets/da4d0900-f449-4c12-a376-0a9f0be46297)

Without the skin it will appear as a error on your screen make sure everything on it.
Everything must be registered also to the sprite name as well
Example being: `sprite("optimus")` the sprite must register the name "optimus" for the sprite character to load.

I used [Replit](https://www.youtube.com/watch?v=37rASpfnCCM) to give me a reference on how to make the sprites load in as the person in the video used replit and did the same 
method to make the images as sprites.

## Section 2: My Engineering Design Process: 
At the moment I think I am in the reserching part of this project level 2 overtime 
I will research more and more on how to make locations more accurate instead of just randomizing my location values. 
I will make it so my research will progress me to learn my tool further and make it to know new things for games.
For now I must research.

## Section 3: My Skills on Kaboom So Far.

I will go over the two skills I have learned and gained while using Kaboom:

Skill 1.
A Skill I gathered so far is creativity, I never thought of making a customizable sprites so it can make animations or change the color and skin.
This will be very good for the future because with amounts of creativity I can do I can make a full custom game.

Skill 2.
Another skill I have gathered so far is debugging, when I was tinkering I had issues with making a sprite have it's own skin
I always noticed how the issue was being made as the skin png itself was missing and so I created it for the skin to appear instead of getting a error.

--------------------------------------------------------------------------------------------------------------------------------------------------------

## My Original Blog. (Don't ever do it like this)
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. 
I am using this tool [Kaboom](https://kaboomjs.com) and here I will talk about what I have tinkered with.
You can choose what animations you want to use for your player and AI maybe a attack animation but so far it is limited to what animations you want to do.
Learning how to make animations is easy throughout the years of my experience and Kaboom extended that experience for my own platformer.
to create games. In time I have developed skills to know how to use my tool, skills such as knowing how to make more AI/sprites and make them also customizable.
The skill was very good to learn because then I can use the skills I know when it comes to making more AI I can make levels in games to be harder each time you increase a level.
It is really fascinating to learn Kaboom it is a useful tool even for my own personal projects. 
Another Skill I have learned is knowing how to make animations and this skill was something I have been wanted to learn and have because in the future AI or the player character 
needs to have animations like a battle animation or a run animation. Learning how to do animations is really important in future gaming purposes.
I would suggest it to any who want to create their own cosmetic or regular based platformer to have a real good experience on how to make games. 
My engineering design process, since I started learning how to do animations due to creating AI and player cosmetics I realized I need to make the AI move at points of interest.
So I looked through Kaboom and found the code add`([sprite("ghosty"),pos(x, y),])` this research lead me to find the position of the sprite 
So this code gave me a start on moving AI on certain POI (Points Of Interest) whenever starting the game or running it the Ai or sprite will spawn at different locations.
But since I need location numbers I would have to randomly pick random numbers to make the AI go to where I want it to move in the area. which helped me solve the issue. 
So I conducted a plan what I tinkered with this `([sprite("optimus"),pos(x 100, y 100),])` I made this prototype of the sprite to go through a random location so it can move. 
During the test I have done so far I got the picture on locations using the position which is very hard to do but it manage. It still needs room for improvement as the location must be 
accurate I may need something in the future for locations and AI movement. My result was at first nothing happened but realized the AI was off the map. I am still testing it but It 
needs to be assigned to a specific location number for the AI to move. You can tinker it in the example Kaboom [Kaboom Example](https://kaboomjs.com/play?example=add) this will take 
you to the example so you can tinker and see how it operates when changing a position to move a AI.





[Next](entry02.md)

[Home](../README.md)
