---
title: messages.getStickers
description: Get stickers by emoji
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getStickers.html
---
# Method: messages.getStickers
[Back to methods index](index.md)



Get stickers by emoji

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|emoticon|[string](../types/string.md) | The emoji | Yes|
|hash|Array of [int](../types/int.md) | [Hash for pagination, for more info click here](https://core.telegram.org/api/offsets#hash-generation) | Optional|


### Return type: [messages.Stickers](../types/messages.Stickers.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages.Stickers = $MadelineProto->messages->getStickers(['emoticon' => 'string', 'hash' => [int, int], ]);
```

Or, if you're into Lua:

```lua
messages.Stickers = messages.getStickers({emoticon='string', hash={int}, })
```

