---
title: help.getAppConfig
description: Get app-specific configuration, see [client configuration](https://core.telegram.org/api/config#client-configuration) for more info on the result.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/help_getAppConfig.html
---
# Method: help.getAppConfig
[Back to methods index](index.md)



Get app-specific configuration, see [client configuration](https://core.telegram.org/api/config#client-configuration) for more info on the result.



### Return type: [JSONValue](../types/JSONValue.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$JSONValue = $MadelineProto->help->getAppConfig();
```

Or, if you're into Lua:

```lua
JSONValue = help.getAppConfig({})
```

