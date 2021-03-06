---
title: messages.getDialogUnreadMarks
description: Get dialogs manually marked as unread
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getDialogUnreadMarks.html
---
# Method: messages.getDialogUnreadMarks
[Back to methods index](index.md)



Get dialogs manually marked as unread



### Return type: [Vector\_of\_DialogPeer](../types/DialogPeer.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Vector_of_DialogPeer = $MadelineProto->messages->getDialogUnreadMarks();
```

Or, if you're into Lua:

```lua
Vector_of_DialogPeer = messages.getDialogUnreadMarks({})
```

