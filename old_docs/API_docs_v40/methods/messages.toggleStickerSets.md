---
title: messages.toggleStickerSets
description: Apply changes to multiple stickersets
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_toggleStickerSets.html
---
# Method: messages.toggleStickerSets
[Back to methods index](index.md)



Apply changes to multiple stickersets

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|uninstall|[Bool](../types/Bool.md) | Uninstall the specified stickersets | Optional|
|archive|[Bool](../types/Bool.md) | Archive the specified stickersets | Optional|
|unarchive|[Bool](../types/Bool.md) | Unarchive the specified stickersets | Optional|
|stickersets|Array of [InputStickerSet](../types/InputStickerSet.md) | Stickersets to act upon | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->toggleStickerSets(['uninstall' => Bool, 'archive' => Bool, 'unarchive' => Bool, 'stickersets' => [InputStickerSet, InputStickerSet], ]);
```

Or, if you're into Lua:

```lua
Bool = messages.toggleStickerSets({uninstall=Bool, archive=Bool, unarchive=Bool, stickersets={InputStickerSet}, })
```

