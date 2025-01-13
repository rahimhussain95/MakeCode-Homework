# Alien Invasion


```ghost
info.onCountdownEnd(function () {
    game.over(true)
})
sprites.onOverlap(SpriteKind.Player, SpriteKind.Projectile, function (sprite, otherSprite) {
    otherSprite.destroy(effects.rings, 200)
    info.changeScoreBy(1)
})
sprites.onOverlap(SpriteKind.Player, SpriteKind.Food, function (sprite, otherSprite) {
    otherSprite.destroy(effects.hearts, 200)
    info.changeLifeBy(1)
})
sprites.onOverlap(SpriteKind.Player, SpriteKind.Enemy, function (sprite, otherSprite) {
    otherSprite.destroy(effects.fire, 200)
    info.changeLifeBy(-1)
})
let projectile: Sprite = null
let extraLife: Sprite = null
let myEnemy: Sprite = null
scene.setBackgroundImage(assets.image`Freeway`)
scroller.scrollBackgroundWithSpeed(-50, 0)
let mySprite = sprites.create(assets.image`Momma`, SpriteKind.Player)
controller.moveSprite(mySprite, 0, 100)
mySprite.setStayInScreen(true)
info.startCountdown(15)
animation.runImageAnimation(
mySprite,
assets.animation`Momma Moving`,
100,
true
)
forever(function () {
    myEnemy = sprites.createProjectileFromSide(assets.image`Tourist`, -90, 0)
    myEnemy.y = randint(0, 120)
    myEnemy.setKind(SpriteKind.Enemy)
    pause(randint(1200, 2200))
})
forever(function () {
    extraLife = sprites.createProjectileFromSide(assets.image`Extra Life`, -90, 0)
    extraLife.y = randint(0, 120)
    extraLife.setKind(SpriteKind.Food)
    pause(randint(4000, 5000))
})
forever(function () {
    projectile = sprites.createProjectileFromSide(assets.image`Baby`, -90, 0)
    projectile.y = randint(0, 120)
    pause(randint(1000, 2000))
})

```


## {Intro @unplugged}

Let's create a stampede!

In this tutorial, you'll learn how to build your own alien invasion.

![It's an alien invasion!]("Try not to get in their way!" )



## {Step 2}

**🖼️ We can start with a background 🖼️**

---

► From the ``||scene:Scene||`` category, grab
``||scene:set background image to [ ]||`` and snap it into the empty ``||loops:on start||`` container already in the workspace.


► Click the **grey square** in the new block to open the image editor and choose a background from the **Gallery**.

---

**Hint:** After clicking the grey box, you can decide whether you want to create a background of your own, select a premade one from our **Gallery**, or select the same one we're using from **My Assets**.




```blocks
//@highlight
scene.setBackgroundImage(assets.image`Planet`)
```




## {Step 3}


**🛣️ Let's add movement to the scene 🛣️**

---

► To make it look like the camera is moving,
go to ``||scroller:Scroller||`` and drag
``||scroller:scroll background with vx [-90] vy [-90]||`` into **the end**
of the **on start** container.

► Change the horizontal speed by changing the value of **vx** to **-50** .

► Stop the background from scrolling vertically by changing the value of **vy** to **0**.


```blocks
scene.setBackgroundImage(assets.image`Planet`)
//@highlight
scroller.scrollBackgroundWithSpeed(-50, 0)
```



## {Step 4}

**🎮  Take a look at the simulator 🎮**

Your background should move on its own!



## {Step 5}

**Unleash the aliens!**

---

► From ``||loops:Loops||``, grab a
``||loops:forever||`` loop container and drag it into
an empty spot on the workspace.

► From ``||sprites:Sprites||``, grab
``||variables(sprites):set [projectile] to projectile [ ] from side with vx [50] vy [50]||``
and snap it into the empty **forever** container.

► Click the grey box to draw an alien sprite (or toggle to **Gallery** or **My Assets** to select one of ours.)


```blocks
forever(function () {
    let projectile = sprites.createProjectileFromSide(assets.image`Alien`, 50, 50)
})

```

