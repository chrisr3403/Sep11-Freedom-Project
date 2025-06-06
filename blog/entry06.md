# Entry 6
##### 6/3/2025

## Section 1: My Learning so far:
Hello My name is Christian Ramos and I am here to talk about my completion of my FP project and everything that I have done for the projects.
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

And with that I also used a reference from videos such as [Replit](https://www.bing.com/videos/riverview/relatedvideo?&q=kaboom.js+tutorial&&mid=E2CA825874E2F76A8E41E2CA825874E2F76A8E41&&FORM=VRDGAR) and 
[Shubham Gupta (Atom-8)](https://www.youtube.com/watch?v=xvTMVGnV660) amazing references on how to destroy pickups and make a score for these pickups.

## Section 2: My Engineering Design Process:
I am at my reserching part and probably even at its final stage of it. I want to streach my research so I can continue more of my project 
and over time I will gain more information in kaboom and over time I will go on to the next step of my research in the next blog.

## Section 3: My Skills on Kaboom So Far.
I will go over the two skills I have learned and gained while using Kaboom:

Skill 1. A Skill I gathered so far is creativity because when I was making the platformer game it looked to bland and it needed something that will be good and valuable.
So I added rings for others to collect and destroy for score to give the game a "alive" experence.

Skill 2. Another skill I have gathered so far is debugging, when I was tinkering I had looked on how the score was tied to the ring. After looking I noticed the class 
must be defined based on the ring and each ring you take boosts the score each time.
