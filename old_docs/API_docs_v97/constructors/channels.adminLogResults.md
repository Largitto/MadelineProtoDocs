---
title: channels.adminLogResults
description: Admin log events
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/channels_adminLogResults.html
---
# Constructor: channels.adminLogResults  
[Back to constructors index](index.md)



Admin log events

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|events|Array of [ChannelAdminLogEvent](../types/ChannelAdminLogEvent.md) | Yes|Events|
|chats|Array of [Chat](../types/Chat.md) | Yes|Chats|
|users|Array of [User](../types/User.md) | Yes|Users|



### Type: [channels.AdminLogResults](../types/channels.AdminLogResults.md)


### Example:

```php
$channels.adminLogResults = ['_' => 'channels.adminLogResults', 'events' => [ChannelAdminLogEvent, ChannelAdminLogEvent], 'chats' => [Chat, Chat], 'users' => [User, User]];
```  


Or, if you're into Lua:

```lua
channels.adminLogResults={_='channels.adminLogResults', events={ChannelAdminLogEvent}, chats={Chat}, users={User}}

```


