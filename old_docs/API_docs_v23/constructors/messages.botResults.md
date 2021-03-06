---
title: messages.botResults
description: Result of a query to an inline bot
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/messages_botResults.html
---
# Constructor: messages.botResults  
[Back to constructors index](index.md)



Result of a query to an inline bot

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|gallery|[Bool](../types/Bool.md) | Optional|Whether the result is a picture gallery|
|query\_id|[long](../types/long.md) | Yes|Query ID|
|next\_offset|[string](../types/string.md) | Optional|The next offset to use when navigating through results|
|switch\_pm|[InlineBotSwitchPM](../types/InlineBotSwitchPM.md) | Optional|Whether the bot requested the user to message him in private|
|results|Array of [BotInlineResult](../types/BotInlineResult.md) | Yes|The results|
|cache\_time|[int](../types/int.md) | Yes|Caching validity of the results|
|users|Array of [User](../types/User.md) | Yes|Users mentioned in the results|



### Type: [messages.BotResults](../types/messages.BotResults.md)


### Example:

```php
$messages.botResults = ['_' => 'messages.botResults', 'gallery' => Bool, 'query_id' => long, 'next_offset' => 'string', 'switch_pm' => InlineBotSwitchPM, 'results' => [BotInlineResult, BotInlineResult], 'cache_time' => int, 'users' => [User, User]];
```  


Or, if you're into Lua:

```lua
messages.botResults={_='messages.botResults', gallery=Bool, query_id=long, next_offset='string', switch_pm=InlineBotSwitchPM, results={BotInlineResult}, cache_time=int, users={User}}

```


