---
title: payments.savedInfo
description: Saved server-side order information
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/payments_savedInfo.html
---
# Constructor: payments.savedInfo  
[Back to constructors index](index.md)



Saved server-side order information

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|has\_saved\_credentials|[Bool](../types/Bool.md) | Optional|Whether the user has some saved payment credentials|
|saved\_info|[PaymentRequestedInfo](../types/PaymentRequestedInfo.md) | Optional|Saved server-side order information|



### Type: [payments.SavedInfo](../types/payments.SavedInfo.md)


### Example:

```php
$payments.savedInfo = ['_' => 'payments.savedInfo', 'has_saved_credentials' => Bool, 'saved_info' => PaymentRequestedInfo];
```  


Or, if you're into Lua:

```lua
payments.savedInfo={_='payments.savedInfo', has_saved_credentials=Bool, saved_info=PaymentRequestedInfo}

```


