<span id="docadmin"></span>Les listes de diffusion - Guide de l'administrateur
------------------------------------------------------------------------------

### Introduction : qui gère les listes de diffusion ?

Rappel : autour des listes de diffusion, on trouve quatre types d'acteurs :

-   **listmasters ;**
-   **propriétaires ;**
-   **modérateurs ;**
-   **abonnés.**

Reportez-vous à la [description du rôle de chacun](introduction.md#roles) pour en savoir plus.

### <span id="create_list"></span>Demander la création d'une liste de diffusion

La **demande de création** d'une liste de diffusion peut être **soumise à conditions**. Si vous remplissez les conditions nécessaires pour effectuer une demande, la **création de la liste** sera néanmoins **soumise à approbation par les listmasters**.

Pour demander la création d'une liste de diffusion, procédez comme suit :

1.  Consultez la **[page d'accueil du service](%7B%7Bpath_cgi%7D%7D/home)** et [**Connectez-vous**](user.md#sympa_auth)..
2.  Dans le menu supérieur, **cliquez sur le lien 'Création de liste'**.

    | Note |
    |------|
    | Si le bouton n'apparait pas, cela signifie que vous n'avez pas les privilèges nécessaires pour créer une liste. |

3.  Donnez un **nom** à votre liste (n'entrez que le nom sans l'arobase et le domaine ; exemple : *lettres\_grec* et non pas *lettres\_grec@*).

    | Note |
    |------|
    | N'utilisez pas d'espaces, d'accents, ni de caractères spéciaux dans les noms des listes : ces caractères peuvent créer des problèmes. |

    | Note |
    |------|
    | Choisissez un nom explicite mais pas trop long : pensez aux abonnés qui devront taper ce nom à chaque fois qu'ils voudront envoyer un message à la liste ! Si vous administrez un ensemble de listes, vous pouvez préfixer le nom de vos listes avec un préfixe commun afin qu'elles soient classées à la suite et clairement identifiables par tous (exemple : *xx-utilisateurs, xx-support(@)cru.fr*, etc.). |

4.  Choisissez un **type de liste** parmi les types prédéfinis suivants (il ne s'agit là que d'exemples de configurations type modifiables par les propriétaires de listes après création ; il est même possible de configurer la liste au delà des options proposées dans le module d'administration de liste, en en faisant la demande auprès des listmasters).
5.  Saisissez un **objet** pour votre liste. Cet objet apparaîtra en tête de toutes les pages de la liste, ainsi que sur les pages d'index de listes (liste des listes, liste de vos abonnements, etc.) et dans la barre de titre du navigateur.
6.  Choisissez une **catégorie** dans la liste déroulante 'Catégories'.

    | Note |
    |------|
    | Si aucune des catégories existantes ne répond à vos besoins, vous pouvez demander la création d'une nouvelle catégorie en vous adressant aux listmasters. |

7.  Saisissez une **description** pour votre liste. La description apparaîtra sur la page d'information de la liste ainsi que dans la 'Charte des abonnés de la liste' envoyée par e-mail à chaque nouvel abonné, à la rubrique 'Objet de cette liste'. Cette description peut comporter des explications sur les points suivants :

    -   objet de la liste et publics visés ;
    -   sujets abordés ;
    -   fonctionnement de la liste (responsabilités, statut de la liste, etc.) ;
    -   règles d'utilisation en vigueur ;
    -   présentation des abonnés type (leurs métiers, les projets dont ils s'occupent, leur nationalité, etc.).

    | Note |
    |------|
    | Vous pouvez mettre en forme la description de votre liste à l'aide de balises HTML. Attention : si votre description est longue, coupez-la par des retours à la ligne manuels (touche ENTRÉE de votre clavier), sans quoi elle ne sera pas visible entièrement dans la fenêtre de votre navigateur. |

8.  Cliquez sur le bouton '**Envoyer votre demande de création**'.

Un message s'affiche alors et vous informe que votre demande de création de liste est enregistrée et que vous pouvez dès à présent modifier la liste en cliquant sur le bouton 'Admin'. Il vous avertit néanmoins que la liste ne sera effectivement installée et rendue visible sur le serveur que lorsqu'un listmaster aura approuvé sa création.

Vous devrez ensuite **attendre que la création de la liste soit approuvée par l'un des listmasters**. Vous recevrez alors un e-mail de notification intitulé '**Création de la liste nomdelaliste**' vous informant que votre liste a bien été créée.

**Abonnez-vous ensuite à votre liste** : la création d'une liste ou le fait d'en devenir propriétaire ou modérateur n'implique pas l'abonnement automatique à la liste !

### Administrer une liste

Pour administrer une liste dont vous êtes propriétaire, procédez comme suit :

1.  Allez sur la **page d'accueil** de l'environnement de listes et **connectez-vous**.

    | Note |
    |------|
    | Si vous êtes abonné à la liste avec plusieurs adresses, utilisez celle avec laquelle vous avez demandé la création de la liste. |

2.  **Allez sur la page d'information de la liste** que vous souhaitez administrer.
3.  Dans le menu de gauche, **cliquez sur le lien 'Admin'**.

Pour passer d'une section à une autre, cliquez sur le menu de gauche sous l'intitulé 'Admin'.

Les différentes sections du module d'administration de la liste vous permettent :

-   de [configurer la liste](listconfig.md) ;
-   de [personnaliser les fichiers associés](#customize) à la liste ;
-   de [gérer les abonnés](#manage_members) ;
-   de [gérer les archives de messages](#manage_archives) de la liste ;
-   de [gérer les erreurs](#manage_bounces) ;
-   de [créer, fermer ou restaurer l'espace de stockage partagé](#manage_shared) ;
-   de [supprimer la liste](#supprlist).
-   de [renommer la liste](#renamelist) ;

Les liens compris dans le sous-menu 'Modérer' vous permettent :

-   de [modérer les messages](#moderate) envoyés à la liste ;
-   de [modérer les documents](shared.md) déposés dans l'espace de stockage partagé ;
-   de [modérer les abonnements](#manage_members) en attente de validation.

#### <span id="edit_list"></span>Configurer la liste

Consultez la [**documentation de la configuration de listes**](listconfig.md).

#### <span id="customize"></span>Personnaliser la liste

À partir de cette page, vous pouvez **éditer certains fichiers associés à votre liste**, parmi lesquels :

-   messages type envoyés aux abonnés dans certains cas particuliers :
    -   **message de bienvenue** : ce message correspond à la notification envoyée aux personnes qui viennent de s'abonner. Il est fortement conseillé de rédiger une charte d'utilisation pour votre liste et de l'inclure dans ce message de bienvenue. Vous pouvez créer un message MIME structuré (réservé aux experts du format MIME) ;
    -   **message de désabonnement** : ce message est envoyé aux personnes qui se désabonnent de la liste ;
    -   **message de suppression** : ce message est envoyé aux personnes que vous désabonnez (commande DEL), notamment parce que leur adresse a généré des erreurs ;
    -   **message de rappel individualisé** : ce message est envoyé aux abonnés lors d'un rappel individualisé (commande REMIND). La commande REMIND est importante pour la bonne gestion de votre liste, car de nombreuses erreurs d'acheminement du courrier (bounces) sont dues à des personnes dont l'adresse courante ne correspond plus à l'adresse d'abonnement, ou même qui ont oublié leur abonnement ;
    -   **invitation à s'abonner** : ce message est envoyé aux personnes que vous invitez à s'abonner à la liste via la commande INVITE ;
    -   **message de rejet par le modérateur** : ce message est envoyé à l'expéditeur lors du rejet d'un message par le modérateur ;
    -   **rejet d'un message contenant un virus** : ce message est envoyé à l'expéditeur en cas de détection d'un virus dans un message.
-   fichiers divers :
    -   **description de la liste** : la description de la liste est envoyée par e-mail en réponse à la commande INFO. Par défaut, elle est également incluse automatiquement dans le message de bienvenue (notification d'abonnement à la liste). Elle ne doit pas être confondue avec la page de présentation de la liste qui est affichée sur l'interface web du serveur de listes Sympa ;
    -   **page d'accueil de la liste** : cette description est affichée sur la page d'information de la liste. Elle peut être au format HTML. Même si vous n'utilisez pas ce format, employez quand même les balises `<br />` pour marquer les sauts de ligne ;
    -   **attachement de début de message** : s'il est défini, une partie MIME comprenant le texte sera ajoutée au début de chaque message diffusé sur la liste ;
    -   **attachement de fin de message** : s'il est défini, une partie MIME comprenant le texte sera ajoutée en fin de chaque message diffusé sur la liste.

Par défaut, Sympa utilise des fichiers par défaut ; dans ce cas, le fichier correspondant spécifique à votre liste est vide. **Pour modifier un fichier, choisissez-le dans la liste déroulante puis cliquez sur le bouton 'Éditer'**. Vous pourrez entre autres modifier le **champ 'From'** (expéditeur), le **champ 'Subject'** (objet) et le **corps des messages**.

| Note |
|------|
| Attention : les valeurs entre crochets sont des variables. Ne les modifiez pas, à moins de réellement savoir ce que vous faites... |

#### <span id="manage_shared"></span>Gérer l'espace de stockage partagé

Par défaut, les listes ne possèdent pas toujours d'espace de stockage partagé. Il faut donc le créer. Pour cela, allez dans le **module d'administration** de la liste et cliquez sur '**Créer un espace documents**'.

Pour que les abonnés puissent publier des documents dans l'espace de stockage partagé, vous devez **modifier les droits** par défaut : dans le module d'administration de la liste, cliquez sur '**Configurer la liste**' puis sur '**Droits d'accès**' (ou 'Privilèges'). Au bas de la page, vous trouverez une liste déroulante intitulée '[**Droit d'édition**](listconfig.md#docsrights)' ; choisissez l'option '**Limité aux abonnés (private)**'.

| Note |
|------|
| Attention : si vous avez créé des dossiers avant d'effectuer cette opération, ces dossiers resteront interdits en écriture. Si vous souhaitez les autoriser en écriture, vous devrez [modifier leurs droits d'accès](shared.md#acces) dossier par dossier. |

Découvrez également [comment créer des **quotas**](listconfig.md#docsrights) pour l'espace de stockage partagé via la page 'Privilèges' de la section 'Configurer la liste'.

Pour **tout savoir sur la gestion de l'espace de stockage partagé** (organisation de l'espace de stockage partagé, modification des droits d'accès, nommage des documents, etc.), reportez-vous à la section '[Utiliser l'espace de stockage partagé](shared.md)' du Guide de l'utilisateur.

Pour **supprimer tout accès à l'espace de stockage partagé**, cliquez sur '**Fermer l'espace documents**' dans le menu supérieur du module d'administration de liste. Vous pourrez ensuite **le rouvrir** en cliquant sur '**Restaurer l'espace documents**'. Le fait de fermer et de rouvrir l'espace de stockage partagé n'a **aucun impact sur les documents qu'il contient**.

#### <span id="manage_members"></span>Gérer les abonnés

La section 'Abonnés' vous présente la **liste de toutes les personnes abonnées à la liste**. Pour chaque abonné, les informations affichées sont :

-   **adresse e-mail** ;
-   **domaine** auquel appartient l'adresse utilisée pour l'abonnement (*@cru.fr*, *@sympa.org*, *@fai.com*, etc.) ;
-   **vignette** si la fonctionnalité a été activée pour la liste ;
-   **nom** (pas toujours affiché : la mention ou non du nom dépend de la méthode employée lors de l'abonnement) ;
-   [**mode de réception**](#deliverymode) des messages ;
-   **source de données** indiquant l'origine si l'utilisateur est inclus dans la liste et pas directement abonné ;
-   **date d'abonnement** à la liste ;
-   **date de dernière mise à jour** des options d'abonné.

| Note |
|------|
| Par défaut, 25 abonnés sont affichés sur chaque page. Vous pouvez naviguer entre les pages au moyen des flèches de navigation ou choisir d'afficher davantage d'abonnés sur chaque page. Vous pouvez également trier les abonnés en fonction de différents critères en cliquant sur l'intitulé des colonnes correspondantes. |

Pour **rechercher un abonné dans la liste**, entrez tout ou partie de son adresse e-mail ou de son nom dans le champ de saisie puis cliquez sur le bouton '**Recherche**'.

Vous pouvez **abonner de nouvelles personnes à la liste** à partir de cette page :

-   Pour ajouter **une seule personne**, entrez l'adresse e-mail de la personne que vous souhaitez abonner dans le champ de saisie et cliquez sur le bouton '**Ajout**'.
-   Pour ajouter **plusieurs personnes**, cliquez sur '**Abonnements par lots**'. Dans la zone de texte qui apparaît, entrez les adresses e-mail et les noms des personnes que vous souhaitez abonner à la liste (une personne par ligne). Supprimez le texte d'exemple puis cliquez sur '**Ajout d'abonnés**'.

| Note |
|------|
| Si vous souhaitez abonner des personnes sans qu'elles ne reçoivent de notification, cochez la case 'Sans prévenir'. Sachez néanmoins qu'il est déconseillé d'abonner des gens sans les prévenir. |

Même si vous pouvez abonner vous-même des personnes à vos listes de diffusion, il est toujours **préférable que les gens fassent la démarche de s'inscrire eux-mêmes** à la liste. Vous pouvez également **inviter des personnes à s'abonner à la liste** au moyen de la commande INVITE : envoyez un e-mail à {{conf.email}} en mettant dans le corps du message la commande **invite nomdelaliste adresseemail** (exemple : *invite cri-exemple jean.dupond(@)fai.com*).

Pour **accepter ou rejeter les demandes d'abonnement à la liste**, cliquez sur '**Abonnements en attente**'. Vous voyez apparaître la liste des personnes ayant demandé leur abonnement à la liste. Pour accepter ou rejeter une demande, cochez la case correspondant à la personne ayant effectué la demande et cliquez sur le bouton de votre choix.

Pour **envoyer à chacun des abonnés une notification de rappel d'abonnement**, cliquez sur le bouton '**Rappel des abonnements**'. La notification de rappel d'abonnement contient :

-   le **nom de la liste** à laquelle l'abonné est abonné ;
-   l'**adresse e-mail** avec laquelle l'abonné est abonné ;
-   le **mot de passe de listes** de l'abonné ;
-   un **lien vers la page d'information** de la liste ;
-   une **adresse cliquable pour se désabonner** de la liste.

| Note |
|------|
| Vous pouvez également configurer un rappel d'abonnement automatique via la page '[Divers](listconfig.md#other)' de la section 'Configurer la liste'. |

Pour **désabonner des abonnés** à partir de cette page, sélectionnez les abonnés en cochant les cases situées en bout de ligne et cliquez sur le bouton '**Désabonner les adresses sélectionnées**'.

| Note |
|------|
| Si vous souhaitez que le désabonnement ne soit pas suivi d'une notification, cochez la case 'Sans prévenir'. Il est déconseillé de désabonner des abonnés sans les prévenir, excepté dans le cas où il s'agit d'abonnés en erreur. |

| Note |
|------|
| Astuce : pour sélectionner tous les abonnés en une fois, assurez-vous tout d'abord qu'ils sont tous affichés sur la page, puis cliquez sur le bouton 'Inverser la sélection' : tous les abonnés seront sélectionnés en un clic ! |

Pour **modifier les options d'abonnés d'un abonné**, cliquez sur son adresse e-mail.

À partir de cette page, vous pouvez **modifier le nom, l'adresse e-mail et le mode de réception des messages de l'abonné**. Vous pouvez également **le désabonner**.

Si l'abonné est [en erreur](#manage_bounces), un second bandeau apparaît sous le bandeau 'Information abonné' :

Les informations affichées sont :

-   type d'erreur (en anglais) ;
-   nombre d'erreurs ;
-   période au cours de laquelle des erreurs ont été observées.

Vous pouvez **consulter la dernière erreur** ou **effacer toutes les erreurs**. Si vous effacez toutes les erreurs, le [score](listconfig.md#bouncers) de l'abonné sera remis à zéro.

Pour gérer plus facilement les adresses en erreur, allez à la page '[Erreurs](#manage_bounces)' du module d'administration de la liste.

#### <span id="manage_bounces"></span>Gérer les erreurs

Lorsqu'il y a un **problème avec les adresses e-mail de certains abonnés** (adresses qui n'existent plus, adresses momentanément indisponibles au moment de l'envoi de messages, capacité de la boîte de réception atteinte, etc.), un pourcentage d'adresses en erreur est affiché dans le menu de gauche sous le texte '**Taux d'adresses en erreur**'. Pour consulter les adresses en erreur, allez à la page '**Erreurs**' du module d'administration de la liste.

Le logiciel Sympa gère automatiquement les abonnés en erreur : en fonction du nombre d'erreurs et du trafic dans la liste, les abonnés en erreur sont soit notifiés, soit désabonnés, soit leur score est remis à zéro lorsque l'erreur ne se reproduit plus.

Pour **faire en sorte que des adresses ne soient plus en erreur**, sélectionnez ces adresses en cochant les cases situées en bout de ligne et cliquez sur le bouton '**Annuler les erreurs pour les abonnés sélectionnés**'. Si l'erreur persiste, les adresses concernées seront de nouveau marquées en erreur lors du prochain envoi de message.

Vous pouvez aussi **désabonner les abonnés dont les adresses sont toujours en erreur** : un nombre trop grand d'adresses en erreur cause une charge significative sur le serveur de listes. Pour désabonner des abonnés, sélectionnez leurs adresses en cochant les cases situées en bout de ligne et cliquez sur le bouton '**Supprimer les adresses sélectionnées**'.

| Note |
|------|
| Astuce : pour sélectionner tous les abonnés en une fois, assurez-vous tout d'abord qu'ils sont tous affichés sur la page, puis cliquez sur le bouton 'Inverser la sélection' : tous les abonnés seront sélectionnés en un clic ! |

#### <span id="moderate"></span>Modérer les messages envoyés à la liste

Lorsqu'une liste est modérée, **tous les messages doivent être approuvés par l'un des modérateurs avant de pouvoir être diffusés sur la liste**. Lorsqu'un abonné envoie un message à la liste, il reçoit un message de notification de la part de l'automate de gestion de listes Sympa, l'informant que son message va être modéré avant de pouvoir être diffusé. Les modérateurs, quant à eux, reçoivent également un message de Sympa, contenant le message à modérer.

Vous pouvez **effectuer des tâches de modération** soit **par e-mail**, en répondant aux messages que vous adresse Sympa, soit **via l'interface web du serveur de listes**. Pour cela, il vous suffit d'aller dans le **module d'administration de la liste** et de cliquer sur '**Modérer**' dans le menu supérieur : la page qui s'affiche contient tous les messages en attente de modération (les messages les plus récents sont en haut de la page). **Pour consulter un message, cliquez sur son objet**.

Vous avez **deux options** de modération :

-   **autoriser la diffusion du message** sur la liste ;
-   **rejeter le message avec notification** : lorsque vous rejetez un message, il est préférable de notifier son expéditeur...

Tous les modérateurs peuvent décider de diffuser ou non un message. Néanmoins, **c'est le premier modérateur à intervenir sur le message qui emporte la décision**. Si vous essayez d'intervenir sur un message qui a déjà été modéré, vous recevrez un message de Sympa vous informant que le message a déjà été traité. Si vous êtes plusieurs modérateurs, il est **préférable de modérer les messages depuis l'interface web du serveur de listes** : ainsi, vous verrez précisément quels messages restent à modérer.

| Note |
|------|
| **Quelles que soient la date et l'heure de la modération, la date et l'heure d'envoi du message ne changent pas**. Si la diffusion du message est autorisée avec beaucoup de retard, il est donc possible de recevoir le 31 décembre un message daté du 1er janvier ! |

En cas de rejet avec notification, l'abonné qui avait envoyé le message rejeté reçoit un message de notification. Vous pouvez [personnaliser ce message](#customize).

Cocher la case « **Rejeter sans notification** » empêchera l'envoi d'un message de notification de rejet à l'auteur du message.

Cocher la case « **Ajouter à la liste noire** » entraîne deux actions : le message est rejeté sans notifier son auteur et celui-ci est ajouté à la liste noire. Vous pouvez gérer votre liste noire en cliquant sur le bouton « **éditer la liste noire** » en base de la page.

Si vous désirez personnaliser le message de rejet que l'auteur du message recevra, cliquez sur le bouton « **Gestion des messages de rejet** ». La page de gestion des messages sera alors affichée. Vous pouvez y définir un ensemble de messages de rejet types.

**Rappel** : vous pouvez [ajouter ou supprimer des modérateurs](listconfig.md#description) via le module d'administration de la liste. Pour cela, à partir de la page d'information de la liste, cliquez sur '**Admin**', puis sur '**Configurer la liste**', et enfin sur '**Définition de la liste**'.

Il est aussi possible d'**intervenir sur les messages après leur diffusion sur la liste** ; ceci est utile dans le cas d'une liste non modérée. Si vous souhaitez **supprimer un message**, allez le consulter en ligne dans la section 'Archives' et cliquez sur le bouton '**Marquer ce message pour suppression**' situé en haut à droite du message. Un message de confirmation s'affiche ; cliquez sur OK. Le message sera supprimé au bout de quelques secondes. **Attention : cette manipulation est irréversible !!! Si vous supprimez un message, vous ne pourrez en aucun cas le récupérer.**

#### <span id="manage_archives"></span>Gérer les archives

L'automate de gestion de listes Sympa peut générer des **archives compressées téléchargeables (format .ZIP) des messages envoyés sur la liste**. Pour télécharger ces archives, **sélectionnez les mois** qui vous intéressent dans la liste et cliquez sur le bouton '**Télécharger le Zip**'.

| Note |
|------|
| Astuce : dans la liste 'Sélection des archives', pour sélectionner tous les mois pendant lesquels des messages ont été échangés, cliquez sur le premier mois, maintenez la touche SHIFT (ou « MAJ ») enfoncée et cliquez sur le dernier mois de la liste. |

Vous recevrez un fichier du type '**nomdelaliste\_archives.zip**' contenant des **dossiers du type 'nomdelaliste\_annee-mois'** (exemple : *cri-exemple\_2005-06*) pour chaque mois. À l'intérieur de chaque dossier, **les fichiers ont pour seul nom un numéro** qui représente leur place dans la chronologie des messages envoyés (exemple : le fichier '1' contient le premier message envoyé dans le mois). Les fichiers de messages n'ont **pas d'extension** ; utilisez l'éditeur de texte de votre choix (Bloc-notes, WordPad, Vim, etc.) pour les ouvrir. **Chaque fichier correspond à un message entier (en-tête détaillé)**.

À partir de la page 'Gérer les archives', vous pouvez également **supprimer des messages** (suppression mois par mois et non message par message). Pour cela, **sélectionnez les mois** qui vous intéressent dans la liste et cliquez sur le bouton '**Détruire les mois sélectionnés**'.

| Note |
|------|
| **Attention : cette manipulation est irréversible !!! Lorsque vous cliquez sur 'Détruire les mois sélectionnés', gardez bien à l'esprit que vous ne supprimez pas simplement un fichier d'archives, mais bien toutes les archives de messages du mois sélectionné !!!** |

#### <span id="renamelist"></span>Renommer la liste

Dans le **module d'administration** de la liste, cliquez sur '**Renommer la liste**'. Entrez le nom de votre choix puis cliquez sur le bouton 'Renommer la liste'. Un message de demande de confirmation s'affiche ; cliquez sur 'OK'.

| Note |
|------|
| Si vous changez d'avis, il vous suffira d'effectuer la même manipulation pour restaurer l'ancien nom de la liste. |

**ATTENTION : lors du renommage d'une liste, vous devez informer les listmasters, sans quoi le changement de nom ne pourra être effectif**.

Quelques conseils pour le choix des noms de vos listes :

-   N'utilisez **pas d'espaces, d'accents ni de caractères spéciaux** dans les noms des listes : ces caractères peuvent créer des problèmes.
-   Choisissez un **nom explicite mais pas trop long** : pensez aux abonnés qui devront taper ce nom à chaque fois qu'ils voudront envoyer un message à la liste !
-   Si vous administrez un ensemble de listes, vous pouvez **préfixer le nom de vos listes avec un préfixe commun** afin qu'elles soient classées à la suite et clairement identifiables par tous (exemple : *sympa-users(@)cru.fr, sympa-fr(@)cru.fr*, etc.).

#### <span id="supprlist"></span>Supprimer la liste

Dans le **module d'administration** de la liste, cliquez sur '**Supprimer la liste**'. Un message de demande de confirmation s'affiche ; cliquez sur 'OK'.

| Note |
|------|
| **Attention : si vous supprimez la liste, vous ne pourrez pas la rouvrir vous-même !!! Si vous désirez rouvrir la liste, il vous faudra faire appel aux listmasters.** |

Concrètement, quelles sont les **conséquences** d'une fermeture de liste ?

-   **Tous les abonnés sont immédiatement désabonnés** de façon automatique (y compris les propriétaires et modérateurs).
-   **Les archives de messages sont préservées** mais plus personne ne peut y accéder.
-   **Les documents publiés dans l'espace de stockage partagé sont préservés** mais plus personne ne peut y accéder.
-   **Seuls les listmasters ont le pouvoir de rouvrir la liste** ; tous les anciens abonnés seront réabonnés automatiquement.

| Note |
|------|
| Attention : en raison d'un petit temps de latence, les pages relatives à la liste restent accessibles à quiconque connaît leur adresse pendant un petit moment. Elles deviendront ensuite complètement inaccessibles. |

**Si vous souhaitez que la liste et tous les fichiers associés soient supprimés définitivement**, vous devrez vous adresser aux listmasters.

### <span id="rulesadmin"></span>Bonnes pratiques

Pour que vos listes de diffusion soient dynamiques, **vous devez être impliqué** dans leur fonctionnement : une liste non contrôlée risque de partir à vau l'eau, de voir la qualité de ses messages se dégrader et de finalement s'éteindre...

**L'utilisation de la messagerie en général et pour les listes de diffusion répond à un ensemble de règles très précises et indispensables pour une communication harmonieuse : la « Nétiquette »**. En tant que propriétaire ou modérateur de liste, vous devez veiller à la faire respecter. Vous pourrez trouver les principes généraux de la Nétiquette ainsi que de nombreux liens sur la [page de la Wikipédia consacrée à la Nétiquette](http://fr.wikipedia.org/wiki/N%C3%A9tiquette).

<span id="charter"></span>Il est conseillé de **rédiger une charte d'utilisation pour votre liste**, regroupant toutes les règles qui la régissent :

-   sujets de conversation autorisés, tolérés et bannis ;
-   règles de rédaction (par exemple pour spécifier les langues dans lesquelles les abonnés ont le droit d'écrire, pour interdire le « langage SMS », etc.) ;
-   règles régissant l'envoi des messages (fréquence, ajout de pièces jointes, etc.) ;
-   responsabilités des abonnés en matière de nétiquette ;
-   droits et devoirs des abonnés ;
-   information sur l'archivage des messages envoyés sur la liste ;
-   informations légales et politique de confidentialité ;
-   sanctions encourues en cas de non-respect de la charte d'utilisation de la liste ;
-   ~~etc.~~

| Note |
|------|
| Pour que tous les abonnés prennent connaissance de la charte d'utilisation de la liste, le mieux est de l'inclure dans le message de bienvenue qu'ils reçoivent lors de leur abonnement. Pour cela, vous devez [personnaliser ce message](#customize) en allant à la page 'Personnaliser' du module d'administration de la liste. |

Lorsqu'elle existe, la [Charte du propriétaire, animateur ou modérateur de liste](http://listes.cru.fr/cnil/charte.proprio.html "Exemple de charte destinée aux propriétaires et modérateurs") fournit aux propriétaires et aux modérateurs de listes toutes les informations indispensables pour pouvoir remplir leurs fonctions. Cette Charte recouvre l'ensemble des responsabilités et des attributions des propriétaires et modérateurs.

------------------------------------------------------------------------
