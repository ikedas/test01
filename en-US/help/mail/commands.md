~~List of the commands of the Sympa mail interface~~
----------------------------------------------------

~~All commands are to be sent at {{conf.email}}@{{conf.host}}.~~

~~It is possible to send several commands in a single message. Commands are to be entered in the message body (one command per line).~~

### ~~Commands for users~~

~~`HELP`: receive a list of all available commands~~

~~`LISTS`: receive a list of all lists managed on the server~~

~~`WHICH`: receive a list of all lists to which you are subscribed~~

~~`CONFIRM key`: confirm sending of a message (according to the way the list is configured)~~

~~`QUIT`: indicates the end of the commands (used to ignore a signature)~~

~~`INFO list`: get information about the list~~

~~`REVIEW list`: receive a list of all list members~~

~~`SUBSCRIBE list name`: subscription (or subscription confirmation) to the list~~

~~`INVITE list email`: invite someone to subscribe to the list~~

~~`UNSUBSCRIBE list email`: unsubscribe from the list. The email address is required only if you want to unsubscribe with an address other than the address with which you send the message~~

~~`UNSUBSCRIBE * email`: unsubscribe from all the lists to which you are subscribed~~

~~`SET list NOMAIL`: suspend receipt of the list's messages~~

~~`SET list DIGEST`: receive messages in digest mode~~

~~`SET list DIGESTPLAIN`: receive messages in digest mode (plain text)~~

~~`SET list SUMMARY`: only receive the message list~~

~~`SET list NOTICE`: only receive the message subjects~~

~~`SET list MAIL`: normal message delivery mode~~

~~`SET list CONCEAL`: become unlisted (hidden subscriber address)~~

~~`SET list NOCONCEAL`: subscriber address visible via REView~~

~~`INDEX list`: receive the list of the archive files~~

~~`GET list file`: receive a file of the list archive~~

~~`LAST list`: receive the list's most recent message~~

### ~~Commands for list owners~~

~~`ADD list email name`: add a member to the list~~

~~`DEL list email`: remove a subscriber from the list~~

~~`STATS list`: check the statistics for the list~~

&lt;~~code&gt;REMIND *list*: send to all subscribers a personalized reminder with the address with which he/she is subscribed to the list~~

### ~~Commands for list moderators~~

~~`DISTRIBUTE list key`: approve of a message~~

~~`REJECT list key`: reject a message to be moderated~~

~~`MODINDEX list`: check the list of messages to be moderated~~
