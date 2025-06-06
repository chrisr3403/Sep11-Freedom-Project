# Entry 6
##### 6/3/2025

## Section 1: My Learning so far:
Hello My name is Christian Ramos and I am here to talk about my completion of my FP project and everything that I have done for the projects using kaboom.js!
Everything that ive done from making levels to bosses to pickups to switch sprites I have presented my project.
Each work I have put in since december on this FP has been amazing and doing the things I liked for make it such as sonic is a great idea!
What did I present is the question?

What I presented first was the levels for the game as seen down below:

## Levels

```js
[
		"     $    $    $    $     $",
		"     $    $    $    $     $",
		"                           ",
		"                           ",
        "                           ",
        "                           ",
		"                           ",
		"                           ",
		"                           ",
		"                           ",
        "                           ",
        "                           ",
		"                           ",
		"                           ",
        "                           ",
		"                           ",
		"                           ",
        "                           ",
        "                           ",
		"                           ",
        "                           ",
		"                           ",
		"                           ",
		" $$$    $$$   ;;        $$$   ?  $$$ ? $$$    ;;;;;;;;;;;;  @",
"======================================================================="
	],
]

        const levelConf = {
        tileWidth: 80,
        tileHeight: 50,
        tiles: {
        "=": () => [
			sprite("grass"),
			area(),
			body({ isStatic: true }),
			anchor("bot"),
			"platform",
        ],
```
![image](https://github.com/user-attachments/assets/8ed107aa-5fa2-4287-b39a-da18d0449582)

During my presentation I wanted to start off with my level code to present how does it work? Each symbol is linked with the const levelconf.
The symbol "=" makes the grass lineup following the level conf.
So to make the floor you also need a sprite as well to load it in.


The next thing I presented is my code for the swap sprite:
## Character swap:

```js
function SonicSprite() {
player.scale = vec2(1)
player.use(sprite("Sonic"));
Sprite.text = "Player: Sonic";

}

onKeyPress("s", () => {
    SuperSonicSprite();
    setGravity(700);
    scale(1200);
    player.play("super");
});

const Sprite = add([
    color(255, 165, 0),
    text("Player: Sonic ", { size: 40 }),
    pos(25, 100),
    fixed(),
]);
```
![chrisr3403 github io_Sep11-Freedom-Project_ and 67 more pages - Personal - Microsoft_ Edge 2025-06-06 06-22-27](https://github.com/user-attachments/assets/c92bfd4a-08c5-42cb-87ce-e4ba9f468988)

With this one I wanted to present so much because of how much detail there is to it!
swap sprite gives the content way better look! 
How it functions is that you need a function for the swap sprite and link it to player.use for the player to use that sprite instead of the default one.

### traps
The last one would be traps obsticles rather to show the game difficulty 
```js
loadSprite("spike", "sprites/Spikes3.png")

";": () => [
            sprite("spike"),
            area(),
            anchor("bot"),
            scale(0.4),
            "danger",
        ],

player.onCollide("danger", () => {
		go("lose")
		play("SpikeDed")
	})
```
![image](https://github.com/user-attachments/assets/e5d32891-5db5-4a6c-a0c9-3a474becef23)

Since the game needed difficulty, spikes were added to give off that difficulty!
Each time you touch the spike you get a game over scene and as well as starting over again.
It has a hitbox range which you can tinker as well and is also connected to levels as seen above.


And with that I also used a reference from videos such as [Replit](https://www.bing.com/videos/riverview/relatedvideo?&q=kaboom.js+tutorial&&mid=E2CA825874E2F76A8E41E2CA825874E2F76A8E41&&FORM=VRDGAR) and 
[Shubham Gupta (Atom-8)](https://www.youtube.com/watch?v=xvTMVGnV660) to help me have a idea on the things I need to work on!

## Section 2: My Engineering Design Process:
YES! Even at this time, I am still at my reserching part. I want to continue my research of kaboom.js over the summer and years to come.
I want to be a game developer one day and I stil feel I need more reserach. I will continue to reserach kaboom.js over time!

## Section 3: My Skills on Kaboom So Far.
I will go over the two skills I have learned and gained while using Kaboom:

Skill 1. A Skill I gathered so far is creativity because I never thought of making a swap sprite until last month or how I would make it work rather.
I used so many references that I can work with to make this possible.

Skill 2. A Skill I gathered so far is attention to detail because when I was looking at the at the swap character I noticed it needed more details. 
So what I did was make it so a name also gets swapped with the character itself to make it look good!
