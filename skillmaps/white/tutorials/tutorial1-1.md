# Create your first Sprite

## Introduction @showdialog

** Let's make a sprite! **

You're going to make your first sprite.


## Design the hero of your story!
**Pick your favorite character or create your own.**

---

🔲 From the ``||sprites:Sprites||`` category, drag the ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` 
block and place it at the end of the ``||loops:on start||`` container.

🔲 Click on the grey box in the middle of your ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` block
to design a character of your own! Are you a brave knight, a cunning ninja, or a magical wizard?

🔲 The game console screen height is 120 and the width is 180. Use the ``||sprites:set [mySprite] position to x [ ] y [ ]||`` block to set the sprite's position in the middle of the screen.

*Hint: The center of the screen is half the height and width!*

---

```blocks
// @highlight
let mySprite = sprites.create(img`
    . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .)
