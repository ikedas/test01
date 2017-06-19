Les listes de diffusion - Guide de l'utilisateur
------------------------------------------------

### <span id="howitworks"></span>Fonctionnement du service de listes

Le service de listes fonctionne grâce à un **logiciel de gestion de listes : Sympa**. Ce logiciel est **associé à une interface web d'environnement de listes**.

**Pour effectuer des actions relatives aux listes** (vous abonner, changer vos options, etc.), vous avez deux possibilités :

-   **connectez-vous sur l'interface web du serveur de listes** ;
-   **envoyer des commandes par e-mail** à l'automate Sympa à l'adresse **{{conf.email}}**.

**Pour envoyer des commandes à Sympa**, procédez comme suit :

-   **Si vous n'envoyez qu'une seule commande**, inscrivez-la dans l'objet de votre message et laissez le corps du message vide.
-   **Si vous envoyez plusieurs commandes**, laissez l'objet de votre message vide et tapez les différentes commandes dans le corps du message. **Attention** : Sympa ne traitera pas votre message si vous ne respectez pas scrupuleusement les règles suivantes :
    -   Chaque commande doit être placée seule sur une ligne.
    -   Le message doit être envoyé en texte brut et non en HTML (aucun formatage).
    -   Le message ne doit rien contenir d'autre que des commandes reconnaissables par Sympa (pas de signature automatique).

Vous pouvez consulter l'[ensemble des commandes que vous pouvez envoyer par mail à Sympa](mail_commands.md).

### <span id="subscribe"></span>S'abonner à des listes

Pour s'abonner à une liste, la procédure est très simple :

1.  **Choisissez l'adresse** avec laquelle vous souhaitez vous abonner à la liste.

    | Note |
    |------|
    | Choisissez de préférence une adresse que vous pouvez consulter fréquemment et qui vous offre une bonne capacité de stockage : certaines listes voient passer de très nombreux messages, parfois accompagnés de pièces jointes volumineuses. |

    | Note |
    |------|
    | Vous pouvez choisir de vous abonner à la même liste avec plusieurs adresses différentes. Pour cela, vous devrez recommencer la procédure d'abonnement avec votre client de messagerie, mais en utilisant un autre compte de messagerie. |

2.  Envoyez un **message à {{conf.email}}** avec l'adresse à partir de laquelle vous souhaitez vous abonner.

    | Note |
    |------|
    | Sympa n'est pas une personne mais un automate de gestion de listes de diffusion. Inutile donc de lui envoyer des mots doux ! ;-) |

