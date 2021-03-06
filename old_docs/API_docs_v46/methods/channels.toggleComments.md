---
title: channels.toggleComments
description: Enable channel comments
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/channels_toggleComments.html
---
# Method: channels.toggleComments  
[Back to methods index](index.md)


Enable channel comments

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|channel|[Username, chat ID, Update, Message or InputChannel](../types/InputChannel.md) | The channel  | Optional|
|enabled|[Bool](../types/Bool.md) | Enable or disable comments | Yes|


### Return type: [Updates](../types/Updates.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->channels->toggleComments(['channel' => InputChannel, 'enabled' => Bool, ]);
```

Or, if you're into Lua:

```lua
Updates = channels.toggleComments({channel=InputChannel, enabled=Bool, })
```

