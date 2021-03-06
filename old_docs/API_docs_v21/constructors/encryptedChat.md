---
title: encryptedChat
description: Encrypted chat
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: encryptedChat  
[Back to constructors index](index.md)



Encrypted chat

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|Chat ID|
|access\_hash|[long](../types/long.md) | Yes|Check sum dependant on the user ID|
|date|[int](../types/int.md) | Yes|Date chat was created|
|admin\_id|[int](../types/int.md) | Yes|Chat creator ID|
|participant\_id|[int](../types/int.md) | Yes|ID of the second chat participant|
|g\_a\_or\_b|[bytes](../types/bytes.md) | Yes|`B = g ^ b mod p`, if the currently authorized user is the chat's creator,<br>or `A = g ^ a mod p` otherwise<br>See [Wikipedia](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) for more info|
|key\_fingerprint|[long](../types/long.md) | Yes|64-bit fingerprint of received key|



### Type: [EncryptedChat](../types/EncryptedChat.md)


### Example:

```php
$encryptedChat = ['_' => 'encryptedChat', 'id' => int, 'access_hash' => long, 'date' => int, 'admin_id' => int, 'participant_id' => int, 'g_a_or_b' => 'bytes', 'key_fingerprint' => long];
```  


Or, if you're into Lua:

```lua
encryptedChat={_='encryptedChat', id=int, access_hash=long, date=int, admin_id=int, participant_id=int, g_a_or_b='bytes', key_fingerprint=long}

```


