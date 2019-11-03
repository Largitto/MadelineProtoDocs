---
title: document
description: Document
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: document  
[Back to constructors index](index.md)



Document

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[long](../types/long.md) | Yes|ID|
|access\_hash|[long](../types/long.md) | Yes|Access hash|
|file\_reference|[bytes](../types/bytes.md) | Yes|File reference|
|date|[int](../types/int.md) | Yes|Date|
|mime\_type|[string](../types/string.md) | Yes|Mime type|
|size|[int](../types/int.md) | Yes|Size|
|thumbs|Array of [PhotoSize](../types/PhotoSize.md) | Optional|Thumbnails|
|dc\_id|[int](../types/int.md) | Yes|DC ID|
|attributes|Array of [DocumentAttribute](../types/DocumentAttribute.md) | Yes|Attributes|



### Type: [Document](../types/Document.md)


### Example:

```php
$document = ['_' => 'document', 'id' => long, 'access_hash' => long, 'file_reference' => 'bytes', 'date' => int, 'mime_type' => 'string', 'size' => int, 'thumbs' => [PhotoSize, PhotoSize], 'dc_id' => int, 'attributes' => [DocumentAttribute, DocumentAttribute]];
```  


Or, if you're into Lua:

```lua
document={_='document', id=long, access_hash=long, file_reference='bytes', date=int, mime_type='string', size=int, thumbs={PhotoSize}, dc_id=int, attributes={DocumentAttribute}}

```

