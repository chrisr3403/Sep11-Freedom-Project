## Entry 2
12/14/24

## Section 1: My Learning so far:
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. I am using this tool [Kaboom](https://kaboomjs.com/) a game development tool for platformer-style games. With this tool you can make games that can be pixelated or customizable. My learning of it has grown so much about it I have conducted many tests, such as programming AI to move to specific positions within the game. One of the features I’ve learned moving a sprite with a key or making them move to a location for you the player.

```js
player.moveTo(x, y)
```
This is a example of one of my learning. Setting a player or the sprite to move on it's own. Think of a cutscene in a game you want to make a cutscene that makes the player run to the 
cutscene in the game or approching a part of the map like a reach point.

So what I tinkered with this code so far:

``` js
player.moveTo(300, 200)
```

^ instead of the x y and I did the location where I want the sprite of my player to be at. This can be useful for checkpoints, like for example let's say you failed a level the 
location can be triggered so you move to that location instead similar to giving locations to a ghost sprite.

A example here from the video that I did.

![2024-12-16 13-11-22](https://github.com/user-attachments/assets/b6da3840-bcfd-48ed-85ca-3408a8c2bf31)

I started to learn more on how to make a player move where I want it which is something I can takeaway from this.

Another part I tinkered with was moving your character manually.
For this it requires keys on your keyboard so you will be able to move the character you play as.
From kaboom here is a example:

![image](https://github.com/user-attachments/assets/b6a0247c-1429-4331-9265-5d21bab2b594)

Pressing a key triggers anything that the key is assigned to.
But In my own tinkering I made it so you can move left and right as your character my code example is down below.

![image](https://github.com/user-attachments/assets/5a4ce0a8-a397-4cdc-9bd4-589b40c5710f)

this code demostrates the programing on moving using a key so the sprite can move. In the future this can be useful for when you want a sprite to move on command.

Here is the video tinker result:

![2024-12-16 13-39-04](https://github.com/user-attachments/assets/97a29397-a859-435c-b4ee-9afc3bb020bf)

The video has shown massive results as it shows how I can move my sprite side to side.
So in the future when I make the game you can navagate in the level so you can roam freely.
So by default the movement will respond to the code of:

```js
onKeyDown("left", () => {
    player.move(-SPEED, 0)
```
though the code needs to respond to another code with the speed because if it does not have this code:

```js
const SPEED = 320
```

you will get a error message of:
![image](https://github.com/user-attachments/assets/2f9933f1-25ac-410f-b6ba-21b1191a651a)

Without the const speed the speed won't be defind which will cause issues
so what I did is add the const speed missing code to make it work which showed the speed must be referenced.
You can modify the speed to any way you want so say what I did was 320 normal speed but if I put it to 0 it will not move.
I used a video guide from [freecodecamp](https://www.bing.com/videos/riverview/relatedvideo?&q=kaboom+tutorial&qpvt=kaboom+tutorial&mid=6A99D7A7E5AE3EDBAACB6A99D7A7E5AE3EDBAACB&mmscn=mtsc&aps=0&FORM=VRDGAR) to give me a idea on how to move characters.

## Section 2: My Engineering Design Process:
Just like my first blog I am still at the reserching part of this project level 2 still I will continue to research so I can continue with my project 
but so far I am at the reserching part my stage over time will hopefully increase based on my knowledge for my projects and Kaboom.

## Section 3: My Skills on Kaboom So Far.
I will go over the two skills I have learned and gained while using Kaboom:

Skill 1. A Skill I gathered so far is creativity, I never thought of making a customizable sprites so it can make animations or change the color and skin. This will be very good for the future because with amounts of creativity I can do I can make a full custom game.

Skill 2. Another skill I have gathered so far is debugging, when I was tinkering I had issues with making a sprite have it's own skin I always noticed how the issue was being made as the skin png itself was missing and so I created it for the skin to appear instead of getting a error.
