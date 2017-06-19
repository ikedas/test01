<span id="listconfig"></span>Configurer la liste
------------------------------------------------

Comme la configuration d'une liste est quelque peu complexe, sa présentation a été séparée en quatre parties :

-   [Définition de la liste](#description) ;
-   [Diffusion/réception](#sending) ;
-   [Droits d'accès](#command) ;
-   [Archives](#archives) ;
-   [Gestion des rapports de non-remise](#bounces) ;
-   [Divers](#other).

Nous vous conseillons d'**effectuer vos changements de configuration très progressivement** : ainsi, si le résultat ne correspond pas à vos attentes, vous pouvez plus facilement revenir en arrière.

Le module d'administration de la liste vous offre une **multitude d'options pour configurer votre liste**. Néanmoins, il se peut que ces options ne correspondent pas parfaitement à vos besoins. Pour remédier à ce problème, vous pouvez **faire appel aux listmasters pour qu'ils créent de nouvelles options** (dans la limite de leurs capacités) : accès et/ou droits restreints à certaines catégories de personnes en fonction de l'endroit d'où elles se connectent, du domaine auquel leur adresse e-mail appartient, du groupe d'utilisateur dont elles font partie, etc.

### <span id="description"></span>Définition de la liste

Dans la zone '**Objet de la liste**', vous pouvez modifier l'objet que vous aviez choisi lors de la création de la liste. Cet objet apparaît dans le bandeau bleu visible en haut de toutes les pages de la liste, ainsi que sur les pages d'index de listes (liste des listes, liste de vos abonnements, etc.) et dans la barre de titre du navigateur.

Vous pouvez également modifier la '**Visibilité de la liste**'. Les différentes options disponibles sont :

-   liste cachée sauf aux abonnés (conceal) - *option par défaut* ;
-   visible de l'intranet (intranet) ;
-   liste visible (noconceal) ;
-   liste cachée même aux abonnés (secret) ;

| Note |
|------|
| Si vous souhaitez restreindre la visibilité de la liste suivant d'autres critères, faites-en la demande aux listmasters : il est probable qu'ils puissent créer une nouvelle option correspondant à vos besoins (exemple : liste visible uniquement par les membres d'un groupe d'utilisateurs, d'un domaine internet, etc.). |

Dans les zones 'Propriétaires' et 'Modérateurs', vous pouvez **ajouter des propriétaires et des modérateurs** à la liste ou **modifier leurs informations** :

-   Pour chaque propriétaire/modérateur, vous devez obligatoirement saisir une **adresse e-mail** et un **nom**.
-   Vous pouvez également ajouter les informations de votre choix dans le champ '**Informations privées**' (numéro de téléphone, fonction, etc.) ; ces informations ne seront visibles que par les listmasters et les propriétaires de listes possédant un profil de type 'Privileged'.
-   Vous pouvez modifier le **mode de réception** des messages (les seules options disponibles sur cette page sont 'mail' et 'nomail').
-   Le paramètre 'Profil' n'est pas modifiable : le **profil 'Privileged'** est réservé au créateur de la liste (les autres propriétaires ont un profil du type 'Normal').

| Note |
|------|
| Attention : le fait de devenir propriétaire ou modérateur d'une liste n'implique pas d'être abonné automatiquement à cette liste. Les propriétaires et modérateurs doivent donc faire la démarche de s'abonner à la liste. |

Pour **supprimer des propriétaires/modérateurs**, effacez le contenu des champs de texte relatifs au propriétaire/modérateur que vous souhaitez supprimer et cliquez sur le bouton 'Mise à jour'.

Vous pouvez également modifier la **catégorie** de la liste ainsi que sa **langue**. Si vous changez la langue de la liste, tous les messages prédéfinis seront envoyés dans la langue choisie (attention : sous réserve que la traduction existe !).

Vous ne pouvez pas modifier le **domaine internet** de la liste : seul les listmasters peuvent modifier ce paramètre.

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.

### <span id="sending"></span>Diffusion/réception

À partir de cette page, vous pouvez tout d'abord **décider qui peut envoyer des messages sur la liste**.

Dans la zone '**Périodicité des compilations**', vous pouvez définir à quel intervalle sont envoyées les compilations de messages (modes de réception Compilation et Résumé) : sélectionnez dans la liste tous les **jours** pour lesquels vous souhaitez que des compilations soient envoyées. Choisissez ensuite un **horaire d'envoi** des compilations (évitez de choisir un horaire compris entre 23h et minuit).

Dans la liste '**Options d'abonné disponibles**', sélectionnez toutes les options d'abonné que vous souhaitez offrir à vos abonnés. Par défaut, toutes les options sont sélectionnées.

La zone '**Adresse de réponse**' vous permet de définir les destinataires par défaut lors d'une réponse à un message envoyé sur la liste :

-   Lorsque la valeur choisie est '**All**', la réponse est envoyée à l'**expéditeur du message** ET à la **liste**.
-   Lorsque la valeur choisie est '**List**', la réponse est envoyée à la **liste**.

    | Note |
    |------|
    | Attention : cette option est à utiliser avec précaution ! L'expérience montre que les abonnés ne vérifient pas toujours l'adresse à laquelle ils expédient leur réponse. Ils risquent donc d'envoyer des messages privés à l'ensemble des abonnés en pensant répondre uniquement à une personne... |

-   Lorsque la valeur choisie est '**Other\_email**', la réponse est envoyée à une **adresse prédéfinie**. Si vous choisissez cette option, vous devez **saisir une adresse e-mail dans le champ 'Autre adresse email'**.
-   Lorsque la valeur choisie est '**Sender**', la réponse est envoyée à l'**expéditeur du message**. C'est la valeur que nous vous conseillons de choisir.

La liste déroulante '**Respect du champ existant**' vous permet de choisir le traitement du champ d'en-tête SMTP 'Reply-To' dans les messages entrants. L'option '**Respect**' préserve ce champ tandis que l'option '**Forced**' permet de l'écraser.

Enfin, l'option '**Marquage du sujet des messages**' permet de choisir le **texte qui sera inséré devant l'objet de tous les messages** envoyés sur la liste : ceci permet aux abonnés de pouvoir trier leurs messages plus facilement, de leur appliquer des filtres de messages, etc. Par défaut, ce texte est constitué du **nom de la liste entouré de crochets** (les crochets sont rajoutés automatiquement par le système, il est inutile de les indiquer vous-même).

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.

### <span id="command"></span>Droits d'accès

À partir de cette page, vous pouvez décider :

-   **qui a accès aux informations sur la liste**. Les options disponibles sont les suivantes :
    -   pour tous (open) - *option par défaut* ;
    -   réservé aux abonnés (private).
-   **qui peut s'abonner à la liste**. Les options disponibles sont les suivantes :
    -   demande d'abonnement après confirmation (auth) ;
    -   soumis à authentification (notification des proprios) (auth\_notify) ;
    -   soumis à authentification puis accord du proprio (auth\_owner) ;
    -   abonnement impossible (closed) ;
    -   les abonnés ou le domaine local (intranet) ;
    -   usager du domaine local ou via autorisation du proprio (intranetorowner) ;
    -   ouvert à tous sans authentification (open) - *option par défaut* ;
    -   ouvert à tous, notification du propriétaire (open\_notify) ;
    -   n'importe qui pas de bienvenue (open\_quiet) ;
    -   ouvert à tous après autorisation du proprio (owner) ;
    -   demande d'abonnement avec signature par certificat (smime) ;
    -   ouvert à tous après autorisation du proprio ou avec signature par certificat (smimeorowner).

        | Note |
        |------|
        | Il est conseillé de toujours choisir une option comportant le paramètre 'auth' : ainsi, le système demandera confirmation par e-mail au futur abonné avant de l'abonner à la liste. Ceci permet d'éviter des abonnements avec une adresse e-mail invalide et assure que personne ne peut être abonné à la liste à son insu. |

-   **qui peut se désabonner de la liste**. Les options disponibles sont les suivantes :
    -   possible après authentification (auth) ;
    -   authentification demandée, notification du proprio (auth\_notify) ;
    -   impossible (closed) ;
    -   autorisé à tous sans authentification (open) - *option par défaut* ;
    -   pas d'authentification (notification au proprio) (open\_notify) ;
    -   soumis à autorisation du proprio (owner).

        | Note |
        |------|
        | Il est conseillé de toujours choisir une option comportant le paramètre 'auth' : ainsi, le système demandera confirmation par e-mail à l'abonné avant de le désabonner. Ceci permet d'éviter que des personnes malintentionnées ne désabonnent des abonnés à leur insu. |

-   **qui peut inviter une nouvelle personne à s'abonner à la liste**. Les options disponibles sont les suivantes :
    -   fermé (closed) ;
    -   invitation par le proprio sans authentification (owner) ;
    -   limité aux abonnés (private) - *option par défaut* ;
    -   ~~public (public).~~
-   **qui a accès à la liste des abonnés**. Les options disponibles sont les suivantes :
    -   pour personne (closed) ;
    -   limité aux abonnés ou aux utilisateurs du domaine local (intranet) ;
    -   listmaster seulement (listmaster) ;
    -   proprio de liste seulement (et listmaster) (owner) - *option par défaut* ;
    -   limité aux abonnés (private) ;
    -   accessible à tous (public).

        | Note |
        |------|
        | Il est fortement déconseillé de rendre la liste des abonnés accessible à tous. L'option 'Réservé aux abonnés' peut être intéressante afin de permettre à ceux-ci de communiquer entre eux sans passer par la liste. Cette option est néanmoins à éviter dans le cas d'une liste de type annonce regroupant des abonnés sans aucun lien entre eux. |

<span id="docsrights"></span>Sur cette page, vous pouvez également **définir les droits relatifs à l'espace de stockage partagé** (section 'Documents' de la liste, accessible via un lien dans le menu de gauche). On distingue les droits de consultation et les droits d'édition des documents :

Pour les **droits de consultation**, les options suivantes sont disponibles :

-   limité aux abonnés ou aux utilisateurs du domaine local (intranet) ;
-   limité aux propriétaires de la liste (owner) ;
-   limité aux abonnés (private) - *option par défaut* ;
-   documents publics (public).

Pour les **droits d'édition**, les options suivantes sont disponibles :

-   limité aux propriétaires de la liste (owner) - *option par défaut* ;
-   modéré pour les abonnés (editor) ;
-   limité aux abonnés (private) ;
-   documents publics (public).

La zone de texte '**Quota**' vous permet de définir une **taille maximale à ne pas dépasser pour l'espace de stockage partagé**. Cette taille ne représente pas la taille maximale d'*un* document publié dans l'espace de stockage partagé, mais bien celle de l'ensemble des documents publiés sur la liste. Elle est exprimée en kilo-octets. Lorsqu'un abonné tente de publier un fichier trop gros par rapport à l'espace restant, il reçoit un message d'erreur.

Pour **plus d'informations sur la gestion de l'espace de stockage partagé** (organisation de l'espace de stockage partagé, modification des droits d'accès, etc.), reportez-vous à la section [Utiliser l'espace de stockage partagé](shared.md) du Guide de l'utilisateur.

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.

### <span id="archives"></span>Archives

À partir de cette page, vous pouvez **décider qui peut accéder aux archives de la liste en ligne** (messages envoyés consultables sur l'interface web du serveur de listes). Les différentes options disponibles sont :

-   fermé (closed) ;
-   les abonnés ou le domaine local (intranet) ;
-   listmaster (listmaster) ;
-   proprio de liste (owner) ;
-   les modérateurs (moderator) ;
-   les abonnés seulement (private) ;
-   ~~public (public).~~

La zone de texte '**Quota**' vous permet de définir une **taille maximale à ne pas dépasser pour les archives de messages**. Cette taille est exprimée en kilo-octets. Les propriétaires reçoivent une notification lorsque les archives atteignent 95 % de la taille autorisée. Si la taille maximale dévolue aux archives est atteinte, les messages ultérieurs ne sont pas archivés.

| Note |
|------|
| Même si les messages cessent d'être archivés, il reste évidemment possible d'envoyer des messages sur la liste. |

Il est également possible d'**accéder aux archives de la liste par e-mail**, en envoyant à **{{conf.email}}** la commande suivante : <span class="commande">**GET nomdelaliste annee-mois**</span> (exemple : *GET cri-exemple 2016-07*). L'abonné reçoit alors une compilation de tous les messages envoyés au cours du mois choisi. Cette compilation est envoyée en texte brut et contient des balises HTML à la place du formatage d'origine ; elle comprend également des en-têtes détaillés pour chaque message. Le paramètre '**Archives textuelles**' vous permet de définir :

-   **qui a le droit** de se faire envoyer par e-mail les archives récapitulatives des messages de la liste ;
-   la **périodicité de création de ces archives**. Par exemple, si la périodicité est 'month', l'ensemble des messages envoyés sur la liste en un mois sera regroupé dans un message d'archives unique qui pourra être demandé par e-mail au serveur.

Si ce paramètre n'est pas défini, la liste n'aura aucune archive consultable par e-mail. Attention : **seuls les listmasters ont le pouvoir de modifier ce paramètre.**

Il est possible d'envoyer des **messages cryptés au format S/MIME** sur la liste. L'option '**Archivage des messages cryptés**' vous permet de définir comment ces messages vont être archivés :

-   L'option '**Decrypted**' archive le message sans qu'il ne soit chiffré.
-   L'option '**Original**' archive le message sous sa forme originale.

Cette option s'applique à la fois aux archives de messages textuelles et aux archives en ligne, ainsi qu'aux compilations de messages envoyées aux personnes qui ont souscrit leur abonnement avec le mode de réception Digest.

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.

### <span id="bounces"></span>Gestion des rapports de non-remise

Les « **bounces** » représentent les **abonnés en erreur**, c'est-à-dire les abonnés qui ne reçoivent pas les messages envoyés sur la liste. Les raisons peuvent être variées : adresses qui n'existent plus, adresses momentanément indisponibles au moment de l'envoi de messages, capacité de la boîte de réception atteinte, etc.

La section '**Gestion des erreurs**' définit deux seuils :

-   Le **seuil d'alerte** indique le taux d'abonnés en erreur à partir duquel le propriétaire de la liste recevra une **notification intitulée 'Taux de bounces trop élevé'** l'invitant à supprimer de sa liste les abonnés en erreur.
-   Le **seuil d'interruption** indique le taux d'erreurs à partir duquel **la distribution des messages de la liste sera automatiquement interrompue** jusqu'à régularisation de la situation (généralement via la suppression des abonnés en erreur).

<span id="bouncers"></span>Les sections '**bouncers\_level1**' et '**bouncers\_level2**' permettent d'effectuer automatiquement des actions en direction des abonnés en erreur. Vous pouvez définir :

-   les **plages de scores qui définissent les bouncers de niveau 1 et de niveau 2**. Par défaut, les bouncers de niveau 1 ont un score compris entre 45 et 74 et les bouncers de niveau 2 ont un score compris entre 75 et 100 ;

    | Note |
    |------|
    | Le score est déterminé par le nombre, le type et la fréquence des erreurs. Si la période de réception des erreurs est trop courte ou s'il n'y a pas eu beaucoup d'erreurs, aucun score n'est affecté au bouncer. |

-   l'**action à effectuer en direction des abonnés concernés** : aucune action, notification, suppression de la liste des abonnés ;
-   la **personne à notifier** lorsqu'une action est entreprise : personne, les propriétaires de la liste, les listmasters. La notification envoyée lorsqu'une action est effectuée en direction des abonnés en erreur comprend les adresses de tous les abonnés concernés ainsi que le détail de l'action effectuée.

**Pour gérer les erreurs** (annuler les erreurs pour certains abonnés, désabonner les abonnés en erreur, demander un rappel des abonnements, etc.), **allez à la page** '[Erreurs](admin#manage_bounces.md)' du module d'administration de la liste.

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.

### <span id="other"></span>Divers

L'option '**Expire\_task**' vous permet de définir un **délai d'expiration automatique des abonnements** à la liste : à intervalles réguliers (exemple : une fois par an), les abonnés recevront un message leur demandant de renouveler leur abonnement à la liste. S'ils ne le renouvellent pas, ils seront automatiquement désabonnés. Cette procédure permet de s'assurer que toutes les personnes abonnées à la liste sont réellement concernées et intéressées.

L'option '**Remind\_task**' vous permet d'**envoyer des rappels d'abonnements à intervalles réguliers** à tous les abonnés de la liste.

L'option '**Méthode de protection des adresses contre les robots spammeurs**' permet d'éviter que les adresses e-mail des abonnés ne soient récupérées par des robots à des fins de spam. Cette option est valable pour l'ensemble des pages relatives à la liste.

Sur cette page, vous pouvez également voir des **informations sur la dernière mise à jour de la liste** (qui l'a effectuée et à quelle date) ainsi que sur le **nombre de changements de configuration** depuis la création de la liste.

**ATTENTION : n'oubliez pas de cliquer sur 'Mise à jour'** au bas de la page pour enregistrer tous vos changements.
