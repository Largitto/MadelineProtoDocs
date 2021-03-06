---
title: updateChannelWebPage
description: A webpage preview of a link in a [channel/supergroup](https://core.telegram.org/api/channel) message was generated
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateChannelWebPage  
[Back to constructors index](index.md)



A webpage preview of a link in a [channel/supergroup](https://core.telegram.org/api/channel) message was generated

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|channel\_id|[int](../types/int.md) | Yes|[Channel/supergroup](https://core.telegram.org/api/channel) ID|
|webpage|[WebPage](../types/WebPage.md) | Optional|Generated webpage preview|
|pts|[int](../types/int.md) | Yes|[Event count after generation](https://core.telegram.org/api/updates)|
|pts\_count|[int](../types/int.md) | Yes|[Number of events that were generated](https://core.telegram.org/api/updates)|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateChannelWebPage = ['_' => 'updateChannelWebPage', 'channel_id' => int, 'webpage' => WebPage, 'pts' => int, 'pts_count' => int];
```  


Or, if you're into Lua:

```lua
updateChannelWebPage={_='updateChannelWebPage', channel_id=int, webpage=WebPage, pts=int, pts_count=int}

```


