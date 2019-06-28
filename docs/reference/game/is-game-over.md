# is Game Over

Find out if the game is over or not.

```sig
game.isGameOver()
```

## Returns

* a [boolean](/types/boolean) value that is `true` if the game is over or `false` if not.
# Example

Be kind and give the player some points for trying.

```blocks
if (game.isGameOver() && game.score() < 10) {
    game.addScore(10 - game.score())
}
```

## See also

[is running](/makecode-blockeditor/reference/game/is-running),
[is paused](/makecode-blockeditor/reference/game/is-paused)