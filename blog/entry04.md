## Entry 2
3/15/25

## Section 1: My Learning so far:
Hello My name is Christian Ramos and I am here to talk about what I learned so far for using my tool during this month. I am using this tool [Kaboom](https://kaboomjs.com/) a game development tool for platformer-style games. With this tool you can make games that can be pixelated or customizable. My learning of it has exstended throughout the year I have conducted a lot tests, such as collecting items like rings from sonic or 
basically objective things for score to collect and increase your points in a game.

```js
"+": () => [
            sprite("example"),
            area(),
            anchor("bot"),
            "example",
        ],
```
This is a example of the first step on how to make a pickup or item. A sprite must be made before making anything else.
Just like my entry before this one a sprite is created by the code above and also to make the sprite visble you require this set of code
`loadSprite("example", "/sprites/example.png");` which loads the png of the sprite.

So what I tinkered with this code so far:



```js
loadSprite("ring", "/sprites/Ring.png");

"$": () => [
            sprite("ring"),
            area(),
            anchor("bot"),
            "ring",
        ],
```

![image](https://github.com/user-attachments/assets/95c50fd4-1e99-4fae-a092-b7c8d67cd5e2)
Making the sprite load to the key word of "ring" to load the png of the ring pickup.
Then I made a code for the action to pickup the ring is vaild follwing the code below.


``` js

player.onCollide("ring", (ring) => {
    destroy(ring);
});
```

^ this code is very new this code shows a result on when a player collides with the ring sprite.
when the player collides with the sprite it starts to take it as either a score or the ring is just gone or destroyed.

A example here from the video that I did:

![2025-03-16 21-36-42](https://github.com/user-attachments/assets/a723c90a-5f51-44a9-9252-1f946493b3f2)

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

Skill 1. A Skill I gathered so far is attention to detail because when I was looking at the keybinds I noticed the syntax of the keybinds it was missing something.
So I payed attention to whats missing I fortunatly I find the issue and it was missing another part of the code.

Skill 2. Another skill I have gathered so far is debugging, when I was tinkering I had problems making a sprite move thinking it was location based.
Instead I looked in further I saw that I can use keybinds to move my sprites entirly.
