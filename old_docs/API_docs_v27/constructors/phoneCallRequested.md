---
title: phoneCallRequested
description: Requested phone call
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: phoneCallRequested  
[Back to constructors index](index.md)



Requested phone call

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[long](../types/long.md) | Yes|Phone call ID|
|access\_hash|[long](../types/long.md) | Yes|Access hash|
|date|[int](../types/int.md) | Yes|When was the phone call created|
|admin\_id|[int](../types/int.md) | Yes|ID of the creator of the phone call|
|participant\_id|[int](../types/int.md) | Yes|ID of the other participant of the phone call|
|g\_a\_hash|[bytes](../types/bytes.md) | Yes|[Parameter for key exchange](https://core.telegram.org/api/end-to-end/voice-calls)|
|protocol|[PhoneCallProtocol](../types/PhoneCallProtocol.md) | Yes|Call protocol info to be passed to libtgvoip|



### Type: [PhoneCall](../types/PhoneCall.md)


### Example:

```php
$phoneCallRequested = ['_' => 'phoneCallRequested', 'id' => long, 'access_hash' => long, 'date' => int, 'admin_id' => int, 'participant_id' => int, 'g_a_hash' => 'bytes', 'protocol' => PhoneCallProtocol];
```  


Or, if you're into Lua:

```lua
phoneCallRequested={_='phoneCallRequested', id=long, access_hash=long, date=int, admin_id=int, participant_id=int, g_a_hash='bytes', protocol=PhoneCallProtocol}

```


