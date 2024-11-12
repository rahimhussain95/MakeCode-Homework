# Create your first Sprite

## Step 1

First let's creat your first sprite! 

Drag the Get a ``||input:temperature||`` block and place it in the value slot of ``||basic:show number||``.

```blocks
forever(function() {
    basic.showNumber(input.temperature())
    basic.pause(1000)
})
```