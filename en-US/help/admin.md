<span id="docadmin"></span>~~Mailing lists - Owner and moderator guide~~
------------------------------------------------------------------------

### ~~Introduction: who is in charge of managing mailing lists?~~

~~Reminder: a mailing list service involves four types of roles:~~

-   **~~listmaster;~~**
-   **~~owner;~~**
-   **~~moderator;~~**
-   **~~subscriber.~~**

~~Refer to the [description of each role](introduction.md#roles) to know more about this.~~

### <span id="create_list"></span>~~Requesting the creation of a mailing list~~

~~The **list creation request** can be **subject to conditions**. Even though you meet those conditions, the **list creation** will nevertheless be **subject to approval by the listmasters**.~~

~~To request the creation of a mailing list, do as follows:~~

1.  ~~Go to the **[list environment homepage](%7B%7Bpath_cgi%7D%7D/home)** and [**log on**](user.md#sympa_auth).~~
2.  ~~In the top menu, **click on the 'Create list' link**.~~

    | Note |
    |------|
    | ~~If this link does not display, it means that you do not have the privileges required to create a list.~~ |

3.  ~~Give your list a **name** (only enter the name without the '@' and the domain name; example: *languages\_spanish* and not *languages\_spanish@{{conf.host}}*).~~

    | Note |
    |------|
    | ~~Do not use any spaces, accents or specials characters in list names: those characters might cause problems.~~ |

    | Note |
    |------|
    | ~~Choose an explicit yet short name: think of the subscribers who will have to type this name every time they will send a message to the list! If you manage a set of lists, you can prefix your lists' names with a common prefix; thus they will be sorted together and will be easily recognizable (example: *xx-users@{{conf.host}}, xx-hotline@{{conf.host}}*, etc.).~~ |

4.  ~~Choose a **list type** among the predefined types (the predefined types are only examples of typical configurations that can be changed by the list owners after creation; it is even possible to configure the list beyond the options offered in the list administration module, by asking the listmasters).~~
5.  ~~Enter a **subject** for your list. This subject will display as a header for all the list pages, and will also be visible on list index pages (list of lists, list of your subscriptions, etc.) and in the browser title bar.~~
6.  ~~Choose a **topic** in the 'Topics' drop-menu.~~

    | Note |
    |------|
    | ~~If no topic suits your needs, you can request the creation of a new topic by asking the listmasters.~~ |

7.  ~~Enter a **description** for your list. This description will display on the list information page and in the 'Subscribers Charter' sent by email to each new subscriber, under the 'List subject' heading. This description may involve explanations about the following issues:~~

    -   ~~object of the list and targets;~~
    -   ~~topics discussed;~~
    -   ~~operation of the list (liabilities, status of the list, etc.);~~
    -   ~~rules applying;~~
    -   ~~description of the typical subscribers (their occupations, the projects they manage, their nationalities, etc.).~~

    | Note |
    |------|
    | ~~You can format your list description with HTML tags. Be careful: if your description is long, cut it with manual line breaks (ENTER key of your keyboard); otherwise, it might not be entirely visible in your browser window.~~ |

8.  ~~Click on the '**Submit your creation request**' button.~~

~~A message displays to inform you that your list creation request has been sent to the listmasters and that from now on, you can modify the list by clicking on the 'Admin' button. However, the message warns you that the list will be actually installed and made visible on the server only after approval by a listmaster.~~

~~After this, you will have to **wait for the list creation to be approved of by one of the listmasters**. Then you will receive a notice message entitled '**Creation of the nameofthelist list**', informing you that your list was actually created.~~

~~**Last, subscribe to your list**: creating a list or becoming its owner or moderator does not mean that you are automatically subscribed to it!~~

### ~~Managing a list~~

~~To manage a list you own, do as follows:~~

1.  ~~Go to the **list environment homepage** and **[log on](user.md#sympa_auth)**.~~

    | Note |
    |------|
    | ~~If you are subscribed to the list with several addresses, use the address with which you requested the list creation.~~ |

2.  ~~Go to the information page of the list you want to manage.~~
3.  ~~In the left menu, **click on the 'Admin' link**.~~

~~To browse the sections of the administration module, click on the links below the 'Admin' link, in the left menu.~~

~~Those different sections allow you to:~~

-   ~~[configure the list](listconfig.md);~~
-   ~~[customize files related to the list](#customize);~~
-   ~~[manage subscribers](#manage_members);~~
-   ~~[manage the message archive of the list](#manage_archives);~~
-   ~~[manage bounces](#manage_bounces);~~
-   ~~[create, delete or restore the shared document web space](#manage_shared);~~
-   ~~[rename the list](#renamelist);~~
-   ~~[delete the list](#supprlist).~~

~~The options available in the 'Moderate' submenu allow you to:~~

-   ~~[moderate messages](#moderate) sent to the list;~~
-   ~~[moderate documents](shared.md) available in the shared document web space;~~
-   ~~[moderate pending subscriptions](#manage_members).~~

#### <span id="edit_list"></span>~~Configuring the list~~

~~To learn how to configure the list, please refer to the [**documentation about list configuration**](listconfig.md).~~

#### <span id="customize"></span>~~Customizing the list~~

~~From this page, you can **edit a number of files relating to your list**, among which:~~

-   ~~typical messages sent to subscribers in particular occasions:~~
    -   ~~**welcome message**: this message is the notice sent to people who just subscribed. You should write a charter for your list and add it in this welcome message. You can create a structured MIME message (reserved to the MIME format experts);~~
    -   ~~**unsubscribe message**: this message is sent to people unsubscribing from the list;~~
    -   ~~**deletion message**: this message is sent to people you unsubscribe from the list (DEL command), especially because their address caused bounces;~~
    -   ~~**remind message**: this message is sent to subscribers as a personalized reminder when using the REMIND command. This command is essential to the good management of your list since many bounces are due to people whose current address is not their subscription address anymore, or even who forgot that they were subscribed to the list;~~
    -   ~~**subscribing invitation message**: this message is sent to people you invite to subscribe to the list using the INVITE command;~~
    -   ~~**notice of message rejected by the moderator**: this message is sent to the sender of a message rejected by the moderator;~~
    -   ~~**notice of message rejected because of a virus**: this message is sent to the sender of a message in which a virus was found.~~
-   ~~miscellaneous files:~~
    -   ~~**list description**: the list description is sent by email in return to the INFO command. By default, it is also included in the welcome message (subscription notice). It is not the same as the list presentation page displayed on the mailing list web interface;~~
    -   ~~**list homepage**: this description is available on the information page of the list. It can be in HTML format. Even though you do not use this format, use `<br />` tags to indicate line breaks;~~
    -   ~~**message header**: when available, it is added as a MIME attachment at the beginning of each message distributed to the list;~~
    -   ~~**message footer**: when available, it is added as a MIME attachment at the end of each message distributed to the list.~~

~~By default, Sympa uses default files; in this case, the specific files corresponding to your list are empty. **To edit a file, choose it from the drop-down list and click on the 'Edit' button**. You will have the possibility to change the **'From' field** (sender), the **'Subject' field** (subject line) and the **message body**.~~

| Note |
|------|
| ~~Be careful: the values between square brackets are variables. Do not change them, unless you really know what you are doing...~~ |

#### <span id="manage_shared"></span>~~Managing the shared document web space~~

~~By default, lists have no shared document web space. Thus, you need to create it. To do that, go to the **list administration module** and click on the '**Create shared**' link.~~

~~To allow subscribers to publish documents in the shared document web space, you need to **change default rights**: in the list administration module, click on '**Edit list config**' and then on '**Privileges**'. At the bottom of the page, there is a drop-down list entitled '[**Who can edit**](listconfig.md#docsrights)'; choose the '**Restricted to subscribers (private)**' option.~~

| Note |
|------|
| ~~Be careful: if you created folders before changing those rights, the folders will still be unwritable. If you want to make them writable, you will have to [change access rights](shared.md#acces) for each folder.~~ |

~~You might also want to [set up **quotas**](listconfig.md#docsrights) for the shared document web space on the 'Privileges' page of the 'Edit list config' section.~~

~~To **know everything about the management of the shared document web space** (how to organize it, change access rights, name documents, etc.), refer to the '[Using the shared document web space](shared.md)' section of the User guide.~~

~~To **deny access to the shared document web space**, click on '**Delete shared**' in the 'Admin' submenu. Then you will still have the possibility to **reopen it** by clicking on '**Restore shared**'. Deleting and restoring the shared document web space has **no impact on the documents it contains**.~~

#### <span id="manage_members"></span>~~Managing subscribers~~

~~This section lets you browse the **list of all the list subscribers**. For each subscriber, the following information is available:~~

-   ~~**email address**;~~
-   ~~**domain** of the email address (*@cru.fr*, *@sympa.org*, *@fai.com*, etc.);~~
-   ~~**picture** (if that feature was activated for the list);~~
-   ~~**name** (according to the subscription method, it is not always displayed);~~
-   ~~[**message delivery mode**](#deliverymode);~~
-   ~~**data source** indicating the origin in case the subscriber is included in the list and not directly subscribed;~~
-   ~~**date of subscription** to the list;~~
-   ~~**latest update** of the subscriber options.~~

| Note |
|------|
| ~~By default, each page displays 25 subscribers. You can browse through the pages by using the browsing arrows or display more subscribers on each page. You may also wish to sort subscribers according to different criteria by clicking on the corresponding column header.~~ |

~~To **search a subscriber**, enter all or part of his/her email address or name in the input field and click on the '**Search**' button.~~

~~You can **subscribe other people to the list** from this page:~~

-   ~~To add **a single person**, enter his/her email address in the input field and click on the '**Add**' button.~~
-   ~~To add **several persons**, click on the '**Multiple add**' button. In the input field that displays, enter the email addresses and names of the people you want to subscribe to the list and click on '**Add subscribers**'.~~

| Note |
|------|
| ~~If you want to subscribe people without letting them know through a notice, tick the 'Quiet' box. However, it is far better to warn people that you subscribe them!~~ |

~~Even though you have the possibility to subscribe people to your mailing lists, it is always **much better that people take the necessary steps to subscribe themselves** to the list. You can also **invite people to subscribe to the list** through the INVITE command: send an email to {{conf.email}}@{{conf.host}} and type the following command in the message body: **invite nameofthelist emailaddress** (example: *invite list\_example john.doe(@)fai.com*).~~

~~To **accept or reject the subscription requests to the list**, click on '**Pending subscriptions**'. The list of all people who requested subscription to the list displays. To accept or reject a request, tick the box in front of a person's name and click on the button of your choice.~~

~~To **send a subscription reminder to all subscribers**, click on the '**Remind all**' button. The subscription reminder message contains:~~

-   ~~the **name of the list** to which the subscriber is subscribed;~~
-   ~~the **email address** with which the subscriber is subscribed;~~
-   ~~the subscriber's **list password**;~~
-   ~~a **link to the information page** of the list;~~
-   ~~a **clickable address in order to allow subscribers to unsubscribe** from the list.~~

| Note |
|------|
| ~~You can also configure an automatic subscription reminder through the '[Miscellaneous](listconfig.md#other)' page of the 'Edit list config' section.~~ |

~~To **unsubscribe subscribers** from this page, select them by ticking the boxes in front of their names and click on the '**Delete selected email addresses**' button.~~

| Note |
|------|
| ~~If you do not want to notify the subscribers, tick the 'Quiet' box. However, this is not advisable, except in the case of bouncing subscribers.~~ |

| Note |
|------|
| ~~Tip: to select all subscribers at once, first make sure that they are all displayed on the page, and then click on the 'Toggle selection' button: all subscribers will be selected in a single click!~~ |

~~To **change a subscriber's subscriber options**, click on his/her email address.~~

~~From this page, you can **change the name, email address and message delivery mode of the subscriber**. You can also **unsubscribe him/her**.~~

~~If the subscriber is [bouncing](#manage_bounces), another form displays under the 'Subscriber information' form:~~

~~The information displayed involves:~~

-   ~~the type of error (in English);~~
-   ~~the number or errors;~~
-   ~~the period during which errors occurred.~~

~~You can **check the latest error** or **reset errors**. If you reset errors, the subscriber's [score](listconfig.md#bouncers) will be reset to zero.~~

~~To manage bouncing addresses more easily, go to the '[Bounces](#manage_bounces)' page of the list administration module.~~

#### <span id="manage_bounces"></span>~~Managing bounces~~

~~When there is a **problem with subscribers' email addresses** (obsolete email addresses, addresses temporarily unavailable when messages were sent, inbox quota exceeded, etc.), the percentage of bouncing addresses displays in the left menu under the text '**Error rate**'. To check the bouncing addresses, go to the '**Bounces**' page of the list administration module.~~

~~The Sympa software automatically manages bouncing subscribers: according to the number of errors and to the traffic on the list, bouncing subscribers are either notified, unsubscribed, or their score is reset to zero when their address stops bouncing.~~

~~To **make addresses stop bouncing**, select them by ticking their boxes and click on the '**Reset errors for selected users**' button. If the error remains, the addresses will be reported as bouncing again as soon as a message is posted on the list.~~

~~You can also **unsubscribe subscribers whose addresses are still bouncing**: too many bouncing addresses cause a considerable load on the mailing list server. To unsubscribe subscribers, select them by ticking the boxes in front of their names and click on the '**Delete selected email addresses**' button.~~

| Note |
|------|
| ~~Tip: to select all subscribers at once, first make sure that they are all displayed on the page, and then click on the 'Toggle selection' button: all subscribers will be selected in a single click!~~ |

#### <span id="moderate"></span>~~Moderating messages sent to the list~~

~~When a list is moderated, **all messages have to be approved of by one of the moderators before being distributed to the list**. After sending a message to a list, subscribers are automatically notified by email that their message will be moderated. As for moderators, they also receive a notice message from Sympa, which includes the message to moderate.~~

~~You can **perform moderating tasks** either **by email**, by answering the messages received from Sympa, or **through the mailing list web interface**. To do that, click on the '**Message**' link in the 'Moderate' submenu: you are brought to a page that displays all messages to be moderated (the most recent messages are on top of page). **To read a message, click on its subject**.~~

~~You have **two options**:~~

-   ~~**authorize the message distribution** on the list;~~
-   ~~**reject the message and notify sender**: when you reject a message, it is better to notify its sender...~~

~~All moderators can decide to distribute a message or not. However, **the first moderator to process the message will carry the day**. You will be notified by Sympa if you try to process a message that has already been moderated. When there are several moderators, it is **easier to moderate messages from the mailing list web interface**: thus, you will be able to view all messages remaining to be moderated.~~

| Note |
|------|
| ~~**Whatever the date and time of moderation, the date and time of sending of the message do not change**. Thus, if the distribution of the message is allowed with a lot of delay, it is possible to receive a message dated January 1st on December 31st!~~ |

~~In case the message was rejected with a notice, the subscriber who had sent it is notified by email. You can [customize the message he/she gets](#customize).~~

~~Checking the '**Reject without notification**' checkbox allows you to prevent the message author from receiving a notification.~~

~~Checking the '**Add to blacklist**' checkbox both skip the rejection notification and adds the message author to the list own blacklist. You can manage the blacklist via the '**edit blacklist**' button at the bottom of the page.~~

~~If you wish to customize the rejection message that is sent to a message author, you can do so via the '**Manage rejection messages**' button. The message management page will let define a set of rejection messages and define the default one.~~

~~**Reminder**: you can [add or remove moderators](listconfig.md#description) through the list administration module. To do that, from the list information page, click on '**Admin**', on '**Edit list config**', and then on '**List definition**'.~~

~~It is also possible to **process messages after their distribution on the list**; this can be useful when a list is not moderated. If you want to **delete a message**, [search for it in the online message archive](arc.md#arcsearch) and click on the '**Tag this mail for deletion**' button in the upper right corner of the message. A confirmation message displays; click on 'OK'. The message will be deleted after a few seconds. **Be careful: this operation is irreversible!!! If you delete a message, you will not be able to retrieve it.**~~

#### <span id="manage_archives"></span>~~Managing the message archive~~

~~The mailing list management robot Sympa can generate **downloadable compressed archives (.ZIP format) of the messages sent to the list**. To download those archives, **select the months** that interest you in the list and click on the '**Download Zip file**' button.~~

| Note |
|------|
| ~~Tip: in the 'Archive selection' list, to select all months during which messages have been sent, click on the first month, hold down the SHIFT key and click on the last month of the list.~~ |

~~You will receive a file of the type '**nameofthelist\_archive.zip**' containing **folders named 'nameofthelist\_year-month'** (example: *list\_example\_2005-06*) for each month. Inside each folder, **the file names are numbers** representing their position in the chronology of the messages sent (example: the file named '1' contains the first message sent in the month). The message files have **no extension**; use the text editor of your choice (Notepad, WordPad, Vim, etc.) to open them. **Each file represents an entire message (full header)**.~~

~~From the 'Manage archive' page, you can also **delete messages** (deletion month by month and not message by message). To do that, **select the months** that interest you in the list and click on the '**Delete selected months**' button.~~

| Note |
|------|
| ~~**Be careful: this operation is irreversible!!! When you click on 'Delete selected months', keep in mind that you are not only deleting an archive file, but also the entire message archive of the selected month!!!**~~ |

#### <span id="renamelist"></span>~~Renaming the list~~

~~In the **list administration module**, click on '**Rename list**'. Enter the name of your choice and click on the 'Rename this list' button. A confirmation message displays; click on 'OK'.~~

| Note |
|------|
| ~~If you change your mind, you will only have to redo the inverse operation in order to retrieve the former list name.~~ |

~~Be careful: when you rename a list, you have to let the listmasters know; otherwise, the change will not be effective.~~

~~A few tips to name your lists:~~

-   ~~**Do not use any spaces, accents or specials characters** in list names: those characters might cause problems.~~
-   ~~Choose an **explicit yet short name**: think of the subscribers who will have to type this name every time they will send a message to the list!~~
-   ~~If you manage a set of lists, you can **prefix your lists' names with a common prefix**; thus they will be sorted together and will be easily recognizable (example: *xx-users@{{conf.host}}, xx-hotline@{{conf.host}}.fr*, etc.).~~

#### <span id="supprlist"></span>~~Deleting the list~~

~~In the **list administration module**, click on '**Remove list**'. A confirmation message displays; click on 'OK'.~~

| Note |
|------|
| ~~**Be careful: if you delete the list, you will not be able to reopen it yourself!!! If you want to reopen the list, you will have to ask the listmasters.**~~ |

~~In real terms, what are the **consequences** of a list deletion?~~

-   ~~**All subscribers are immediately unsubscribed** automatically (including owners and moderators).~~
-   ~~**The message archive is preserved** but no one can access it anymore.~~
-   ~~**The documents published in the shared document web space are preserved** but no one can access them anymore.~~
-   ~~**Only the listmasters have the power to reopen the list**; if they do, the former list subscribers will automatically be subscribed again.~~

| Note |
|------|
| ~~Be careful: due to a slight latency, the list pages remain accessible for a while if you know their addresses. Then they will become fully unavailable.~~ |

~~**If you want the list and all the associated files to be deleted permanently**, you will have to ask the listmasters.~~

### <span id="rulesadmin"></span>~~Good practices~~

~~In order to have dynamic lists, **you must be deeply involved** in their exchanges: if a list is neither controlled nor enlivened by its owners, it may result in a loss of quality in its messages and it might even end up vanishing...~~

~~**The use of email in general and for mailing lists is bound by a set of precise rules necessary to share pleasant exchanges: the "Netiquette"**. As a list owner or moderator, it is your role to have subscribers respect it. You will find the general principles of the Netiquette, as well as many links on the [page of the Wikipedia dedicated to the Netiquette](http://en.wikipedia.org/wiki/Netiquette).~~

<span id="charter"></span>~~You should **write a charter for your list** to define all the rules that apply to its use:~~

-   ~~allowed, tolerated and forbidden topics;~~
-   ~~writing rules (for example to specify the languages in which the subscribers are to post, to ban "SMS language", etc.);~~
-   ~~rules applying when sending messages (frequency, attachments, etc.);~~
-   ~~liabilities of subscribers regarding the netiquette;~~
-   ~~rights and responsibilities of the subscribers;~~
-   ~~information about retention of the messages sent to the list;~~
-   ~~legal information and privacy policy;~~
-   ~~sanctions applying to those who would not respect the list charter;~~
-   ~~etc.~~

| Note |
|------|
| ~~In order to have all subscribers read the list charter, you should include it in the welcome message they get after subscribing. To do that, you need to [customize that message](#customize) through the 'Customize' page of the list administration module.~~ |

~~When available, the 'Owner and moderator charter' provides list owners and moderators with all the necessary information to carry out their roles. This Charter involves all the rights and responsibilities of owners and moderators.~~

------------------------------------------------------------------------
