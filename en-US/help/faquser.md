### ~~Users Frequently Asked Questions~~

#### ~~You can not subscribe to a list~~

~~This problem may be due to the following reasons:~~

-   ~~The list owners forgot to process your subscription request: to err is human, and your request might have been lost among many other messages! Resubmit your request before [contacting list owners directly](#contactadmin).~~
-   ~~Subscription to the list is reserved to a certain category of people. To know more, [contact list owners](#contactadmin).~~

#### ~~You can not log on to the mailing list web interface~~

~~This problem may be due to the following reasons:~~

-   ~~**You have no password**. To be given a password, follow the [First login?](%7B%7Bpath_cgi%7D%7D/firstpasswd) link from the homepage. You will receive your new password by email.~~
-   **You entered an incorrect password**. If you have forgotten your password, you can reset it. To do so, follow the [Lost password?](%7B%7Bpath_cgi%7D%7D/renewpasswd) link from the homepage.
-   ~~**You are not using the correct username** (the email address with which you are subscribed to the list).~~

| Note |
|------|
| ~~In order to avoid any mistake when typing your password, you can type it into another application (such as your email client) and copy and paste it into your web browser.~~ |

#### ~~You do not receive (all) messages sent to a list~~

~~This problem can have multiple reasons:~~

-   <span id="notsubscribedyet"></span>**~~You have never been subscribed to the list~~**:
    -   ~~Maybe you made a mistake in your email address when you tried to subscribe.~~
    -   ~~Maybe you are subscribed with an email address other than the one you are checking.~~
    -   ~~Maybe your subscription request was rejected by the list owners.~~

    ~~In any case, try and [subscribe](user.md#subscribe) again.~~
-   <span id="notsubscribedanymore"></span>**~~You are not subscribed to the list anymore~~**:
    -   ~~If your address has been bouncing for a while, you might have been automatically unsubscribed by the system (or even by the list owners). Try and [subscribe again](user.md#subscribe) after ensuring that your email address will not be in trouble again.~~
    -   ~~If you have not respected the different rules applying to the mailing list, the list owners might have "banned" you...~~
    -   ~~You might also have been arbitrarily unsubscribed by an ill-intentioned person, in case the list is not configured to send a confirmation request for any subscription and unsubscription request... In that case, try and [subscribe](user.md#subscribe) again.~~
-   ~~**Your [delivery mode](user.md#deliverymode) does not allow you to receive messages**: for example, it is the case with the 'Nomail' delivery mode.~~
-   ~~**Your inbox is full**. Be careful: when your inbox is not completely full, you receive only small messages, which makes it difficult to understand what actually is the problem... Furthermore, if your email address causes trouble on a regular basis, you might be unsubscribed by the list owners or by the system. Thus, you should clean your inbox frequently.~~
-   ~~**Your inbox is subject to some restrictions**: it does not allow you to receive messages with attachments, bans some types of attachments or limits the maximum size of incoming messages; in that case, we advise you to choose the [Urlize delivery mode](user.md#deliverymode).~~

#### ~~You can not send messages to a list~~

~~This problem can have multiple reasons:~~

-   ~~**You have [never been subscribed](#notsubscribedyet)** to the list.~~
-   ~~**You are [not subscribed to the list anymore](#notsubscribedanymore)**.~~
-   ~~**You are using another address** than the one with which you are subscribed to the list.~~
-   ~~**If the list is a moderated list, the distribution of the message depends on the moderators' availability**: they can not monitor the list night and day! Thus the distribution of your message might be a bit delayed.~~
-   ~~**If the list is a moderated list, your message might have been rejected by a moderator**. In case you received no notice, you can possibly send a message to nameofthelist-request@{{conf.host}} to ask for an explanation.~~
-   ~~**The message you are trying to send does not fulfill the conditions to be distributed** on the list: it may be too large, contain a forbidden type of attachment or even contain any type of attachment (in case attachments are forbidden on the list).~~
-   ~~**The problem may also come from your email account**:~~
    -   ~~The mail server is temporarily unavailable.~~
    -   ~~Your inbox is full and it prevents you from sending new messages.~~
    -   ~~Your inbox is subject to some restrictions: it does not allow you to send messages with attachments, bans some types of attachments or limits the maximum size of outgoing messages.~~
-   ~~Last, **you might have made a mistake in the list address** when sending your message!~~

#### ~~You can not unsubscribe from a list~~

~~This problem can have multiple reasons:~~

-   ~~**You are using another address** than the one with which you are subscribed to the list.~~
-   ~~**You are subscribed through a dynamic data source** (examples: databases, LDAP directories, etc.) which does not allow you to unsubscribe. [Contact the list owners](#contactadmin) to know more about this.~~
-   ~~**The list owners forgot to process your unsubscription request**: to err is human, and your request might have been lost among many other messages! Resubmit your request before [contacting list owners directly](#contactadmin).~~

#### <span id="contactadmin"></span>~~You want to contact list owners~~

~~The list owners and moderators' names are mentioned in the left menu. However, you should never write directly to a list owner or moderator: first, the person to whom you are writing might be absent, and furthermore, it is better to inform all owners and moderators of your request. When you have a question or remark, **the address you should write to is: nameofthelist-request@{{conf.host}}** (replace 'nameofthelist' by the name of the list).~~
