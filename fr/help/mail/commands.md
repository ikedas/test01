Liste des commandes de l'interface mail de Sympa
------------------------------------------------

Toutes les commandes doivent être adressées à l'adresse {{conf.email}}.

Il est possible de mettre plusieurs commandes dans chaque message. Les commandes doivent apparaître dans le corps du message et chaque ligne ne doit contenir qu'une seule commande.

### Les commandes pour les utilisateurs

`HELP` : recevoir la liste des commandes disponibles

`LISTS` : recevoir l'annuaire des listes gérées sur ce serveur

`WHICH` : recevoir la liste des listes auxquelles vous êtes abonné

`CONFIRM cle` : confirmer l'envoi d'un message (selon la configuration de la liste)

`QUIT` : indique la fin des commandes (pour ignorer une signature)

`INFO liste` : obtenir des informations sur une liste

`REVIEW liste` : recevoir la liste des abonnés à la liste

`SUBSCRIBE liste nom` : abonnement (ou confirmation d'abonnement) à la liste

`INVITE liste email` : inviter une personne à s'abonner à la liste

`UNSUBSCRIBE liste email` : se désabonner de la liste. L'adresse email est optionnelle ; uniquement requise si vous voulez vous désabonner d'une adresse différente de votre adresse courante

`UNSUBSCRIBE * email` : se désabonner de toutes les listes auxquelles vous êtes abonné

`SET liste NOMAIL` : suspendre la réception des messages de la liste

`SET liste DIGEST` : recevoir les messages en mode compilation

`SET liste DIGESTPLAIN` : recevoir les messages en mode compilation (fichier texte)

`SET liste SUMMARY` : recevoir la liste des messages uniquement

`SET liste NOTICE` : recevoir l'objet des messages uniquement

`SET liste MAIL` : mode de réception normal des messages

`SET liste CONCEAL` : passage en liste rouge (adresse d'abonné cachée)

`SET liste NOCONCEAL` : adresse d'abonné visible via REView

`INDEX liste` : recevoir la liste des fichiers des archives

`GET liste fichier` : obtenir un fichier des archives de la liste

`LAST liste` : recevoir le dernier message de la liste

### Les commandes pour les propriétaires

`ADD liste email nom` : ajouter un membre à la liste

`DEL liste email` : supprimer un utilisateur de la liste

`STATS liste` : consulter les statistiques de la liste

`REMIND liste` : envoyer à chaque abonné un message personnalisé lui rappelant l'adresse avec laquelle il est abonné

### Les commandes pour les modérateurs

`DISTRIBUTE liste cle` : valider un message

`REJECT liste cle` : rejeter un message à modérer

`MODINDEX liste` : consultation de la liste des messages à modérer
