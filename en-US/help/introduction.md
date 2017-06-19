~~Mailing lists - General introduction~~
----------------------------------------

### ~~What is a mailing list?~~

~~A mailing list is a **distribution list allowing a group of subscribers to automatically receive by email all messages sent to the list**: every message sent to the list by a subscriber is received by all the other subscribers. When subscribed to a mailing list, it is possible to send messages, to reply to them or to read them without contributing (i.e. to "lurk").~~

~~Special cases:~~

-   ~~It is sometimes possible to send messages to a mailing lit without having subscribed to it. However, you need to be subscribed to a list to receive its messages.~~
-   ~~It is sometimes impossible to send messages to the list even though you are actually subscribed to it: it is the case for announcement lists, which are used to transmit information from a unique sender to a large number of recipients.~~

### ~~Interest of mailing lists~~

~~People subscribe to a mailing list (sometimes abbreviated in ML) to **be informed about a particular topic** and to **take part in exchanges about it**. Examples are:~~

-   ~~mailing list for all the employees of a company;~~
-   ~~mailing list reserved to the participants in a project;~~
-   ~~mailing list dedicated to a class of students;~~
-   ~~mailing list about the latest news in computer security;~~
-   ~~mailing list of mutual aid between handymen;~~
-   ~~mailing list restricted to a family and dedicated to the organization of large family gatherings;~~
-   ~~and so on!~~

### ~~Types of mailing lists~~

~~There are **thousands of mailing lists** of all kinds on the Internet: public or private, free or not, with subscription subject to conditions or not, etc. Those lists may have from a dozen up to several thousand members.~~

~~According to the way they work, we can distinguish between **two types of lists**:~~

-   ~~**Announcements lists** allow subscribers to receive messages without being allowed to post some themselves. In fact, those messages are newsletters: electronic magazines, daily services (daily horoscope, daily weather report, daily security alert, etc.), update notices about a website, etc. With this type of mailing list, the information flows from a unique sender to a large number of recipients.~~
-   ~~**Discussion lists** allow all subscribers to take part in exchanges. Those lists can be moderated or not:~~
    -   ~~In a **moderated discussion list**, messages are transmitted to all subscribers after approval by one of the list moderators. Moderation is a token of quality for the list. For example, it ensures that subscribers will not receive off-topic messages, unsolicited commercial messages (spams), messages containing large attachments, etc.~~
    -   ~~In a **non moderated discussion list**, messages are transmitted to all subscribers as soon as the mailing list management robot receives them.~~

### <span id="features"></span>~~Features~~

~~Once subscribed to a mailing list service, you can:~~

-   ~~search for mailing lists matching your main interests or your particular situation;~~
-   **~~manage your subscriptions:~~**
    -   ~~[subscribe](user.md#subscribe) to lists,~~
    -   ~~[unsubscribe](user.md#unsubscribe) from lists to which you are subscribed,~~
    -   ~~change your [subscriber options](user.md#options) list by list,~~
    -   ~~change your [general preferences](user.md#pref), which apply to the whole mailing list environment (name, password, language of the mailing list web interface, etc.);~~
-   **~~use mailing lists~~**:
    -   ~~read the [online message archive of lists to which you are not subscribed](arc.md) if that archive is public and if your personal rights allow you to access those lists,~~
    -   ~~read the [archive of lists to which you are subscribed](arc.md),~~
    -   ~~perform [searches in the list archive](arc.md#arcsearch),~~
    -   ~~[send messages](sendmsg.md) to lists to which you are subscribed,~~
    -   ~~[download documents](shared.md#shared_read) from the shared document web space,~~
    -   ~~[upload documents](shared.md#shared_upload) in the shared document web space;~~
-   **~~manage mailing lists~~**:
    -   ~~[create new lists](admin.md#create_list) (restricted access) - subject to authorization,~~
    -   ~~[configure lists](admin.md#edit_list) you own,~~
    -   ~~[manage subscriptions](admin.md#manage_members),~~
    -   ~~[manage the shared document web space](admin.md#manage_shared),~~
    -   ~~[moderate lists](admin.md#moderate) for which you are a moderator.~~

### <span id="roles"></span>~~How the mailing list service works: roles and responsibilities~~

~~A mailing list service involves four types of roles:~~

-   ~~**listmaster;**~~
-   ~~**owner;**~~
-   ~~**moderator;**~~
-   ~~**subscriber.**~~

~~It is possible to have several roles at once (for example, you can be an owner and a moderator of a list and be subscribed to several others).~~

#### ~~Listmasters~~

~~Listmasters are in charge of the **management of the mailing list service**. Their duties:~~

-   ~~**manage the mailing list server** (deployment, maintenance, etc.);~~
-   ~~**define the general orientations of the mailing list service**:~~
    -   ~~who will be allowed to ask for the creation of a new list,~~
    -   ~~which options will be available to manage lists (scenario definition),~~
    -   ~~what the default files will contain (creation of templates),~~
    -   ~~what will the mailing list web interface look like;~~
-   ~~**set the way the mailing list service should be used** and **document those rules through providing charters** to subscribers, moderators and owners;~~
-   ~~**approve of requests of mailing list creations**;~~
-   ~~**temporarily replace list owners** when necessary; on the other hand, listmasters are not supposed to take the place of moderators.~~

~~List owners and moderators can turn to listmasters when they face a problem not dealt with by the documentation or for any comment. However, in order not to flood listmasters with messages, it is recommended that subscribers rather turn to list owners.~~

#### ~~Owners~~

~~The list owner is generally its creator or, failing him/her, the person who requested the list creation or who became responsible for it. **His/her role**:~~

-   ~~**define the [way the list will be used](admin.md#edit_list)**;~~
-   ~~**write a [list charter](admin.md#charter)** aimed at subscribers;~~
-   ~~**appoint one or several [moderators](listconfig.md#description)**;~~
-   ~~**manage [subscriptions and unsubscriptions](admin.md#manage_members)**;~~
-   ~~**decide whether it is relevant to put a [shared document web space](admin.md#manage_shared)** at the subscribers' disposal;~~
-   ~~**answer questions from subscribers and potential subscribers about the list;**~~
-   ~~etc.~~

~~A list can have several owners. However, the **'Privileged' profile** is reserved to the list's creator; other owners have a 'Normal' profile, which has fewer prerogatives.~~

#### ~~Moderators~~

~~**Moderators are appointed by the list owner**. They are **in charge of [controlling the relevancy of the messages](admin.md#moderate)** sent to the list: after reading them, **they choose to accept or to reject them** . Moderation occurs before the message is actually sent to subscribers. Rejection of a message is possibly followed by a notice to the sender in order to explain the reason for that rejection.~~

~~A list can have **one or several moderators**; generally, the list owner is also a moderator.~~

~~This concerns only moderated lists.~~

### <span id="policy"></span>~~Regulatory framework~~

~~The use of a mailing list service means respecting a number of rules:~~

-   ~~In most mailing list services, subscribers receive a 'List subscribers charter' on subscription. Then they are obliged to respect all the rules contained in that charter.~~
-   ~~If available, list owners and moderators have to conform to the 'Owner and moderator charter'.~~
-   ~~The use of mailing lists naturally means respecting the rules of good practices as regards to email.~~

~~To know more, refer to the section dedicated to [good practices for subscribers](sendmsg.md#rulesuser) and to the section about [good practices for owners and moderators](admin.md#rulesadmin).~~

------------------------------------------------------------------------
