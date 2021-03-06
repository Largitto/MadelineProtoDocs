---
title: auth.sendCode
description: You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info)
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/auth_sendCode.html
---
# Method: auth.sendCode  
[Back to methods index](index.md)


You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info)

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|phone\_number|[string](../types/string.md) | You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info) | Yes|
|sms\_type|[int](../types/int.md) | You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info) | Yes|
|api\_id|[int](../types/int.md) | You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info) | Yes|
|api\_hash|[string](../types/string.md) | You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info) | Yes|
|lang\_code|[string](../types/string.md) | You cannot use this method directly, use the phoneLogin method instead (see https://docs.madelineproto.xyz for more info) | Yes|


### Return type: [auth.SentCode](../types/auth.SentCode.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$auth.SentCode = $MadelineProto->auth->sendCode(['phone_number' => 'string', 'sms_type' => int, 'api_id' => int, 'api_hash' => 'string', 'lang_code' => 'string', ]);
```

Or, if you're into Lua:

```lua
auth.SentCode = auth.sendCode({phone_number='string', sms_type=int, api_id=int, api_hash='string', lang_code='string', })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|API_ID_INVALID|API ID invalid|
|400|API_ID_PUBLISHED_FLOOD|This API id was published somewhere, you can't use it now|
|400|INPUT_REQUEST_TOO_LONG|The request is too big|
|400|PHONE_NUMBER_APP_SIGNUP_FORBIDDEN|You can't sign up using this app|
|400|PHONE_NUMBER_BANNED|The provided phone number is banned from telegram|
|400|PHONE_NUMBER_FLOOD|You asked for the code too many times.|
|400|PHONE_NUMBER_INVALID|The phone number is invalid|
|400|PHONE_PASSWORD_PROTECTED|This phone is password protected|
|400|SMS_CODE_CREATE_FAILED|An error occurred while creating the SMS code|
|406|PHONE_NUMBER_INVALID|The phone number is invalid|
|406|PHONE_PASSWORD_FLOOD|You have tried logging in too many times|


