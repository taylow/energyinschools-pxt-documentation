# add Score

Add more to the current score for the game.

```sig
game.addScore(1)
```
### Parameters

* a [number](/types/number) that means how much to add to the score. A negative number means to subtract from the score.

### Examples

This program is a simple game.
Press button ``A`` as much as possible to increase the score. 
Press ``B`` to display the score and reset the score.

```blocks
input.onButtonPressed(Button.B, () => {
    basic.showNumber(game.score())
    game.setScore(0)
})
input.onButtonPressed(Button.A, () => {
    game.addScore(1)
})
```

### See Also

[score](/makecode-blockeditor/reference/game/score), [set score](/makecode-blockeditor/reference/game/set-score), [start countdown](/makecode-blockeditor/reference/game/start-countdown)
