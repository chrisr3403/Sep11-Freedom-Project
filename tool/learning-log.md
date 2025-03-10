# Tool Learning Log

## Tool: Kaboom

## Project: Game Editor DX

---

### 10/17/24:
* Hello My name is Christian Ramos and I am here to talk about my learning log and about my tool.
 I'am using [Kaboom](https://kaboomjs.com/)  for my Game editor DX. In some cases I tried to use the code that I started out for a game.
 Codes such as `// start the game kaboom()` as a way to start out the game of course I needed more time and code to try this but essentally I wanted to make a game start.
 My Progress on this is more slower then expected I still need to adapt to this tool and learn more about it.
 My question I really do have is: How will this work in some cases as giving it some thought. What will it give the audience the benefit of the doubt how good this game is.
 At first I had a challenge when it came to kahoots code. I thought "oh its just a game start up." well here is where it got tricky.
 See I needed more code when it came to my start game or things to make it give a idea on how to do it better. The code did not work at first
 then I looked into Kahoot gave me a code to play as a character and fixed it. The code gave me a sprite like this for example "// load a default sprite
 loadBean()" I want to try how to make a character move next.

  

### 10/18/24:
* Hello My name is Christian Ramos and here is a part two of my learning on kaboom!
In [Kaboom](https://kaboomjs.com/) I tried looking for the code to make my character move.
My progress is learning how to make a character jump which I had to look for it in Kaboom to make it work.
I used the code ```// jump when player presses "space" key
onKeyPress("space", () => {
// .jump() is provided by the body() component
    player.jump()``` which provides the player to jump essentially.
I had difficulty trying to find this code and making it work when I realized I missed a part of the code so I manage to fix it.
The question: How does code like this to make a character jump or play a animation. What makes the code function?
My next part will be on making the character be able to color change to whatever you want.

### 11/11/2024
* Hello My name is Christian Ramos making a report on my third learning log.
During my time using [Kaboom](https://kaboomjs.com/) I found codes that may lead to my cosmetic platformer project of 2025 and personal project for 2026
I have inspected this code ```// blue frogadd([ sprite("bean"),color(0, 0, 255)])```  This code makes the color of a AI/Sprite/Player Skin be customizable to any color you want.
Just Follow the code padlette to chose any color you want to see what suits your best interest in this game that will be made.
Now lets start with the challenges of this, my challenge to know how to use the color was very interesting I looked at the code for the ```color(0, 0, 255)```
and at first it looked like location numbers which I tried looking further to see if there was other methods actually I tried it out at first the code did not even
respond or work so I assumed it was until it was put in the wrong area. My progress on it seems very good as now I know how to make color on ai and player skins.
My questions I have is what will color bring to the games, what is the hot take on this custimizable platformer.
Well to answer that question sometime in the future I will try how to swap skins using a sprite skin swap. 

### 11/24/2024
* Hello and welcome to my learning log entry four! My name is Christian Ramos and I am to talk about my skin swapping lesson!
Using [Kaboom](https://kaboomjs.com/) I have been learning how to do skin swapping within a character or AI for quite sometime.
So I tried to give one of my sprite a optimus prime character and the progress of it is very very A BIG very easy progress and works perfectly.
I used this video to help me learn on how to make skins/png sprites [Learn to Make a Game with Kaboom.js in 39 Minutes](https://www.youtube.com/watch?v=hgReGsh5xVU&t=402s) with this I
learned how make a sprite have a different skin or png to whatever I want. What code I tinkered was with ```loadSprite("optimus",
"optimus.png") ``` this will basically make the character or AI have the sprite loaded as "optimus" you can change it to whatever you prefer on what project you are making.
A a-ha moments I have for myself is trying to get the png loading in I had the code but A BIG thing that I was missing is the png directory.
I thought I had put it in but I had to make it as a directory similar to github when putting a png.
The questions I still have is: How will Ai spawn? how will it be at a location when running the game? Next I will be trying location positions in Kaboom.

### 12/8/2024
* Hello and welcome to the learning log entry five! My name is Christian Ramos and I am here to discuss my learning on how to do positioning for sprites!
  Over the course of using my tool [Kaboom](https://kaboomjs.com/) I have been learning over time on making locations for AI or sprite start/spawns.
  So I did a experiment on a AI sprites for them to spawn though I will say the progress on it went by quick since it is a very simple process.
  I used this website to give me a idea on how to set a position of sprites which is [JSLegend](https://jslegenddev.substack.com/p/how-to-implement-player-controls)
  JSLegend has taught me all I need to know About positioning a sprite. The code I tinkered for my Sprite is the position:
 ```js
const player = add([
	sprite("Optimus"),
	pos(200, 90),
	anchor("center"),
])
```
What I did instead is experment with locations giving it number values to see where the sprite will appear on the game when running the game. 
I ran a few tests to see how the locations work and if you set the position to  `pos(x,y), ` it will teleport the sprite in different places after running the game multiple times. 
Though I did have some challenges for this such as pin pointing where I want the sprite to show up and to this day I have yet to know where to make it spawn where I want it to spawn.
Pin pointing these locations is hard if you want exact locations it's a hit or miss to make the location you want.
My question for locations is: How will we be able to pin point locatiosn correctly? Will it be easy to do? for what I will try next is moving a sprite manually using keys on the 
keyboard to see how will they all function all the same!

### 3/10/2025
* Hello and welcome to the learning log entry nine! My name is Christian Ramos and I am here to discuss my learning on how to do move a sprite in kaboom.js!
  from my knowledge so far to move a sprite using your keybinds is often needed if you want to play right?
  Without movement how will you do things in the game or even play!
  Thats why I am here to showcase my own code on how to move your sprite character in a kaboom with a click of a button!

  
 ```js
onKeyDown("left", () => {
    player.move(-SPEED, 2);
    player.flipX = true;
    // .play() will reset to the first frame of the anim, so we want to make sure it only runs when the current animation is not "run"
    if (player.isGrounded() && player.curAnim() !== "run") {
        player.play("run");
    }
});

onKeyDown("right", () => {
    player.move(SPEED, 2);
    player.flipX = false;
    if (player.isGrounded() && player.curAnim() !== "run") {
        player.play("run");
    }
});
```
What I did is look through my tool [kaboom](https://kaboomjs.com/) and also used this video as reference [CodeWithHarry](https://www.bing.com/videos/riverview/relatedvideo?&q=kaboom.js+game&&mid=9C03EE310C6A6B1F4FFA9C03EE310C6A6B1F4FFA&mmscn=mtsc&aps=0&FORM=VRDGAR_) I looked in both to see how do you move how does the function of a player is able to move?
What I did first is tried the code above it was the correct code I needed but 1 I did not try a key to see nor did I set a key up. I set it to key down right and I was able to move right and the
animation is triggered by this part of code `playerplay("run") and (player.isGrounded() && player.curAnim() !== "run")` - this part is where a run animation is triggered to move to the right. 
A ah moment was that I was missing a value or a part of the code which was connected to the speed this code is: `const SPEED = 1020;` this speed defines the movement speed without this
code the speed won't be defined and it will give you a error. My progress on it was very fast since all movement can be triggered with a click of a button.
My question is how does the key value get referenced to run? Why does the speed need to be refernecd when it also comes to animations.
Next will be my animations and actually going over the animation sets of what a sprite can do this will include sprite changing animations as well!

  

<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
