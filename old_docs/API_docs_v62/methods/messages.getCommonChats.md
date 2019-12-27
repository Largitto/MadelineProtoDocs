---
title: messages.getCommonChats
description: Get chats in common with a user
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getCommonChats  
[Back to methods index](index.md)


Get chats in common with a user

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|user\_id|[Username, chat ID, Update, Message or InputUser](../types/InputUser.md) | User ID | Optional|
|max\_id|[int](../types/int.md) | Maximum ID of chat to return (see [pagination](https://core.telegram.org/api/offsets)) | Yes|
|limit|[int](../types/int.md) | Maximum number of results to return, [see pagination](https://core.telegram.org/api/offsets) | Yes|


### Return type: [messages\_Chats](../types/messages_Chats.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_Chats = $MadelineProto->messages->getCommonChats(['user_id' => InputUser, 'max_id' => int, 'limit' => int, ]);
```

Or, if you're into Lua:

```lua
messages_Chats = messages.getCommonChats({user_id=InputUser, max_id=int, limit=int, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|USER_ID_INVALID|The provided user ID is invalid|

