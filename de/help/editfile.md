Beschreibung der Service-Meldungen:
-   Willkommensnachricht: Diese Nachricht wird an neue Abonnenten gesendet. Es kann eine vollständig MIME strukturierte Nachricht sein (nur für MIME Gurus).
-   Abmeldenachricht: Diese Nachricht wird versendet, wenn Benutzer die Liste mittels des Befehls UNSUBSCRIBE verlassen.
-   Löschnachricht: Diese Nachricht wird Benutzern gesendet, wenn Sie sie mit dem Befehl DEL aus der Liste löschen (es sei denn, Sie verwenden den "leise"-Knopf).
-   Erinnerungsnachricht: Diese Nachricht wird jedem Abonnenten gesendet, der den REMIND-Befehl verwendet. Sie ist sehr hilfreich, wenn Benutzer sich über ihre Abonnements im Unklaren sind oder auch für Benutzer, die sich nicht selbst abmelden können.
-   Einladung zum Abonnement: Wird an einen Benutzer gesendet, wenn jemand den Befehl INVITE verwendet, um jemanden zum Abonnement einzuladen.

Beschreibung anderer Dateien/Seiten:
-   Homepage der Liste: HTML-Text als Beschreibung der Liste. Dieser wird auf der rechten Seite der Listen-Hauptseite angezeigt (Standardwert ist die Beschreibung der Liste).
-   Listenbeschreibung: Dieser Text wird als Antwort auf den Mailbefehl INFO verschickt. Er kann auch in der *Willkommensnachricht* enthalten sein.
-   Nachrichtenkopf: Wenn diese Datei nicht leer ist, wird sie als MIME Anlage am Beginn jeder Nachricht angehängt, die an die Liste verteilt wird.
-   Nachrichtenfuß: das Gleiche wie *Nachrichtenkopf*, wird aber am Ende der Nachricht angefügt.

