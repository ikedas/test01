Liste der Befehle der Sympa-Mailoberfläche
------------------------------------------

Alle Befehle müssen an {{conf.email}}@{{conf.host}} geschickt werden.

Es ist möglich, mehrere Befehle in einer einzelnen Nachricht zu schicken. Befehle müssen dann in den Nachrichtenrumpf eingetragen werden (ein Befehl pro Zeile).

### Befehle für Benutzer

`HELP`: eine Liste aller verfügbaren Befehle abfragen

`LISTS`: eine Liste aller auf dem Server verwalteten Listen abfragen

`WHICH`: eine Liste aller durch Sie abonnierten Listen abfragen

`CONFIRM schlüssel`: das Senden einer Nachricht bestätigen (je nach Konfiguration der Liste)

`QUIT`: bezeichnet das Ende der Befehlssequenz (nützlich, um eine Signatur zu ignorieren)

`INFO liste`: Informationen über die Liste abfragen

`REVIEW liste`: eine Liste aller Listenabonnenten abfragen

`SUBSCRIBE liste name`: Abonnement einer Liste (oder Bestätigung eines Abonnements)

`INVITE liste e-mail`: jemanden dazu einladen, die Liste zu abonnieren

`UNSUBSCRIBE liste e-mail`: die Liste abbestellen. Die E-Mail-Adresse wird nur benötigt, wenn Sie sich unter einer anderen Adresse aus der Liste austragen wollen als der Absenderadresse der Nachricht

`UNSUBSCRIBE * e-mail`: alle abonnierten Listen abbestellen

`SET liste NOMAIL`: Erhalt von Nachrichten der Liste stoppen

`SET liste DIGEST`: Nachrichten als Kompilat erhalten

`SET liste DIGESTPLAIN`: Nachrichten als Kompilat in reinem Textformat erhalten

`SET liste SUMMARY`: nur Nachrichtenauflistungen erhalten

`SET liste NOTICE`: nur Nachrichtenbetreffzeilen erhalten

`SET liste MAIL`: normale Nachrichtenauslieferung

`SET liste CONCEAL`: Adresse in der Abonnentenliste verbergen

`SET liste NOCONCEAL`: Adresse in der Abonnentenliste (REVIEW-Befehl) sichtbar machen

`INDEX liste`: eine Liste der Archivdateien abfragen

`GET liste datei`: eine Datei aus dem Listenarchiv abrufen

`LAST liste`: die letzte über die Liste versandte Nachricht abfragen

### Befehle für Listeneigentümer

`ADD liste e-mail name`: einen Abonnenten zur Liste hinzufügen

`DEL liste e-mail`: einen Abonnenten aus der Liste austragen

`STATS liste`: die Statistiken der Liste abfragen

`REMIND liste`: an alle Abonnenten eine personalisierte Erinnerung mit der Adresse, unter der die Liste abonniert wurde, schicken

### Befehle für Listenmoderatoren

`DISTRIBUTE liste schlüssel`: eine Nachricht akzeptieren

`REJECT liste schlüssel`: eine zu moderierende Nachricht ablehnen

`MODINDEX liste`: die Liste der noch zu moderierenden Nachrichten abrufen
