---
title: inputMediaGame
description: A game
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputMediaGame  
[Back to constructors index](index.md)



A game

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[InputGame](../types/InputGame.md) | Yes|The game to forward|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```php
$inputMediaGame = ['_' => 'inputMediaGame', 'id' => InputGame];
```  


Or, if you're into Lua:

```lua
inputMediaGame={_='inputMediaGame', id=InputGame}

```


