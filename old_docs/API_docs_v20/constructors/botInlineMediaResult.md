---
title: botInlineMediaResult
description: Media result
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: botInlineMediaResult  
[Back to constructors index](index.md)



Media result

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[string](../types/string.md) | Yes|Result ID|
|type|[string](../types/string.md) | Yes|Result type (see [bot API docs](https://core.telegram.org/bots/api#inlinequeryresult))|
|photo|[Photo](../types/Photo.md) | Optional|If type is `photo`, the photo to send|
|document|[Document](../types/Document.md) | Optional|If type is `document`, the document to send|
|title|[string](../types/string.md) | Optional|Result title|
|description|[string](../types/string.md) | Optional|Description|
|send\_message|[BotInlineMessage](../types/BotInlineMessage.md) | Yes|Depending on the `type` and on the [constructor](../types/BotInlineMessage.md), contains the caption of the media or the content of the message to be sent **instead** of the media|



### Type: [BotInlineResult](../types/BotInlineResult.md)


### Example:

```php
$botInlineMediaResult = ['_' => 'botInlineMediaResult', 'id' => 'string', 'type' => 'string', 'photo' => Photo, 'document' => Document, 'title' => 'string', 'description' => 'string', 'send_message' => BotInlineMessage];
```  


Or, if you're into Lua:

```lua
botInlineMediaResult={_='botInlineMediaResult', id='string', type='string', photo=Photo, document=Document, title='string', description='string', send_message=BotInlineMessage}

```


