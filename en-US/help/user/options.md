~~This is a description of the reception modes available in Sympa. These options are mutually exclusive, which means that you can't set two different receive modes at the same time. Only some of the modes might be available to specific mailing lists.~~

-   ~~Digest~~
    Instead of receiving individual mail messages from the list, the subscriber will periodically receive batched messages in a Digest. This Digest compiles a group of messages from the list, using the multipart/digest MIME format.
    ~~The sending interval for these Digests is defined by the list owner.~~
-   ~~DigestPlain~~
    Similar to the Digest option in that the subscriber will periodically receive batched messages in a Digest. With DigestPlain the Digest is sent in a plain text format, with all attachments stripped out. DigestPlain is useful if your email software doesn't display multipart/digest format messages well.
    ~~The sending interval for these Digests is defined by the list owner.~~
-   ~~Summary~~
    Instead of receiving individual mail messages from the list, the subscriber will periodically receive a list of messages. This mode is very close to the Digest reception mode but the subscriber receives only the list of messages.
-   ~~Nomail~~
    ~~This mode is used when a subscriber no longer wishes to receive mail from the list, but nevertheless wishes to retain the ability to post to the list. This mode therefore prevents the subscriber from unsubscribing and subscribing later on.~~
-   Txt
    This mode is used when a subscriber wishes to receive mails sent in both HTML and plain text formats only in plain text format.
-   Html
    This mode is used when a subscriber wishes to receive mails sent in both HTML and plain text formats only in HTML format.
-   Urlize
    This mode is used when a subscriber does not want to receive attached files. The attached files are replaced by a URL leading to the file stored on the list site.
-   Not\_me
    This mode is used when a subscriber does not want to receive copies of messages that he or she has sent to the list.
-   Normal
    This option is used mainly to cancel the nomail, summary or digest modes. If the subscriber was in nomail mode, he or she will again receive individual mail messages from the list.

