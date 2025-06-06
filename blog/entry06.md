# Entry 6
##### 6/3/2025

## Section 1: My Learning so far:
Hello My name is Christian Ramos and I am here to talk about my completion of my FP project and everything that I have done for the projects.
Everything that ive done from making levels to bosses to pickups to switch sprites I have presented my project.

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
During my presentation I wanted to start off with my level code to present how does it work? Each symbol is linked with the const levelconf.
The symbol "=" makes the grass lineup following the level conf.
So to make the floor you also need a sprite as well to load it in.

So what I tinkered with this code so far:

```js
scene("start", () => {
    play("MenuTheme")

	add([
		text("Eat All"),
		pos(center()),
		scale(2),
		anchor("center"),
	])

	add([
		sprite("Menu"),
		pos(center()),
		scale(2),
		anchor("center"),
	])

    onKeyPress((space) => go("game"))

})
```

![image](https://github.com/user-attachments/assets/49606dd0-18ed-436a-81ba-fd761cb68833)

Once you load into kaboom, A screen will appear like above showcasing sonic screen as a example.
To head in game you have to press space bar to play!

At first It did not work because I wrote the code wrong.


``` js

player.onCollide("ring", (ring) => {
    destroy(ring);
});
```

^ this code is very new this code shows a result on when a player collides with the ring sprite.
when the player collides with the sprite it starts to take it as either a score or the ring is just gone or destroyed.



A example here from the video that I did:

![2025-03-16 21-36-42](https://github.com/user-attachments/assets/a723c90a-5f51-44a9-9252-1f946493b3f2)

I started to learn more on how objective/pickups work I was thinking it had something to do with the player destroying a item when coming into contact with it.
The more the player comes into contact with the ring the more the score increases each time during the score.

Ah yes score. When destroying a object or pickup you will be able to track score.

what I tinkered so far with score is this first part:

``` js
const score = add([
    text("Score: 0"),
    pos(24, 24),
    { value: 0 },
])
```
this tracks all the ring count anytime you destroy a ring the score number changes from zero to the amounts of pickups you do.
The score will show up on your side screen when making a code like this:

```js
player.onCollide("ring", () => {
        score.value += 1
        score.text = "Score:" + score.value
    })
```
I made it so it is linked with the ring and when linked to the ring each time a player destroys a ring the score shall increase each time.
and the score value is set at zero and each time you collect a ring the score value increases with the code of `score.value += 1` makes the score increase with the ring class.

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
