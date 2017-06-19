Les listes de diffusion - Introduction générale
-----------------------------------------------

### Qu'est-ce qu'une liste de diffusion ?

Une liste de diffusion est une **liste d'envoi permettant à un groupe d'abonnés de recevoir automatiquement par courrier électronique l'ensemble des messages expédiés à la liste** : tout message envoyé à la liste par un abonné est reçu par chacun des autres abonnés. Lorsque l'on est abonné à une liste de diffusion, il est possible d'envoyer des messages, d'y répondre ou de lire les messages envoyés sans participer.

**Cas particuliers :**

-   Il est parfois possible d'envoyer des messages à une liste de diffusion sans y être abonné. Néanmoins, il faut impérativement être abonné à la liste pour en recevoir les messages.
-   Il est parfois impossible d'envoyer des messages à la liste même lorsque l'on y est abonné : c'est le cas pour les listes de type annonce, qui servent à diffuser des informations d'un émetteur unique vers un grand nombre de destinataires.

### Intérêt des listes de diffusion

On s'abonne à une liste de diffusion (ou « *mailing list* », parfois abrégée en ML) pour **se tenir au courant d'un sujet en particulier** et pour **participer à des échanges sur ce sujet**. On peut citer en exemple :

-   liste de diffusion à destination de tous les employés d'une entreprise ;
-   liste de diffusion réservée aux participants d'un projet ;
-   liste de diffusion regroupant tous les étudiants d'une promotion ;
-   liste de diffusion sur l'actualité de la sécurité informatique ;
-   liste de diffusion d'entraide entre bricoleurs ;
-   liste de diffusion restreinte à une famille et destinée à organiser les grands rassemblements familiaux ;
-   etc. !

### Types de listes de diffusion

Il existe **des milliers de listes de diffusion** de toutes sortes sur Internet : publiques ou privées, gratuites ou payantes, avec inscription soumise à conditions ou non, etc. Ces listes peuvent rassembler un nombre de personnes allant d'une dizaine à plusieurs milliers.

En fonction de leur mode de fonctionnement, on distingue généralement **deux types de listes** :

-   Les **listes de type annonce** permettent aux abonnés de recevoir des messages sans pouvoir en poster eux-mêmes. Il s'agit en fait de lettres d'information (ou « newsletters ») : magazines électroniques, services quotidiens (horoscope du jour, météo du jour, alerte de sécurité du jour, etc.), bulletins d'informations sur les mises à jour d'un site, etc. Avec ce type de liste de diffusion, l'information circule d'un émetteur vers un grand nombre de destinataires.
-   Les **listes de type discussion** permettent à tous les abonnés de participer. Ces listes peuvent être modérées ou non modérées :
    -   Dans une **liste de discussion modérée**, les messages sont transmis à tous les abonnés après validation par un des modérateurs de la liste. La modération est un gage de qualité pour la liste. Elle garantit, par exemple, que les abonnés ne recevront pas de messages hors-sujet, de sollicitations commerciales non désirées (spams), de messages contenant des pièces jointes volumineuses, etc.
    -   Dans une **liste de discussion non modérée**, les messages sont transmis à tous les abonnés dès réception par l'automate de gestion de listes.

### <span id="features"></span>Fonctionnalités proposées

Une fois abonné à un service de listes, vous pouvez :