3.  En objet du message, écrivez : **subscribe nomdelaliste Prénom Nom** (remplacez 'nomdelaliste' par le nom de la liste à laquelle vous souhaitez vous abonner et indiquez vos propres prénom et nom).
4.  **Laissez le corps du message vide**.

    | Note |
    |------|
    | Vous pouvez également envoyer plusieurs commandes dans le même message pour gagner du temps. Pour cela, procédez comme indiqué dans la section [Fonctionnement du service de listes](#howitworks). |

**Vous recevrez ensuite un message vous informant que votre demande a été acceptée ou rejetée** : si l'inscription à la liste est soumise à approbation, le propriétaire peut choisir de ne pas vous abonner. Dans ce cas, il est inutile de renvoyer plusieurs demandes d'abonnement, car le résultat sera toujours le même. Vous pouvez éventuellement envoyer un message directement au propriétaire de la liste (nomdelaliste-request@{{conf.host}}) en justifiant le pourquoi de votre demande d'abonnement.

| Note |
|------|
| Note : dans certains cas, on vous demandera au préalable de confirmer votre demande d'abonnement. Conformez-vous aux instructions contenues dans le message expédié le cas échéant. |

En fonction du type de liste (liste à inscription soumise à conditions ou non) et de la disponibilité du propriétaire, **le délai de réception de la notification peut varier**. Il est inutile d'envoyer plusieurs demandes.

**Si votre demande a été acceptée, le message que vous recevez confirme votre inscription à la liste. Ce message** (la Charte des abonnés de la liste) **contient plusieurs informations capitales :**

-   votre **mot de passe de listes**. Ce mot de passe sera le même pour l'ensemble des listes auxquelles vous serez abonné avec la même adresse. Vous pouvez le [modifier en ligne](#global_pref "Comment modifier son mot de passe") en vous connectant sur l'environnement de listes ;
-   des **informations détaillées sur la liste** : son objet, l'adresse web où aller consulter les archives, etc ;
-   les **conditions d'utilisation de la liste** : sujets de discussion autorisés et exclus, nétiquette, informations légales, politique de confidentialité, etc ;

**Conservez précieusement votre notification de confirmation d'inscription** : vous pourriez en avoir besoin ultérieurement pour vous rappeler votre mot de passe ou pour envoyer une commande précise à Sympa (exemple : commande de désabonnement). D'une manière générale, **nous vous conseillons d'archiver toutes les notifications de confirmation d'inscription à une liste de diffusion**.

Il est **également possible de s'abonner à une liste via l'interface web** du serveur de listes. Pour cela, procédez comme suit :

1.  Allez sur la **[page d'accueil](%7B%7Bpath_cgi%7D%7D/home)** de l'environnement de listes et **connectez-vous**.
2.  **Allez sur la page d'information de la liste** à laquelle vous souhaitez vous abonner.
3.  Dans le menu de gauche, **cliquez sur le lien 'Abonnement'**.

### <span id="sympa_auth"></span>Se connecter sur l'environnement de listes

Pour vous connecter sur l'environnement de liste, utilisez la zone d'authentification située dans la colonne gauche de l'interface web. Si vous êtes déjà connecté, votre adresse e-mail et votre profil (abonné, modérateur ou propriétaire) s'affichent à cet endroit. Dans le cas contraire, un formulaire de connexion vous est proposé.

En fonction de votre situation personnelle, la procédure d'authentification varie :

-   **Si l'entité qui propose le service de listes utilise un système de compte et d'authentification unique** (SSO, *single sign-on*, par exemple via le système CAS), le mieux est de vous authentifier à l'aide de votre compte unique. Pour cela, cliquez sur le bouton 'Go' situé à côté du texte '**Authentification \[nom du système en place\]**'. Entrez ensuite votre identifiant et votre mot de passe auprès du serveur d'authentification.

    | Note |
    |------|
    | Si vous êtes déjà connecté sur un autre service utilisant le système d'authentification unique, votre connexion est immédiate. Rechargez la page si nécessaire. |

-   **Si vous n'êtes pas concerné par une procédure d'authentification unique**. Dans ce cas, connectez-vous via la méthode classique : entrez l'**adresse e-mail avec laquelle vous êtes abonné** comme identifiant et votre **mot de passe de listes** dans le champ 'Mot de passe'.

    | Note |
    |------|
    | Si vous ne vous souvenez plus de votre mot de passe de listes, cliquez sur « Mot de passe perdu ? ». Vous devrez ensuite indiquer votre adresse e-mail ; un mail contenant une URL de validation vous sera envoyé à cette adresse. |

-   Si vous n'êtes pas encore inscrit, cliquez sur '**Première connexion**Indiquez votre adresse e-mail. Un lien de confirmation (URL) vous sera envoyé à cette adresse. Cliquer sur ce lien pour être redirigé vers la page où vous pourrez définir votre mot de passe.

| Note |
|------|
| Attention : le mot de passe de listes est un mot de passe spécial qui ne vous sert que pour les listes. |

### Consulter ses abonnements

Pour voir toutes les listes auxquelles vous êtes abonné, vous devez tout d'abord [vous connecter](#sympa_auth). Vous voyez apparaître dans la boîte 'Vos listes' de la colonne de gauche, le nom de toutes les listes auxquelles vous êtes abonné, suivi chacun d'une brève description de la liste.

**Pour aller consulter la page d'information d'une liste, cliquez sur son nom**. La page d'information comporte une description plus ou moins détaillée de la liste (son objet, les usages en vigueur pour l'envoi de messages, etc.).

À partir de cette page d'information, vous pourrez :

-   modifier vos [options d'abonné](#options) ;
-   [lire les archives](arc.md) de la liste ;
-   effectuer une [recherche dans les archives](arc.md#search) ;
-   [envoyer des messages](sendmsg.md) ;
-   [télécharger des documents](shared.md#downloaddoc) à partir de l'espace partagé ;
-   [publier des documents](shared.md#publishdoc) dans l'espace de stockage partagé ;
-   accéder à la [liste des abonnés](#subscribers) (lorsqu'elle est disponible) ;
-   [suspendre ou reprendre](suspend.md) votre abonnement pour chaque liste;
-   [vous désabonner](#unsubscribe) de la liste.

<span id="subscribers"></span>Le **nombre de personnes abonnées** à la liste est affiché de manière permanente dans le **menu de gauche**. **Pour accéder à la liste des abonnés, cliquez sur le lien 'Voir les abonnés'** dans le menu de gauche (si le propriétaire de la liste n'a pas autorisé l'accès à la liste des abonnés, ce bouton n'apparaît pas). La liste des abonnés s'affiche et vous présente l'**adresse e-mail** et le **nom** de chacun des abonnés (la mention ou non du nom dépend de la méthode employée lors de l'abonnement).

| Note |
|------|
| Par défaut, 25 abonnés sont affichés sur chaque page. Vous pouvez naviguer entre les pages au moyen des flèches de navigation ou choisir d'afficher davantage d'abonnés sur chaque page. Vous pouvez également trier les abonnés en fonction de leur adresse e-mail, de leur domaine ou de leur nom en cliquant sur l'intitulé de la colonne correspondante. |

**Les noms des propriétaires et des modérateurs de la liste sont indiqués dans le menu de gauche**. N'écrivez jamais directement à un propriétaire ou à un modérateur de liste. Lorsque vous avez une question ou une remarque, l'adresse que vous devez utiliser est : **nomdelaliste-request@{{conf.host}}** (remplacez 'nomdelaliste' par le nom de la liste en question).

Pour voir la **date de votre inscription à la liste** et la **date de dernière mise à jour de vos options d'abonné**, **cliquez sur le lien 'Options d'abonné'** dans le menu de gauche.

### <span id="pref"></span>Gérer ses préférences

Pour une **plus grande souplesse** dans votre utilisation des listes, **il vous est possible de définir certaines préférences personnelles**. Ces préférences se décomposent en deux volets :

-   vos **options d'abonné**, qui sont à choisir liste par liste ;
-   vos **préférences générales**, valables pour tout l'environnement de listes Sympa.

#### <span id="options"></span>Modifier ses options d'abonné

**Les options d'abonné sont relatives à chaque liste** et peuvent donc différer d'une liste à l'autre. Pour modifier vos options d'abonné, procédez comme suit :

1.  Allez sur la **[page d'accueil](%7B%7Bpath_cgi%7D%7D/home)** de l'environnement de listes et **connectez-vous**.
2.  **Allez sur la page d'information de la liste** pour laquelle vous souhaitez modifier vos options d'abonné.
3.  Dans le menu de gauche, **cliquez sur le lien 'Options d'abonné'**.
4.  <span id="deliverymode"></span>**Choisissez un mode de réception des messages** (ces options sont exclusives, vous ne pouvez donc pas en sélectionner deux différentes) :
    -   **Compilation au format MIME** : au lieu de recevoir régulièrement les messages de la liste, vous en recevrez périodiquement une compilation. Cette compilation regroupe un ensemble de messages de la liste au sein d'un message au format MIME multipart/digest. La périodicité d'envoi des compilations est définie par le gestionnaire de la liste.
    -   **Compilation au format texte** : au lieu de recevoir régulièrement les messages de la liste, vous en recevrez périodiquement une compilation. Cette compilation regroupe un ensemble de messages de la liste au sein d'un message au format texte simple. La périodicité d'envoi des compilations est définie par le gestionnaire de la liste.
    -   **Résumé des messages** : comme pour le mode digest, vous recevrez périodiquement une compilation, excepté qu'il s'agit cette fois uniquement d'un index des messages. Si vous souhaitez les lire dans leur entier, vous devrez aller consulter les archives de la liste en ligne.
    -   **Notification** : avec cette méthode, vous allez recevoir tous les messages avec un corps vide. De cette manière, vous êtes informé en temps réel de l'arrivée de messages sans prendre pour autant le risque de voir votre boîte mail saturée.
    -   **Interrompre la réception des messages** : ce mode permet de ne plus recevoir les messages de la liste tout en y restant abonné. Cela évite par exemple de devoir se désabonner d'une liste pendant une période d'absence puis de se réabonner lorsque l'on revient.
    -   **Réception au format texte uniquement** : ce mode permet de ne recevoir que la version texte (text/plain) des messages postés aux deux formats (texte et HTML).
    -   **Réception au format HTML** : ce mode permet de ne recevoir que la version HTML (text/html) des messages postés aux deux formats (texte et HTML).
    -   **Attachements stockés sur le serveur** : ce mode permet de ne pas recevoir les documents attachés. Ceux-ci sont remplacés dans le message par une URL pointant vers l'interface web.
    -   **Pour ne pas recevoir ses propres messages** : ce mode permet de ne pas recevoir une copie de ses propres messages.
    -   **Normal** : ce mode est le mode de réception par défaut ; il permet d'annuler les autres modes d'abonnement.
    -   Suspension: ce mode vous permet de suspendre votre abonnement à une ou plusieurs listes pour une période déterminée ou non. Contrairement au désabonnement, vous pouvez garder une trace de votre abonnement et de le réactiver à tout moment en visitant la page "Gérer votre abonnement".
5.  **Choisissez une option de visibilité** :
    -   **Référencé dans la liste des abonnés** : vous serez visible dans la liste des abonnés (si l'accès à celle-ci est autorisé).
    -   **Non visible** : vous ne serez plus visible dans la liste des abonnés. Votre adresse e-mail sera néanmoins visible dans les archives des messages si vous en avez envoyé.
6.  **Cliquez sur le bouton 'Mise à jour'**.

#### <span id="global_pref"></span>Modifier ses préférences générales

Les préférences générales sont relatives à l'ensemble de vos abonnements et à la manière dont se présente votre interface de listes Sympa. Pour modifier vos préférences, procédez comme suit :

1.  Allez sur la **[page d'accueil](%7B%7Bpath_cgi%7D%7D/home)** de l'environnement de listes et **connectez-vous**.
2.  Dans la boîte en haut de la colonne de gauche, **cliquez sur le lien 'Vos préférences'**.
3.  **Modifiez vos préférences**.
4.  **Cliquez sur 'Valider' pour chaque option** que vous modifiez.

Vous pouvez modifier :

-   votre **nom** ; si vous vous abonnez à une liste depuis l'interface web du serveur de listes, le champ 'Nom' sera automatiquement renseigné dans la liste des abonnés ;
-   la **langue de l'interface de listes Sympa** (le choix de la langue est disponible sur toutes les pages de l'interface de listes ; votre choix sera conservé même si vous modifiez la langue de l'interface sans passer par la page 'Préférences' ;
-   la **durée de vie du cookie stocké sur votre ordinateur par Sympa** ('Expiration de la connexion'). Par défaut, la session expire lorsque vous fermez votre navigateur ; si vous utilisez les listes de manière intensive, nous vous conseillons de choisir une durée plus longue ;

    | Note |
    |------|
    | Un cookie est un petit fichier qu'un serveur web enregistre, le plus souvent temporairement, sur votre disque dur, pour vous identifier sur son service. Il contient quelques informations de référence vous concernant : nom, adresse e-mail, date de dernière connexion, etc. |

-   l'**adresse e-mail avec laquelle vous êtes abonné** aux listes (si vous êtes abonné aux listes avec plusieurs adresses, l'adresse remplacée sera celle avec laquelle vous êtes connecté);

    | Note |
    |------|
    | Attention : ceci modifiera vos abonnements à l'ensemble des listes. Si vous ne souhaitez changer d'adresse e-mail que pour une seule liste, il vaut mieux vous désabonner de cette liste et vous y réabonner avec l'adresse idoine. |

-   votre **mot de passe de listes**.

La section '**Vos autres adresses e-mail**' équivaut à un changement d'adresse e-mail.

### Rechercher une liste de diffusion

Vous pouvez avoir besoin de rechercher une liste. Pour cela, vous avez trois possibilités :

-   **parcourir les différentes rubriques** listées en [page d'accueil du serveur de listes](%7B%7Bpath_cgi%7D%7D/home) ;
-   rechercher une liste grâce au **champ de recherche** : la chaîne recherchée renverra tous les résultats trouvés dans les noms et les descriptions des listes (les descriptions des listes se résument généralement à une courte phrase) ;
-   cliquer sur l'onglet '[Liste des listes](%7B%7Bpath_cgi%7D%7D/lists)' en haut de page pour **afficher l'intégralité des listes**.

| Note |
|------|
| En fonction du domaine auquel appartient votre adresse (exemple : *cru.fr*, *fai.com*, etc.) et de l'endroit à partir duquel vous vous connectez, vous n'aurez pas accès aux mêmes listes. Vous pouvez malgré tout vous abonner aux listes qui vous sont cachées si vous connaissez leur nom. Pour cela, [utilisez votre client de messagerie](#subscribe). |

### <span id="archives"></span>Lire les archives d'une liste en ligne

Consultez la [**documentation des archives**](arc.md).

### <span id="sendmsg"></span>Envoyer un message

Consultez la [**documentation pour l'envoi de messages**](sendmsg.md).

### <span id="shared"></span>Utiliser l'espace de stockage partagé

Consultez la [**documentation de l'espace de stockage**](shared.md).

### <span id="suspend"></span>suspendre ou reprendre votre abonnement à chaque liste

Consultez la [**documentation sur la gestion des abonnements**](suspend.md).

### <span id="unsubscribe"></span>Se désabonner des listes

Pour vous désabonner d'une liste, procédez comme suit :

1.  À partir de l'adresse avec laquelle vous êtes abonné à la liste, envoyez un **message à {{conf.email}}**.
2.  En objet du message, écrivez : **unsubscribe nomdelaliste** (remplacez 'nomdelaliste' par le nom de la liste dont vous souhaitez vous désabonner).
3.  **Laissez le corps du message vide**.

    | Note |
    |------|
    | Vous pouvez également envoyer plusieurs commandes dans le même message pour gagner du temps. Pour cela, procédez comme indiqué dans la section [Fonctionnement du service de listes](#howitworks). |

Vous pouvez également vous désabonner à partir de l'interface de listes (vous devrez répéter l'opération pour chaque liste dont vous souhaitez vous désabonner) :

1.  Allez sur la **[page d'accueil](%7B%7Bpath_cgi%7D%7D/home)** de l'environnement de listes et **connectez-vous**.
2.  **Allez sur la page d'information de la liste** dont vous souhaitez vous désabonner.
3.  **Dans le menu de gauche, cliquez sur le lien 'Désabonnement'**.

------------------------------------------------------------------------
