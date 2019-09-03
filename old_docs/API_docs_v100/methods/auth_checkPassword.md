---
title: auth.checkPassword
description: You cannot use this method directly, use the complete_2fa_login method instead (see https://docs.madelineproto.xyz for more info)
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: auth.checkPassword  
[Back to methods index](index.md)


You cannot use this method directly, use the complete_2fa_login method instead (see https://docs.madelineproto.xyz for more info)

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|password|[InputCheckPasswordSRP](../types/InputCheckPasswordSRP.md) | You cannot use this method directly, use the complete_2fa_login method instead (see https://docs.madelineproto.xyz for more info) | Yes|


### Return type: [auth\_Authorization](../types/auth_Authorization.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$auth_Authorization = $MadelineProto->auth->checkPassword(['password' => InputCheckPasswordSRP, ]);
```

Or, if you're into Lua:

```lua
auth_Authorization = auth.checkPassword({password=InputCheckPasswordSRP, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|PASSWORD_HASH_INVALID|The provided password hash is invalid|

