---
title: messages.setBotShippingResults
description: If you sent an invoice requesting a shipping address and the parameter is\_flexible was specified, the bot will receive an [updateBotShippingQuery](../constructors/updateBotShippingQuery.md) update. Use this method to reply to shipping queries.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_setBotShippingResults.html
---
# Method: messages.setBotShippingResults  
[Back to methods index](index.md)


If you sent an invoice requesting a shipping address and the parameter is\_flexible was specified, the bot will receive an [updateBotShippingQuery](../constructors/updateBotShippingQuery.md) update. Use this method to reply to shipping queries.

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|query\_id|[long](../types/long.md) | Unique identifier for the query to be answered | Yes|
|error|[string](../types/string.md) | Error message in human readable form that explains why it is impossible to complete the order (e.g. "Sorry, delivery to your desired address is unavailable'). Telegram will display this message to the user. | Optional|
|shipping\_options|Array of [ShippingOption](../types/ShippingOption.md) | Shipping options | Optional|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->setBotShippingResults(['query_id' => long, 'error' => 'string', 'shipping_options' => [ShippingOption, ShippingOption], ]);
```

Or, if you're into Lua:

```lua
Bool = messages.setBotShippingResults({query_id=long, error='string', shipping_options={ShippingOption}, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|QUERY_ID_INVALID|The query ID is invalid|


