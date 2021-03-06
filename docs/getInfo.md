---
title: getInfo
description: getInfo parameters, return type and example
redirect_from: /get_info.html
---
## Method: getInfo  


### Parameters:

| Name     |    Type       |
|----------|---------------|
|id| A username, a bot API chat id, a tg-cli chat id, a [Chat](API_docs/types/Chat.md), a [User](API_docs/types/User.md), an [InputPeer](API_docs/types/InputPeer.md), an [InputUser](API_docs/types/InputUser.md), an [InputChannel](API_docs/types/InputChannel.md), a [Peer](API_docs/types/Peer.md), or a [Chat](API_docs/types/Chat.md) object|

### Return type: [Info](Info.md)

### Example ([now fully async!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
$Chat = yield $MadelineProto->getInfo($id);
```

Or, if you're into Lua:

```lua
Chat = getInfo(id)
```

