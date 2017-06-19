Description des messages de service :
-   Message de bienvenue : Ce message est envoyé aux nouveaux abonnés. Vous pouvez utiliser un message MIME structuré (réservé aux experts du format MIME).
-   Message de désabonnement : Envoyé aux personnes qui se désabonnent de la liste.
-   Message de suppression : Envoyé aux personnes supprimées de la liste des abonnés par le propriétaire de la liste (sauf s'il active l'option « quiet ») ou via le module de gestion des erreurs.
-   Message de rappel individualisé : Message envoyé à chaque abonné lors du rappel des abonnements. Ce message peut être envoyé depuis l'interface d'administration de liste dans la page *abonnés* ou via la commande REMIND. Cette procédure est très utile pour aider chaque personne à se désabonner au cas où celles-ci ne connaissent plus leur adresse d'abonnement.
-   Invitation à s'abonner : Message envoyé à une personne via la commande `INVITE [nom de liste]`.

Description des autres fichiers/pages :
-   Page d'accueil de la liste : Description de la liste au format HTML. S'affiche en partie droite de la page de la liste. (a pour défaut la description de la liste)
-   Description de la liste : Ce texte accompagne la réponse à la commande mail `INFO`. Il peut également être inclus dans le *message de bienvenue*.
-   Attachement de début de message : Si non vide, ce fichier est attaché au début de chaque message diffusé dans la liste.
-   Attachement de fin de message : Identique à l'*Attachement de début de message* mais attaché en fin de message.

