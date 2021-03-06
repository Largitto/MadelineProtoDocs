---
title: updateNewMessage
description: New message.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateNewMessage  
[Back to constructors index](index.md)



New message.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|message|[Message](../types/Message.md) | Optional|Message|
|pts|[int](../types/int.md) | Yes|New quantity of actions in a message box|
|pts\_count|[int](../types/int.md) | Yes|Number of generated events|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateNewMessage = ['_' => 'updateNewMessage', 'message' => Message, 'pts' => int, 'pts_count' => int];
```  


Or, if you're into Lua:

```lua
updateNewMessage={_='updateNewMessage', message=Message, pts=int, pts_count=int}

```


