---
title: User
description: constructors and methods of type User
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Type: User
[Back to types index](index.md)

You can directly provide the [Update](Update.md) or [Message](Message.md) object here, MadelineProto will automatically extract the destination chat id.

The following syntaxes can also be used:

```php
$User = '@username'; // Username

$User = 'me'; // The currently logged-in user

$User = 44700; // bot API id (users)
$User = -492772765; // bot API id (chats)
$User = -10038575794; // bot API id (channels)

$User = 'https://t.me/danogentili'; // t.me URLs
$User = 'https://t.me/joinchat/asfln1-21fa_'; // t.me invite links

$User = 'user#44700'; // tg-cli style id (users)
$User = 'chat#492772765'; // tg-cli style id (chats)
$User = 'channel#38575794'; // tg-cli style id (channels)
```

A [Chat](Chat.md), a [User](User.md), an [InputPeer](InputPeer.md), an [InputDialogPeer](InputDialogPeer.md), an [InputNotifyPeer](InputNotifyPeer.md), an [InputUser](InputUser.md), an [InputChannel](InputChannel.md), a [Peer](Peer.md), an [DialogPeer](DialogPeer.md), [NotifyPeer](NotifyPeer.md), or a [Chat](Chat.md) object can also be used.




### Possible values (constructors):

[userEmpty](../constructors/userEmpty.md)  

[user](../constructors/user.md)  



### Methods that return an object of this type (methods):

[$MadelineProto->account->updateProfile](../methods/account.updateProfile.md)  

[$MadelineProto->account->updateUsername](../methods/account.updateUsername.md)  

[$MadelineProto->account->changePhone](../methods/account.changePhone.md)  

[$MadelineProto->users->getUsers](../methods/users.getUsers.md)  

[$MadelineProto->contacts->importCard](../methods/contacts.importCard.md)  



[userEmpty](../constructors/userEmpty.md)  

[user](../constructors/user.md)  

[$MadelineProto->account->updateProfile](../methods/account.updateProfile.md)  

[$MadelineProto->account->updateUsername](../methods/account.updateUsername.md)  

[$MadelineProto->account->changePhone](../methods/account.changePhone.md)  

[$MadelineProto->users->getUsers](../methods/users.getUsers.md)  

[$MadelineProto->contacts->importCard](../methods/contacts.importCard.md)  

