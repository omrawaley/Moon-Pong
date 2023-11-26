# Moon Pong
Moon Pong is a Pong clone made with Lua and LÖVE/Love2D. This is my first project with Lua and LÖVE.

<img width="400" alt="image" src="https://github.com/omrawaley/moon-pong/assets/133281331/35960afd-21cc-4e97-a7d1-3c3fbe319142">
<img width="400" alt="image" src="https://github.com/omrawaley/moon-pong/assets/133281331/5f484ed6-d520-49a1-a286-3ef99184b503">

It uses around 200MB of RAM.

## Customization
Modules are included that are useful to create multiple paddles, controlled via the keyboard or a the A.I.

The full list:
- `playerModule`
- `paddleModule`
- `keyboardPaddleLogicModule`
- `aiPaddleLogicModule`

The `playerModule` returns a table containing a `paddle` and a `paddleLogic`. The `paddle` can be initialized via the `paddleModule` and the `paddleLogic` can be initialized via the `keyboardPaddleLogicModule` or the `aiPaddleLogicModule`.

`paddleModule` stores the paddles data such as the location, velocity, etc. It excepts a single parameter for the `x` value of the paddle.

`keyboardPaddleLogicModule` allows the paddle to be controlled via the keyboard. It excepts a two parameters: the up and down key.

`aiPaddleLogicModule` allows the paddle to be controlled via the A.I. It excepts one parameter: difficulty. The higher the number you provide for this parameter, the easier the harder the A.I. will be. This is set at 7 by default.

The window resolution and such can be modified in the `conf.lua` file.

## Credits
Thanks to @Pharap for reviewing the code and making several design suggestions.