-   **chercher des listes de diffusion** correspondant à vos centres d'intérêts ou à votre situation particulière ;
-   **gérer vos abonnements** :
    -   [vous abonner](user.md#subscribe) à des listes,
    -   [vous désabonner](user.md#unsubscribe) de listes auxquelles vous êtes abonné,
    -   modifier vos [options d'abonné](user.md#options) liste par liste,
    -   modifier vos [préférences générales](user.md#pref) relatives à votre environnement de listes (nom, mot de passe, langue de l'interface web du serveur de listes, etc.) ;
-   **utiliser des listes de diffusion** ::
    -   consulter les [archives des listes auxquelles vous n'êtes pas abonné](arc.md) (c'est-à-dire lire en ligne les archives des messages envoyés sur ces listes) si ces archives sont publiques et que vos droits vous permettent d'accéder à ces listes,
    -   consulter les [archives des listes auxquelles vous êtes abonné](arc.md),
    -   effectuer des [recherches dans les archives des listes](arc.md#arcsearch),
    -   [envoyer des messages](sendmsg.md) aux listes auxquelles vous êtes abonné,
    -   [télécharger des documents](shared.md#shared_read) à partir de l'espace de stockage partagé,
    -   [publier des documents](shared.md#publishdoc) dans l'espace de stockage partagé ;
-   **administrer des listes de diffusion** ::
    -   [créer de nouvelles listes](admin.md#create_list) (accès restreint) - soumis à autorisation,
    -   [configurer](admin.md#edit_list) des listes dont vous êtes propriétaire,
    -   [gérer des abonnements](admin.md#manage_members),
    -   [gérer l'espace de stockage partagé](admin.md#manage_shared),
    -   [modérer](admin.md#moderate) des listes dont vous êtes modérateur.

### <span id="roles"></span>Fonctionnement des listes de diffusion : qui fait quoi ?

Quatre rôles peuvent intervenir dans un service de listes de diffusion :

-   **listmaster ;**
-   **propriétaire ;**
-   **modérateur ;**
-   **abonné.**

Il est possible de jouer plusieurs rôles à la fois (par exemple, il est possible d'être propriétaire et modérateur d'une liste et d'être abonné à plusieurs autres).

#### ~~Listmasters~~

Les listmasters sont les personnes qui s'occupent de la **gestion d'un service de listes**. Leurs rôles :

-   **administrer le serveur de listes de diffusion** (mise en place, maintenance, etc.) ;
-   **définir les orientations générales du service de listes de diffusion** :
    -   qui aura l'autorisation de demander la création d'une nouvelle liste,
    -   quelles seront les options disponibles pour l'administration des listes (définition de scénarii),
    -   que contiendront les fichiers par défaut (création de modèles),
    -   à quoi ressemblera l'interface web du serveur de listes de diffusion ;
-   **établir les règles d'utilisation** du service de listes de diffusion et **les documenter en rédigeant des chartes d'utilisation** à destination des abonnés, des modérateurs et des propriétaires ;
-   **valider les demandes de création de listes de diffusion**  ;
-   **se substituer temporairement aux propriétaires de listes** en cas de besoin ; en revanche, les listmasters ne sont pas censés se substituer aux modérateurs.

**Les propriétaires et modérateurs de listes peuvent s'appuyer sur les listmasters** en cas de problème non traité dans la documentation ou pour toute remarque. Néanmoins, afin que les listmasters ne soient pas submergés de messages, il est préférable que les simples abonnés s'adressent plutôt aux propriétaires de listes.

#### Propriétaires

**Le propriétaire d'une liste est généralement son créateur**, ou à défaut, la personne qui a exprimé le souhait que la liste soit créée ou qui en a hérité. **Son rôle** :

-   **définir le [mode de fonctionnement](admin.md#edit_list) de la liste** ;
-   **rédiger une [charte d'utilisation](admin.md#charter)** de la liste à destination des abonnés ;
-   **désigner un ou plusieurs modérateur(s)** ;
-   **gérer les [abonnements et désabonnements](admin.md#manage_members)** ;
-   **décider de mettre ou non à la disposition des abonnés un [espace de stockage partagé](admin.md#manage_shared)** ;
-   **répondre aux questions des abonnés et futurs abonnés à propos de la liste ;**
-   ~~etc.~~

Une liste peut avoir plusieurs propriétaires. Néanmoins, le **profil 'Privileged'** est réservé au créateur de la liste ; les autres propriétaires ont un profil du type 'Normal', qui possède moins de prérogatives.

#### Modérateurs

**Les modérateurs sont désignés par le propriétaire de la liste**. Ils sont **chargés de [réguler la diffusion des messages](admin.md#moderate)** envoyés sur la liste : après lecture, **ils peuvent décider de les accepter ou de les rejeter**. La modération intervient avant la diffusion du message sur la liste. Le rejet d'un message est éventuellement suivi d'une notification à l'expéditeur du message afin de l'informer des raisons de ce rejet.

Une liste peut avoir **un ou plusieurs modérateurs** ; généralement, le propriétaire de la liste en est aussi le modérateur.

Ceci ne concerne que les listes modérées.

### <span id="policy"></span>Cadre réglementaire

L'utilisation d'un service de listes de diffusion implique le respect d'un certain nombre de règles :

-   Dans la plupart des services de listes, les abonnés reçoivent lors de leur abonnement une charte des abonnés de la liste. Ils sont alors tenus de respecter l'ensemble des règles contenues dans cette charte.
-   Si elle est disponible, les modérateurs doivent se conformer à la charte des propriétaires et des modérateurs.
-   L'utilisation des listes de diffusion implique de respecter les règles de bonne utilisation de la messagerie (la « Nétiquette »).

Pour en savoir plus, reportez-vous à la section consacrée aux [bonnes pratiques des propriétaires et modérateurs](admin.md#rulesadmin).

------------------------------------------------------------------------
