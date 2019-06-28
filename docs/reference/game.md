# Game

Make games with sprites. Keep score and controls gameplay. 

## ~ hint

Once the game engine is started, it will render the sprites to the screen and potentially override any kind of animation you are trying to show.
Using [game pause](/makecode-blockeditor/reference/game/pause) and [game resume](/makecode-blockeditor/reference/game/resume) to disable and enable the game rendering loop.

## ~

## Sprites

```cards
game.createSprite(0,0);
game.createSprite(0,0).delete();
game.createSprite(0,0).move(0);
game.createSprite(0,0).turn(Direction.Left,0);
game.createSprite(0,0).ifOnEdgeBounce();
game.createSprite(0,0).get(LedSpriteProperty.X);
game.createSprite(0,0).set(LedSpriteProperty.X, 0);
game.createSprite(0,0).change(LedSpriteProperty.X, 0);
game.createSprite(0,0).isTouching(null);
game.createSprite(0,0).isTouchingEdge();
```

## Scoring

```cards
game.addScore(1);
game.score();
game.setScore(0);
```

## Life

```cards
game.setLife(0)
game.addLife(0)
game.removeLife(0)
```

## Game control

```cards
game.startCountdown(10000);
game.gameOver();
game.pause();
game.resume();
game.isGameOver()
game.isRunning();
game.isPaused();
```

## See also

[create sprite](/makecode-blockeditor/reference/game/create-sprite), [move](/makecode-blockeditor/reference/game/move), [turn](/makecode-blockeditor/reference/game/turn),
[ifOnEdgeBounce](/makecode-blockeditor/reference/game/if-on-edge-bounce), [get](/makecode-blockeditor/reference/game/get), [set](/makecode-blockeditor/reference/game/set),
[change](/makecode-blockeditor/reference/game/change), [is touching](/makecode-blockeditor/reference/game/is-touching) [is touching edge](/makecode-blockeditor/reference/game/is-touching-edge),
[add score](/makecode-blockeditor/reference/game/add-score), [score](/makecode-blockeditor/reference/game/score), [set score](/makecode-blockeditor/reference/game/set-score),
[set life](/makecode-blockeditor/reference/game/set-life), [add life](/makecode-blockeditor/reference/game/add-life), [remove life](/makecode-blockeditor/reference/game/remove-life),
[start countdown](/makecode-blockeditor/reference/game/start-countdown), [game over](/makecode-blockeditor/reference/game/game-over),
[pause](/makecode-blockeditor/reference/game/pause), [resume](/makecode-blockeditor/reference/game/resume),
[is game over](/makecode-blockeditor/reference/game/is-game-over,) [is running](/makecode-blockeditor/reference/game/is-running), [is paused](/makecode-blockeditor/reference/game/is-paused)
