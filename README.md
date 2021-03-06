# jquery-snake-game
jQuery plugin that provides a classic snake game.

Requires pstrinkle/jquery-paintbox


Plans
-----

See issues.

Usage
-----
```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
<script src="/libs/jquery-paintbox/dist/jquery.paintbox.js"></script>
<script src="/libs/jquery-snake-game/dist/jquery.snake-game.js"></script>

<div id='container'></div>

<script>
    $('#container').snakeGame({});
</script>
```

Options
-------
You should specify options like in usage example above.

| Name | Type | Default | Description |
| ---- | ---- | ---- | ---- |
| rows | integer | `50` | Number of rows. |
| cols | integer | `50` | Number of columns. |
| speed | integer | `100` | Speed of movement in milliseconds. |
| snakeColor | css string | `blue` | Color of the snake. |
| foodColor | css string | `red` | Color of the food. |
| startLength | integer | `1` | Starting length of the snake. |
| cornerFood | boolean | `true` | Can food spawn in the corner? |
| wallFood | boolean | `true` | Can food spawn against the outer wall? |
| onPoint | callback | `null` | Function called with single parameter, the score increase. |
| onGameOver | callback | `null` | Function called when the game ends. |

Methods
-------
There are a few methods to programmatically change the painting.

| Method | Param | Type | Description |
| ---- | ---- | ---- | ---- |
| `start` | |  | Start the game! |
| `turn` | direction | string | turn the snake, `left, right, up, down` |

License
-------
[Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)



