~~Mailing lists - User Guide~~
------------------------------

### <span id="howitworks"></span>~~How the mailing list service works~~

~~The mailing-list service is managed by a **mailing-list software: Sympa**. This software comes with a **web mailing list environment**.~~

~~To perform actions related to mailing lists (subscribe, change your options, etc.), you have two options:~~

-   ~~**log on to the web environment**;~~
-   ~~**send commands by email** to the Sympa mailing list manager at **{{conf.email}}@{{conf.host}}**.~~

~~**To send a command to Sympa**, do as follows:~~

-   ~~**If you send a single command**, type it into the subject line of your email and leave its body blank.~~
-   ~~**If you send several commands**, leave the subject line of your email blank and type all the commands in the email body. **Be careful**: Sympa will not process your message unless you respect the following rules:~~
    -   ~~Write every command on a new line.~~
    -   ~~Send your message in plain text, not in HTML (no formatting).~~
    -   ~~Your message can not contain anything else than Sympa commands (no signature block).~~

~~A description of all the commands you can send to Sympa is available at [file:///help/mail\_commands](mail_commands.md).~~

### <span id="subscribe"></span>~~Subscribing to mailing lists~~

~~Subscribing to a mailing list is very simple:~~

1.  **~~Choose the address with which you want to subscribe to the list.~~
    **

    | Note |
    |------|
    | ~~You should choose an address you can check frequently and which offers a large storage capacity for your email: some lists distribute many messages, which sometimes contain large attachments.~~ |

    | Note |
    |------|
    | ~~Of course you can subscribe to the same list with several email addresses. Then you will need to redo the whole process with a different email address.~~ |

2.  ~~Send a **message to {{conf.email}}@{{conf.host}}** from the address you want to subscribe to the list.~~

    | Note |
    |------|
    | ~~Sympa is not a person but a mailing list management robot. Thus it is useless to send it loving words! ;-)~~ |

