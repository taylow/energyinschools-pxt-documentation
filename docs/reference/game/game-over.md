# Game Over

End the game and show the score.

```sig
game.gameOver();
```

## Example

This program asks you to pick a button.
If you press button `A`, the program says `YOU WIN!`.
If you press button `B`, it shows an animation and ends the game.

```blocks
basic.showString("PICK A BUTTON");
input.onButtonPressed(Button.A, () => {
    basic.showString("YOU WIN!");
});
input.onButtonPressed(Button.B, () => {
    game.gameOver();
});
```

## See Also

[score](/makecode-blockeditor/reference/game/score),
[add score](/makecode-blockeditor/reference/game/add-score), [start countdown](/makecode-blockeditor/reference/game/start-countdown)
