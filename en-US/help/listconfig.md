<span id="listconfig"></span>~~Configuring the list~~
-----------------------------------------------------

~~As the list configuration is quite complex, it is divided in several parts with a separate page for each part:~~

-   ~~[List definition](#description);~~
-   ~~[Sending/receiving](#sending);~~
-   ~~[Privileges](#command);~~
-   ~~[Archive](#archives);~~
-   ~~[Bounces](#bounces);~~
-   ~~[Miscellaneous](#other).~~

~~We advise you to **make configuration changes very progressively**: thus, if the result does not match your expectations, it will be easier to backtrack.~~

~~The list administration module offers you **many options to configure your list**. However, these options might not match your own needs perfectly. To cure this problem, you can **ask the listmasters to create new options** (within the limits of what they can do, naturally...): access and/or rights limited to some categories of people according to the place they log on from, the domain of their email address, the user group they belong to, etc.~~

### <span id="description"></span>~~List definition~~

~~In the '**Subject of the list**' area, you can change the subject you had chosen when creating the list. This subject displays as a header for all the list pages, and is also be visible on list index pages (list of lists, list of your subscriptions, etc.) and in the browser title bar.~~

~~You can also change the '**Visibility of the list**'. The options available are the following:~~

-   ~~conceal except for subscribers (conceal) - *default option*;~~
-   ~~intranet access (intranet);~~
-   ~~no conceal (noconceal);~~
-   ~~conceal even for subscribers (secret);~~

| Note |
|------|
| ~~If you want to limit the list visibility according to other criteria, you should ask the listmasters: they may be able to create a new option matching your needs (example: list visible only by members of a user group, of an Internet domain, etc.).~~ |

~~In the 'Owners' and 'Moderators' areas, you can **add owners and moderators** to the list or **change their personal information**:~~

-   ~~For each owner/moderator, you have to indicate an **email address** and a **name**.~~
-   ~~You can also add the information of your choice in the '**Private information**' input box (phone number, function, etc.); this information will only be accessible by listmasters and list owners with a 'Privileged' profile.~~
-   ~~You can change the **message delivery mode** (the only options available on this page are 'mail' and 'nomail').~~
-   ~~The 'Profile' parameter can not be changed: the **'Privileged' profile** is reserved to the list creator (other owners have a 'Normal' profile).~~

| Note |
|------|
| ~~Be careful: becoming owner or moderator of a list does not mean that you are automatically subscribed to that list. Thus owners and moderators have to subscribe themselves to the list.~~ |

~~To **delete owners/moderators**, clear the content of the input boxes relating to the person you want to delete and click on the 'Update' button.~~

~~You can also change the **list topic** as well as its **language**. If you change the list language, all predefined messages will be sent in the chosen language (be careful: subject to the availability of a translation!).~~

~~You can not change the **Internet domain** of the list: only the listmasters can change this parameter.~~

~~**BE CAREFUL: do not forget to click on the 'Update' button** on bottom of page to save all your changes.~~

### <span id="sending"></span>~~Sending/receiving~~

~~From this page, you can **decide who will be allowed to post messages on the list**.~~

~~In the '**Digest frequency**' area, you can define how frequently compiled messages are sent (Digest and Summary delivery modes): in the list, select all the **days** for which you want digests to be sent. Then choose a **delivery time** for digests (please avoid choosing a time between 11 p.m. and midnight).~~

~~In the '**Available subscription options**' list, select all the subscriber options you want to offer to your subscribers. By default, all options are selected.~~

~~The '**Reply address**' area allows you to define the default recipients of any reply to a message sent to the list:~~

-   ~~With the '**All**' value, the reply is sent to both the **message sender** AND the **list**.~~
-   ~~With the '**List**' value, the reply is sent to the **list**.~~

    | Note |
    |------|
    | ~~Be careful: use this option carefully! Experience shows that subscribers do not always check the address to which they send their reply. Thus, they might send private messages to the whole list when trying to reply to a single person...~~ |

-   ~~With the '**Other\_email**' value, the reply is sent to a **predefined address**. If you choose this option, you will have to **indicate an email address in the 'Other email address' input box**.~~
-   ~~With the '**Sender**' value, the reply is sent to the **message sender**. This is the option you should probably choose.~~

~~The '**Respect of existing header field**' drop-down list allows you to choose how the 'Reply-To' SMTP header field will be processed in incoming messages. The '**Respect**' option preserves that field while the '**Forced**' option allows it to be overwritten.~~

~~Last, the '**Subject tagging**' option lets you choose the **text included before the subject of all messages** sent to the list: this allows subscribers to sort their messages easily, to use message filters on them in order to process messages automatically, etc. By default, this text consists of the **list name surrounded by square brackets** (the square brackets are automatically added by the system, thus it is useless that you add them yourself).~~

~~**BE CAREFUL: do not forget to click on the 'Update' button** on bottom of page to save all your changes.~~

### <span id="command"></span>~~Privileges~~

~~From this page, you can decide:~~

-   ~~**who can view list information**. The following options are available:~~
    -   ~~for anyone (open) - *default option*;~~
    -   ~~restricted to subscribers (private).~~
-   **~~who can subscribe to the list. The following options are available:~~**
    -   ~~subscription request confirmed (auth);~~
    -   ~~need authentication (notification is sent to owners) (auth\_notify);~~
    -   ~~requires authentication then owner approval (auth\_owner);~~
    -   ~~subscribe is impossible (closed);~~
    -   ~~restricted to local domain users (intranet);~~
    -   ~~local domain users or owner approval (intranetorowner);~~
    -   ~~for anyone without authentication (open) - *default option*;~~
    -   ~~anyone, notification is sent to list owner (open\_notify);~~
    -   ~~anyone, no welcome message (open\_quiet);~~
    -   ~~owner approval (owner);~~
    -   ~~requires S/MIME signed (smime);~~
    -   ~~requires S/MIME signed or owner approval (smimeorowner).~~

        | Note |
        |------|
        | ~~You should always choose an option involving the 'auth' parameter: this way, the system requires confirmation from the future subscriber by email before subscribing him/her to the list. This avoids subscriptions with invalid email addresses and guarantees that no one can be subscribed to the list without knowing it.~~ |

-   ~~**who can unsubscribe from the list**. The following options are available:~~
    -   ~~need authentication (auth);~~
    -   ~~authentication requested, notification sent to owner (auth\_notify);~~
    -   ~~impossible (closed);~~
    -   ~~open (open) - *default option*;~~
    -   ~~open with mail confirmation, owner is notified (open\_notify);~~
    -   ~~owner approval (owner).~~

        | Note |
        |------|
        | ~~You should always choose an option involving the 'auth' parameter: this way, the system requires confirmation from the subscriber by email before unsubscribing him/her from the list. This prevents ill-intentioned people from unsubscribing others without letting them know.~~ |

-   **~~who can invite people to subscribe to the list. The following options are available:~~**
    -   ~~closed (closed);~~
    -   ~~list owner, no authentication (owner);~~
    -   ~~restricted to subscribers (private) - *default option*;~~
    -   ~~public (public).~~
-   ~~**who can review subscribers**. The following options are available:~~
    -   ~~no one can review (closed);~~
    -   ~~restricted to subscribers or local domain users (intranet);~~
    -   ~~listmaster only (listmaster);~~
    -   ~~only owner (and listmaster) (owner) - *default option*;~~
    -   ~~restricted to subscribers (private);~~
    -   ~~anyone can do it! (public).~~

        | Note |
        |------|
        | ~~You should in no case make the members list accessible to anyone. The 'Restricted to subscribers' option may be interesting in order to allow subscribers to communicate with each others without posting messages on the list. However, this is not appropriate in the case of an announcement list involving subscribers having no particular relationship.~~ |

<span id="docsrights"></span>~~From this page, you can also **define the access rights applying to the shared document web space** ('Shared documents' section of the list, accessible through a link in the left menu). You can define both the read and write access rights for the documents:~~

-   ~~The following options are available in the '**Who can view**' drop-down list:~~
    -   ~~restricted to subscribers or local domain users (intranet);~~
    -   ~~restricted to list owners (owner);~~
    -   ~~restricted to subscribers (private) - *default option*;~~
    -   ~~public documents (public).~~
-   ~~The following options are available in the '**Who can edit**' drop-down list:~~
    -   ~~restricted to list owners (owner) - *default option*;~~
    -   ~~moderated for subscribers (editor);~~
    -   ~~restricted to subscribers (private);~~
    -   ~~public documents (public).~~

~~The '**Quota**' input box allows you to define a **maximum size not to be exceeded for the shared document web space**. This size does not represent the maximum size of *one* document published in the shared document web space, but the maximum size for all documents published on the list. It is expressed in kilobytes. When a subscriber tries to publish a too large document regarding the space left, he/she gets an error message.~~

~~To know **more about the management of the shared document web space** (how to organize it, change access rights, name documents, etc.), please refer to the '[Using the shared document web space](shared.md)' section of the User guide.~~

~~**BE CAREFUL: do not forget to click on the 'Update' button** on bottom of page to save all your changes.~~

### <span id="archives"></span>~~Archive~~

~~From this page, you can **decide who can access the online list archive** (messages readable on the mailing list web interface). The following options are available:~~

-   ~~closed (closed);~~
-   ~~restricted to local domain users (intranet);~~
-   ~~listmaster (listmaster);~~
-   ~~owner (owner);~~
-   ~~moderator (moderator);~~
-   ~~subscribers only (private);~~
-   ~~public (public).~~

~~The '**Quota**' input box allows you to define a **maximum size not to be exceeded for the message archive**. This size is expressed in kilobytes. List owners are notified when the archive size reaches 95 % of the allowed size. When the maximum size is reached, later messages are not archived.~~

| Note |
|------|
| ~~Even though messages stop being archived, it is naturally still possible to send messages to the list.~~ |

~~It is also possible to **access the list archive by email**, by sending **{{conf.email}}@{{conf.host}}** the following command: <span class="commande">**GET nameofthelist year-month**</span> (example: *GET list\_example 2016-07*). Then you receive a compilation of all messages sent during the chosen month. This compilation is sent in plain text and contains HTML tags instead of the original formatting; it also involves full headers for each message. The '**Text archives**' parameter allows you to define:~~

-   ~~**who is allowed** to receive the list message archive by email;~~
-   ~~**how frequently these archive files will be created**. For example, if the frequency is set to 'month', all messages distributed to the list in a month will be gathered in a single archive file.~~

~~If this parameter is not defined, the list will have no archive accessible by email. Be careful: **only the listmasters have the power to change this parameter.**~~

~~It is possible to send **messages encrypted in S/MIME** to the list. The '**Archive encrypted mails as cleartext**' option allows you to define how those messages will be archived:~~

-   ~~The '**Decrypted**' option archives the message after removing the encryption.~~
-   ~~The '**Original**' option archives the message under its original encrypted form.~~

~~This option applies to both the text archive and the online archive, as well as to the compilations sent to those who chose the 'Digest' delivery mode.~~

~~BE CAREFUL: do not forget to click on the 'Update' button on bottom of page to save all your changes.~~

### <span id="bounces"></span>~~Bounces~~

~~"**Bounces**" represent the **subscribers whose address is in error**, i.e. subscribers who can not receive the messages sent to the list. This can be due to many reasons: obsolete email addresses, addresses temporarily unavailable when messages were sent, inbox quota exceeded, etc.~~

~~The '**Bounce management**' section defines two rates:~~

-   ~~The **warn rate** indicates the bouncing email addresses rate from which the list owner will receive a **notice entitled 'Bounce rate too high'** inviting him/her to delete bouncing subscribers from the list.~~
-   ~~The **halt rate** indicates the bouncing email addresses rate from which **the message distribution will automatically be stopped** up to the resolution of the problem (generally through the deletion of bouncing subscribers).~~

<span id="bouncers"></span>~~The '**Management of bouncers, 1st level**' and '**Management of bouncers, 2nd level**' sections allow you to perform automatic tasks with regard to bouncing subscribers. You can define:~~

-   ~~the **score ranges that define level 1 and level 2 bouncers**. By default, level 1 bouncers have a score comprised between 45 and 74 and level 2 bouncers have a score comprised between 75 and 100;~~

    | Note |
    |------|
    | ~~The score depends on the number, type and frequency of errors. If the bouncing time is too short or if there have not been many errors, the bouncer is not given a score.~~ |

-   ~~the **task to perform towards the subscribers concerned**: no task, notice, deletion from the list;~~
-   ~~the **person to be notified** when a task is carried out: no one, the list owners, the listmasters. The notice sent when a task is carried out involves the names of all the subscribers concerned as well as precise information about the task.~~

~~**To manage bounces** (reset errors for some subscribers, unsubscribe bouncing subscribers, request a subscription reminder, etc.), **go to the '[Bounces](admin.md#manage_bounces)' page** of the list administration module.~~

~~BE CAREFUL: do not forget to click on the 'Update' button on bottom of page to save all your changes.~~

### <span id="other"></span>~~Miscellaneous~~

~~The '**Periodical subscription expiration task**' option allows you to define an **automatic expiration deadline for subscriptions** to the list: on a regular basis (example: once a year), subscribers will receive a message asking them to renew their subscription to the list. If they don't, they will automatically be unsubscribed. This procedure ensures that all people subscribed to the list are really concerned and interested.~~

~~The '**Periodical subscription reminder task**' option allows you to **send subscription reminders** to list members on a regular basis.~~

~~The '**email address protection method**' option ensures that the subscribers' email addresses will not be collected by robots for spamming purposes. This option applies to all the list pages.~~

~~On this page, you can also view **information about the last update of the list** (who made it and when), as well as the **number of configuration change** since the list was created.~~

~~**BE CAREFUL: do not forget to click on the 'Update' button** on bottom of page to save all your changes.~~