3.  ~~In the subject line of your message, type in: **subscribe nameofthelist Firstname Name** (replace 'nameofthelist' by the name of the list you want to subscribe to and indicate your own first name and name).~~
4.  ~~**Leave the message body blank**.~~

    | Note |
    |------|
    | ~~To save some time, you can also send several commands in a single message. To do that, follow the instructions available in the [How the mailing list service works](#howitworks) section.~~ |

~~**After this, you will receive a message telling you whether your request was accepted or not**: if the subscription to the list is subject to any approval, the list owner may choose not to subscribe you. If so, do not send several other requests: it is useless as the result will remain the same. You can possibly send a message directly to the list owner (nameofthelist-request@{{conf.host}}) to explain why you really want to subscribe to the list...~~

| Note |
|------|
| ~~Note: you will sometimes be asked to confirm your subscription request before it can be processed. If so, please conform to the instructions contained in the message you receive.~~ |

~~According to the type of list (list with subscription subject to conditions or not) and to the availability of the list owner, **you may not receive the notice immediately**. It is useless to send several requests.~~

~~**If your request is accepted, the message you receive confirms your subscription to the list. This message** (the list Charter) **contains several pieces of essential information:**~~

-   ~~your **list password**. This password is the same for all the lists you subscribed to with a single email address. You can [change it online](#global_pref "How to change your password") after logging on to the mailing list environment;~~
-   ~~**detailed information about the list**: its purpose, the Internet address at which the message archive is available, etc.~~
-   ~~the **rules applying to the list and its members**: allowed and forbidden topics, netiquette, legal information, privacy policy, etc.~~

~~**You should keep your subscription notice**: you may need it later to remember your password or to send a precise command to Sympa (example: signoff command). More generally, **we advise you to keep all your subscription notices to mailing lists**.~~

~~**You can also subscribe to a list through the mailing list web interface**. To do that, do as follows:~~

1.  ~~Go to the list environment **[homepage](%7B%7Bpath_cgi%7D%7D/home)** and **log on**.~~
2.  ~~**Go to the information page of the list** you want to subscribe to.~~
3.  ~~In the left menu, **click on the 'Subscribe'** link.~~

### <span id="sympa_auth"></span>~~Logging on to the mailing list environment~~

~~To log on to the mailing list environment, use the authentication form displayed on top of the left column of the web interface. When you are logged on, your email address and user profile (subscriber, moderator or owner) are displayed there.~~

~~The authentication process varies according to your personal situation:~~

-   ~~**If the organization offering the mailing list service uses single sign-on technology** (unique account and unique authentication, for example through the CAS system), you will preferably log on with your unique account. To do that, click on the 'Go' button next to the text '**Authentication \[name of the system used\]**'. Then, type in your login and password to log on to the authentication server.~~

    | Note |
    |------|
    | ~~If you have already logged on to another service using the unique authentication system, your authentication is automatic. Refresh page if necessary.~~ |

-   **If the unique authentication process does not apply to you but you are already subscribed to lists**, then you have been granted a list password (displayed in the list Charter you got when you subscribed to the list). In this case, log on through the classic method: enter the **email address with which you subscribed to the list** as a login and your **list password** in the 'Password' field.

    | Note |
    |------|
    | If you do not remember your list password, click on 'Lost password ?'. Then enter your email address and password. Shortly afterward you will receive an email with a validation link. |

-   **If the unique authentication process does not apply to you and you do not have a list password yet**, click on '**First login?**' and type in your email address. A confirmation URL will be sent to that address. Then you will be able to choose your password.

| Note |
|------|
| ~~Remember: the list password is a special password you will only use for the mailing list service.~~ |

### ~~Checking your subscriptions~~

~~To see all the lists you subscribed to, you need to [log on](#sympa_auth) first. Then a list of all your lists, including a short description for each of them, will be displayed in the 'Your lists' form on the left column.~~

~~**To look at a list information page, click on its name**. The information page includes a description of the list (object, rules applying when sending a message, etc.), which length varies according to the list.~~

~~Form this information page, you can:~~

-   ~~change your [subscriber options](#options);~~
-   ~~read the [list archive](arc.md);~~
-   ~~[search in the message archive](arc.md#arcsearch);~~
-   ~~[send new messages](sendmsg.md);~~
-   ~~[download documents](shared.md#shared_read) from the shared document web space;~~
-   ~~[upload documents](shared.md#shared_upload) in the shared document web space;~~
-   ~~[review members](#subscribers) of the list (if available);~~
-   ~~[suspend or resume](suspend.md) your subscription of each list;~~
-   ~~[unsubscribe](#unsubscribe) from the list.~~

<span id="subscribers"></span>~~The **number of people subscribed** to the list is permanently displayed in the **left menu**. **To review the list members, click on the 'Review members' link** in the left menu (if the list-owner decided to deny access to the members list, this link is not available). The subscribers list displays and shows the **email address** and **name** of each of the subscribers (the indication of the name depends on the subscription method used by the subscribers).~~

| Note |
|------|
| ~~By default, each page displays 25 subscribers. You can browse through the pages by using the browsing arrows or display more subscribers per page. You may also wish to sort subscribers according to their email address, domain or name by clicking on the corresponding column header.~~ |

~~**The names of the list owners and moderators are displayed in the left menu**. You should never write directly to a list owner or moderator. If you want to ask a question or make a comment, you should use the following address: **nameofthelist-request@{{conf.host}}** (replace 'nameofthelist' by the name of the list in question).~~

~~To know **when you subscribed to the list** and **when you last updated your subscriber options**, **click on the 'Subscriber options' link** in the left menu.~~

### <span id="pref"></span>~~Managing your preferences~~

~~To allow you to **use lists more easily**, **you can define a number of personal preferences**. There are two types of preferences you can change:~~

-   ~~your **subscriber options**, which can vary according to the list;~~
-   ~~your **general preferences**, which apply to the entire Sympa mailing list environment.~~

#### <span id="options"></span>~~Changing your subscriber options~~

~~**Your subscriber options can vary from a list to another**. To change them, do as follows:~~

1.  ~~Go to the list environment **[homepage](%7B%7Bpath_cgi%7D%7D/home)** and **log on**.~~
2.  ~~**Go to the information page of the list** for which you want to change your subscriber options.~~
3.  ~~In the left menu, **click on the 'Subscriber options' link**.~~
4.  <span id="deliverymode"></span>&lt;~~strong&gt;Choose a message delivery mode (those options are mutually exclusive, thus you can not select several of them):~~
    -   ~~**digest MIME format**: instead of receiving the list messages in a normal manner, you will get a digest of them on a regular basis. This digest compiles a group of messages from the list, using multipart/digest MIME format. The digest frequency is set up by the list owner.~~
    -   ~~**digest plain text format**: instead of receiving the list messages in a normal manner, you will get a digest of them on a regular basis. This digest compiles a group of messages from the list, using plain text format. The digest frequency is set up by the list owner.~~
    -   ~~**summary mode**: instead of receiving the list messages in a normal manner, you will get a list of them on a regular basis. To read the messages, you will need to browse the online list archive.~~
    -   ~~**notice mode**: with this mode, you will receive all the messages with a blank body: this way you are informed of every message sent to the list real time, without risk of flooding your inbox.~~
    -   ~~**no mail (useful for vacations)**: this mode makes it possible not to receive the messages of the list. It is especially useful when you have no access to your email for a long time and want to remain subscribed to the list nevertheless.~~
    -   ~~**text only mode**: this mode allows you to receive only the text version (text/plain) of messages sent in both formats (plain text and HTML).~~
    -   ~~**HTML only mode**: this mode allows you to receive only the HTML version (text/html) of messages sent in both formats.~~
    -   ~~**urlize mode**: this mode allows you not to receive attached documents. However these documents are available in the list archive and you can access them through a URL provided in the message.~~
    -   ~~**you do not receive your own posts**: this mode allows you not to receive a copy of your own messages.~~
    -   ~~**standard (direct reception)**: this mode is the default delivery mode; it cancels any other delivery mode.~~
    -   **suspended**: this mode allows you to suspend your subscription to one or more lists for a a specified or unspecified period. Unlike unsubscription, you can keep track of your subscription and reactivate it at any time by visiting the "Manage your subscription" section.
5.  ~~**Choose a visibility option**:~~
    -   ~~**listed in the list review page**: your name and email address will be displayed in the members list (if the list owner allowed subscribers to review the list members).~~
    -   ~~**concealed**: your name and email address will not be displayed in the members list. However you email address will be visible in the list archive if you send messages.~~
6.  ~~**Click on the 'Update' button**.~~

#### <span id="global_pref"></span>~~Changing your general preferences~~

~~The general preferences apply to all your subscriptions as well as to the way your Sympa mailing list web interface displays. To change your preferences, do as follows:~~

1.  ~~Go to the list environment **[homepage](%7B%7Bpath_cgi%7D%7D/home)** and **log on**.~~
2.  ~~In the form displayed on top of the left column, **click on the 'Your preferences' link**.~~
3.  ~~**Change your preferences**.~~
4.  ~~**Click on 'Submit' for every option** you change.~~

~~You can change:~~

-   ~~your **name**; if you subscribe to a list from the mailing list server web interface, the 'Name' field will automatically be filled in in the members list;~~
-   ~~the **language in which the Sympa web interface is displayed** (you can change language on every page of the web interface; your choice will remain even though you change the interface language on another page than the 'Preferences' page;~~
-   ~~the **lifetime of the cookie placed on your computer by Sympa** ('Connection expiration period'). By default, the session expires when you close your browser; if you use the mailing list service a lot, we advise you to choose a longer duration;~~

    | Note |
    |------|
    | ~~A cookie is a small file a web server stores on your hard disk, most generally temporarily, in order to identify you as a user of its service. It contains a few pieces of personal information about you: name, email address, latest logon time, etc.~~ |

-   ~~the **email address with which you subscribed** to the lists (if you subscribed with several email addresses, the address to be replaced will be the one you logged on with);~~

    | Note |
    |------|
    | ~~Be careful: this will change your subscriptions to all your lists. If you want to change address for a single mailing list, you had better unsubscribe from that list and subscribe again with the right email address.~~ |

-   ~~your **list password**.~~

~~The '**Your other email addresses**' section acts like an email address change.~~

### ~~Searching for a mailing list~~

~~You may need to search for a mailing list. To do that, you have three options:~~

-   ~~**browse the different sections** displayed on the [list environment homepage](%7B%7Bpath_cgi%7D%7D/home);~~
-   ~~search for a list via the **search box**: the searched string will return all the lists whose name or description matches your search criteria (descriptions of the lists generally consist of a short sentence);~~
-   ~~click on the '[List of lists](%7B%7Bpath_cgi%7D%7D/lists)' tab on top of page to **display all available lists**.~~

| Note |
|------|
| ~~According to the domain to which your email address belongs (example: *cru.fr*, *fai.com*, etc.) and to the location you log on from, you will not have access to the same lists. However you can subscribe to a list that does not display if you know its name. To do this, [use your email client](#subscribe).~~ |

### <span id="archives"></span>~~Reading a list archive online~~

~~Please refer to the [**archive documentation**](arc.md).~~

### <span id="sendmsg"></span>~~Sending a message~~

~~Please refer to the [**documentation about sending messages**](sendmsg.md).~~

### <span id="shared"></span>~~Using the shared document web space~~

~~Please refer to the [**shared document web space documentation**](shared.md).~~

### <span id="suspend"></span>~~Suspending or resuming your subscription of each list~~

~~Please refer to the [**subscription management documentation**](suspend.md).~~

### <span id="unsubscribe"></span>~~Unsubscribing from lists~~

~~To unsubscribe from a list, do as follows:~~

1.  ~~From the address with which you subscribed to the list, send a **message to {{conf.email}}@{{conf.host}}**.~~
2.  ~~In the subject line of your email, type in: **unsubscribe nameofthelist** (replace 'nameofthelist' by the name of the list you want to unsubscribe from).~~
3.  ~~**Leave the message body blank**.~~

    | Note |
    |------|
    | ~~To save some time, you can also send several commands in a single message. To do that, follow the instructions available in the [How the mailing list service works](#howitworks) section.~~ |

~~You can also unsubscribe through the mailing list web interface (you will need to repeat the operation for each list you want to unsubscribe from):~~

1.  ~~Go to the list environment **[homepage](%7B%7Bpath_cgi%7D%7D/home)** and **log on**.~~
2.  ~~**Go to the information page of the list** you want to unsubscribe from.~~
3.  ~~**In the left menu, click on the 'Unsubscribe' link**.~~

------------------------------------------------------------------------
