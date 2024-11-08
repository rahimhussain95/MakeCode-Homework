# Get to Know MakeCode Arcade 


```ghost
let mySprite: Sprite = null;
mySprite.startEffect(effects.spray)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    game.showLongText("The little unicorn walked into the meadow.", DialogLayout.Top)
    scene.cameraShake(4, 500)
})
scene.setBackgroundColor(9)
scene.setBackgroundImage()
mySprite.x += 0
effects.confetti.startScreenEffect()
effects.confetti.endScreenEffect()
mySprite.setPosition(70, 80)
for (let index = 0; index < 4; index++) {
    controller.moveSprite(mySprite)
    music.setVolume(20)
    music.playMelody("- - - - - - - - ", 120)
}
game.onUpdateInterval(5000, function () {
    if (game.askForString("Continue?") == "Y" || game.askForString("Continue?") == "y") {
        mySprite.say(":)")
    }
    game.splash("")
})

```

### @explicitHints true

## Introduction @unplugged

**Are you ready to start coding your own games?**

Complete this tutorial to learn how to:
- follow tutorial prompts
- find blocks in the toolbox
- build code in the workspace
- run your game on the built-in simulator 

Before you know it, you'll have an arcade game of your very own!

## step 1 

**⭐Welcome⭐**

You've just discovered the most important part of following a tutorial — reading instructions!

If you can't see all of the instructions, click **[v More...]** below to expand the box.

---

When you're ready to move to the next step, click **[ >  Next]** to continue.  


## step 2

This box is where you'll find information for each step. 

If you don't find all of the info you need, 
click the lightbulb to the right for an extra hint.


#### ~ tutorialhint 
```
**You found the hints!**
```


## Using the workspace

Now let's talk about your [__*workspace*__](#workIt "The area where you build code").

Your workspace is the area below the instructions where you'll connect blocks to build your program. 
Not all blocks will connect with one another, but we'll talk more about that later.

---

🔲 Click inside the text area of the ``||game:splash "___"||`` block 
and change the current sentence to something a little more exciting.

---

**Tip:** Did you notice that the first use of the word __workspace__ had a special look? 
From time to time, we'll enhance important words. Roll your mouse over them to see a definition.

#### ~ tutorialhint 
```blocks
game.splash("I like bananas!")
```

```template
game.splash("These blocks are in your workspace!")

```

## Meet the Blocks  @unplugged

Blocks can be dragged out from the  [__*toolbox*__](#tools "The strip to the left of your workspace that lists block categories."), 

connected, duplicated, and deleted.

Keep going to learn more about blocks.


