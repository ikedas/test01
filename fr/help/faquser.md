### Problèmes rencontrés par les abonnés

#### Vous n'arrivez pas à vous abonner à une liste

Ce problème peut être dû aux raisons suivantes :

-   **Les propriétaires de la liste ont oublié de traiter votre demande d'abonnement** : l'erreur est humaine et il se peut que votre demande ait été noyée au milieu de nombreux autres mails ! Resoumettez votre demande avant de [contacter directement les propriétaires de la liste](#contactadmin).
-   **L'abonnement à la liste est réservé à une catégorie de personnes particulière**. Pour en savoir plus, [contactez les propriétaires de la liste](#contactadmin).

#### Vous n'arrivez pas à vous connecter sur l'interface web du serveur de listes

Ce problème peut être dû aux raisons suivantes :

-   **Vous n'avez pas de mot de passe**. Pour vous faire allouer un mot de passe, suivez le lien [Première connexion](%7B%7Bpath_cgi%7D%7D/sendpasswd) depuis la page d'accueil. Vous recevrez ce mot de passe par e-mail.
-   **Vous avez saisi un mot de passe incorrect**. Si vous avez oublié votre mot de passe, vous pouvez le réinitialiser. Pour cela, suivez le lien [Mot de passe perdu ?](%7B%7Bpath_cgi%7D%7D/renewpasswd) depuis la page d'accueil.
-   **Vous n'utilisez pas le bon identifiant** (l'adresse e-mail avec laquelle vous êtes abonné).

| Note |
|------|
| Afin d'éviter toute erreur dans la saisie de votre mot de passe, effectuez une opération de copier/coller entre votre logiciel de messagerie et votre navigateur web. |

#### Vous ne recevez pas (tous) les messages diffusés sur une liste

Les raisons du problème peuvent être multiples :

-   <span id="notsubscribedyet"></span>**Vous n'avez jamais été abonné à la liste** : :
    -   Vous vous êtes peut-être trompé dans votre adresse e-mail lors de votre demande d'abonnement.
    -   Vous êtes peut-être abonné avec une autre adresse e-mail que celle que vous consultez.
    -   Votre demande d'abonnement a peut-être été rejetée par les propriétaires de la liste.

    Dans tous les cas, essayez de [vous abonner](user.md#abbo) à nouveau.
-   <span id="notsubscribedanymore"></span>**Vous n'êtes plus abonné à la liste** ::
    -   Si votre adresse a été en erreur pendant un certain temps, le système peut vous avoir désabonné automatiquement (cela peut également être le fait des propriétaires de la liste). Essayez de vous [réabonner](user.md#abbo) après vous être assuré que votre adresse e-mail ne poserait plus de problème.
    -   Si vous n'avez pas respecté les règles d'utilisation de la liste, il est possible que les propriétaires vous aient « banni »...
    -   Vous pouvez aussi avoir été désabonné de manière arbitraire par une personne malintentionnée, si la liste n'est pas configurée de manière à demander une confirmation pour toute demande d'abonnement/désabonnement... Dans ce cas, essayez de vous [réabonner](user.md#abbo).
-   **Votre [mode de réception](user.md#deliverymode) ne vous permet pas de recevoir les messages** : c'est par exemple le cas pour le mode de réception 'Nomail'.
-   **Votre boîte de réception est saturée**. Attention : si votre boîte de réception n'est pas complètement saturée, vous recevrez uniquement les messages les moins volumineux, ce qui retardera le diagnostic... Si votre adresse e-mail est régulièrement à l'origine de problèmes, vous risquez en outre d'être désabonné par les propriétaires ou par le système. Nettoyez donc votre boîte de réception.
-   **Votre boîte de réception est affectée par certaines restrictions** : elle ne vous permet pas de recevoir les messages avec pièces jointes, interdit certains types de pièces jointes ou limite la taille des messages entrants ; dans ce cas, nous vous conseillons de choisir le [mode de réception Urlize](user.md#deliverymode).

#### Vous n'arrivez pas à envoyer des messages sur une liste

Les raisons du problème peuvent être multiples :

-   **Vous n'avez [jamais été abonné](#notsubscribedyet)** à la liste.
-   **Vous n'êtes [plus abonné](#notsubscribedanymore)** à la liste.
-   **Vous utilisez une autre adresse** que celle avec laquelle vous êtes abonné à la liste.
-   **Si la liste est une liste modérée, la diffusion du message dépend de la disponibilité des modérateurs** : ceux-ci ne peuvent pas surveiller nuit et jour la liste de diffusion ! La diffusion du message peut donc prendre un peu de retard.
-   **Si la liste est une liste modérée, il est possible que votre message ait été rejeté par un modérateur**. Si vous n'avez reçu aucune notification, vous pouvez éventuellement écrire à nomdelaliste-request@{{conf.host}} pour obtenir des explications.
-   -   **Le message que vous essayez d'envoyer ne remplit pas les critères de diffusion** sur la liste : il peut être trop volumineux, contenir des pièces jointes d'un type interdit ou tout simplement contenir des pièces jointes, quelles qu'elles soient (si les pièces jointes sont interdites sur la liste).
-   **Le problème peut également venir de votre compte de messagerie** :
    -   Le serveur de courrier est temporairement indisponible.
    -   Votre boîte de réception est saturée, ce qui vous empêche d'envoyer de nouveaux messages.
    -   Votre boîte de réception est affectée par certaines restrictions : elle ne permet pas l'envoi de messages avec pièces jointes, interdit certains types de pièces jointes ou limite la taille des messages sortants.
-   Enfin, **peut-être vous êtes-vous tout simplement trompé dans l'adresse de la liste** en expédiant votre message !

#### Vous n'arrivez pas à vous désabonner d'une liste

Les raisons du problème peuvent être multiples :

-   **Vous utilisez une autre adresse** que celle avec laquelle vous êtes abonné à la liste.
-   **Vous êtes abonné via une source de données dynamique** (exemples : base de données, annuaire LDAP, etc.) qui ne vous autorise pas à vous désabonner. [Contactez les propriétaires de la liste](#contactadmin) pour en savoir plus.
-   **Les propriétaires de la liste ont oublié de traiter votre demande de désabonnement** : l'erreur est humaine et il se peut que votre demande ait été noyée au milieu de nombreux autres mails ! Resoumettez votre demande avant de [contacter directement les propriétaires de la liste](#contactadmin).

#### <span id="contactadmin"></span>Vous souhaitez contacter les responsables d'une liste

Les noms des propriétaires et des modérateurs des listes sont indiqués dans le menu de gauche. Néanmoins, n'écrivez jamais directement à un propriétaire ou à un modérateur de liste : d'une part la personne à qui vous écrivez peut être absente, d'autre part, il est mieux d'informer tous les responsables de votre requête. Lorsque vous avez une question ou une remarque, **l'adresse que vous devez utiliser est : nomdelaliste-request@{{conf.host}}** (remplacez 'nomdelaliste' par le nom de la liste en question).
