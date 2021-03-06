---
title: updateDcOptions
description: Changes in the data center configuration options.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateDcOptions  
[Back to constructors index](index.md)



Changes in the data center configuration options.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|dc\_options|Array of [DcOption](../types/DcOption.md) | Yes|New connection options|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateDcOptions = ['_' => 'updateDcOptions', 'dc_options' => [DcOption, DcOption]];
```  


Or, if you're into Lua:

```lua
updateDcOptions={_='updateDcOptions', dc_options={DcOption}}

```


