<span id="docadmin"></span>Mailinglisten - Handbuch für Eigentümer und Moderatoren
----------------------------------------------------------------------------------

### Einführung: Wer ist für die Verwaltung von Mailinglisten zuständig?

Erinnerung: Ein Mailinglistendienst kennt vier verschiedene Rollen:

-   **Listmaster;**
-   **Eigentümer;**
-   **Moderator;**
-   **Abonnent.**

Betrachten Sie die [Beschreibung der jeweiligen Rolle,](introduction#roles.md) um mehr hierüber zu erfahren.

### <span id="create_list"></span>Das Erstellen einer Mailingliste beantragen

Der **Antrag zum Einrichten einer Mailingliste** kann **bestimmten Bedingungen unterliegen.** Auch wenn Sie diese Bedingungen einhalten, erfordert das **Erstellen einer Liste** trotzdem die **Zustimmung durch einen Listmaster.**

Um das Erstellen einer Mailingliste zu beantragen, gehen Sie folgendermaßen vor:

1.  Gehen Sie zur **[Homepage der WWW-Listenoberfläche](%7B%7Bpath_cgi%7D%7D/home)** und [**melden Sie sich an.**](user#sympa_auth.md)
2.  Wählen Sie im oberen Menü **'Liste anlegen'.**

    | Note |
    |------|
    | Falls dieser Link nicht angezeigt ist, heißt dies, dass Sie nicht berechtigt sind, eine Liste anzulegen. |

3.  Geben Sie Ihrer Liste einen **Namen** (nur den Namen ohne '@' und den Domainnamen; Beispiel: *schneckenzucht* und nicht *schneckenzucht@{{conf.host}}*.)

    | Note |
    |------|
    | Verwenden Sie keine Leerzeichen, Akzente oder Sonderzeichen in Listennamen: diese Zeichen könnten Schwierigkeiten machen. |

    | Note |
    |------|
    | Wählen Sie einen ausdrucksstarken, aber kurzen Namen: Denken Sie an die Abonnenten, die diesen Namen jedes Mal, wenn sie eine Nachricht an die Liste schicken, eintippen müssen! Wenn Sie eine Reihe von Listen verwalten, können Sie Ihre Listennamen mit einem gemeinsamen Präfix versehen; sie werden dann nahe beieinander sortiert und sind leicht erkennbar (Beispiel: *xx-nutzer@{{conf.host}}, xx-stab@{{conf.host}}* etc.). |

4.  Wählen Sie einen **Listentypen** unter den vordefinierten Typen (die vordefinierten Typen sind nur Beispiele typischer Konfigurationen, die von den Listeneigentümern nach dem Erstellen geändert werden können; es ist sogar möglich, die Listen über die auf der Administrationsseite hinaus sichtbaren Optionen zu konfigurieren, indem man einen Listmaster darum bittet).
5.  Geben Sie ein **Thema** für Ihre Liste an. Dieses Thema wird als Kopfzeile für alle Listenseiten angezeigt; es dient auch als Bezeichnung in den Listenindexseiten (Listenübersicht, Abonnementübersicht etc.) und in der Titelseite des Browserfensters.
6.  Wählen Sie einen **Themenbereich** im Menü 'Themenbereiche'.

    | Note |
    |------|
    | Falls Ihnen kein Themenbereich zusagt, können Sie einen Listmaster darum bitten, ein neues Themengebiet einzurichten. |

7.  Geben Sie eine **Beschreibung** Ihrer Liste ein. Diese Beschreibung wird auf der Informationsseite der Liste und in der 'Abonnentencharta', die jedem neuen Abonnenten per Mail zugeschickt wird, unter der Überschrift 'Listenthema' angezeigt. Die Beschreibung kann beispielsweise Folgendes erklären:

    -   Gegenstand und Zweck der Liste;
    -   besprochene Themen;
    -   Listenbetrieb (Pflichten, Betriebszustand, etc.);
    -   geltende Regeln;
    -   Beschreibung typischer Abonnenten (Beschäftigung, Projekte, Nationalitäten etc.).

    | Note |
    |------|
    | Sie können Ihre Listenbeschreibung mit HTML-Tags formatieren. Seien Sie vorsichtig: Brechen Sie bei einer langen Beschreibung die Zeilen mit manuellen Zeilenumbrüchen um (ENTER-Taste auf Ihrer Tastatur); ansonsten passt sie eventuell nicht ganz ins Browserfenster. |

8.  Klicken Sie auf den Knopf **'Anfrage zur Listenerzeugung absenden'.**

Eine Nachricht wird angezeigt, um Sie zu informieren, dass Ihre Erzeugungsanfrage an die Listmasters geschickt wurde und dass Sie von nun an die Liste per Klick auf den 'Admin'-Knopf bearbeiten können. Die Nachricht warnt Sie allerdings auch, dass die Liste auf dem Server erst dann installiert und sichtbar gemacht wird, wenn ein Listmaster sie freigegeben hat.

Sie müssen hiernach **darauf warten, dass die Listenerzeugung durch einen Listmaster freigegeben wird.** Sie erhalten dann eine Benachrichtigung mit dem Betreff **'Erstellung der Mailingliste listenname',** die Sie darüber informiert, dass die Liste tatsächlich angelegt wurde.

**Abonnieren Sie als letzten Schritt die Liste:** Wenn Sie eine Liste anlegen oder zu ihrem Eigentümer oder Moderator ernannt werden, heißt dies nicht, dass Sie automatisch auch abonniert sind!

### Eine Liste verwalten

Um eine Liste, die Ihnen gehört, zu verwalten, gehen Sie folgendermaßen vor:

1.  Gehen Sie zur **Homepage der WWW-Listenoberfläche** und **[melden Sie sich an.](user#sympa_auth.md)**

    | Note |
    |------|
    | Wenn Sie die Liste unter mehreren Adressen abonniert haben, verwenden Sie die Adresse, unter der Sie die Erzeugung der Liste beantragt haben. |

2.  **Gehen Sie zur Informationsseite der Liste,** die Sie verwalten möchten.
3.  Klicken Sie im linken Menü auf den **'Admin'-Link.**

Um die Abschnitte des Administrationsmoduls zu durchblättern, klicken Sie auf die Links unter dem 'Admin'-Link im linken Menü.

In diesen verschiedenen Abteilungen können Sie:

-   [die Liste konfigurieren;](listconfig.md)
-   [zur Liste gehörige Dateien anpassen;](#customize)
-   [Abonnenten verwalten;](#manage_members)
-   [die Nachrichtenarchive der Liste verwalten;](#manage_archives)
-   [Zustellfehler verwalten;](#manage_bounces)
-   [den Bereich für gemeinsame Dokumente anlegen, löschen oder wiederherstellen;](#manage_shared)
-   [die Liste umbenennen;](#renamelist)
-   [die Liste löschen.](#supprlist)

Mit den im Untermenü 'Moderieren' verfügbaren Optionen können Sie:

-   an die Liste geschickte [Nachrichten moderieren;](#moderate)
-   im Bereich für gemeinsame Dokumente verfügbare [Dokumente moderieren;](shared.md)
-   [anstehende Abonnements moderieren.](#manage_members)

#### <span id="edit_list"></span>Die Liste konfigurieren:

Um zu erfahren, wie Sie die Liste konfigurieren können, betrachten Sie bitte die [**Dokumentation zur Listenkonfiguration.**](listconfig.md)

#### <span id="customize"></span>Die Liste anpassen

Auf dieser Seite können Sie **diverse Dateien bearbeiten, die zu Ihrer Liste gehören,** darunter:

-   typische Nachrichten, die zu bestimmten Anlässen an Benutzer geschickt werden:
    -   **Willkommensnachricht**: Diese Nachricht ist die Benachrichtigung, die frisch angemeldete Abonnenten erhalten. Sie sollten eine Charta für Ihre Liste schreiben und sie zu dieser Willkommensnachricht hinzufügen. Sie können hierfür eine strukturierte MIME-Nachricht erstellen (dies ist MIME-Experten vorbehalten);
    -   **Nachricht beim Austragen:** Diese Nachricht wird an Abonnenten geschickt, die die Liste abbestellen;
    -   **Löschnachricht:** Diese Nachricht wird an Abonnenten geschickt, die Sie von der Liste genommen haben (Befehl DEL), besonders falls ihre Adresse Zustellfehler verursacht hat;
    -   **Erinnerungsnachricht:** Diese Nachricht wird Abonnenten als persönliche Erinnerung geschickt, wenn der REMIND-Befehl verwendet wird. Dieser Befehl ist für eine gute Listenverwaltung unverzichtbar, da viele Zustellfehler auf Abonnenten zurückgehen, deren aktuelle Adresse nicht mehr die Adresse ist, unter der sie die Liste abonniert haben, oder die gar vergessen haben, dass sie die Liste überhaupt abonniert haben;
    -   **Einladungsnachricht:** Diese Nachricht erhalten Personen, die mittels des INVITE-Befehls eingeladen wurden, die Liste zu abonnieren;
    -   **Moderator-Ablehnungsnachricht:** Diese Nachricht erhält der Absender einer vom Moderator zurückgewiesenen Nachricht;
    -   **Virus-Ablehnungsnachricht:** diese Nachricht erhält der Absender einer Nachricht, in der ein Virus gefunden wurde.
-   Verschiedene Dateien:
    -   **Listenbeschreibung:** Die Listenbeschreibung wird per Mail nach Aufforderung durch einen INFO-Befehl verschickt. Sie ist per Vorgabe auch Teil der Willkommensnachricht (Abonnementbestätigung). Dies ist nicht dasselbe wie die Selbstdarstellung der Liste in der WWW-Listenoberfläche;
    -   **Listen-Homepage**: Diese Beschreibung wird auf der Informationsseite der Liste angezeigt. Sie kann im HTML-Format gehalten sein. Auch wenn Sie dieses Format nicht verwenden, benutzen Sie bitte `<br />`-Tags, um Zeilen umzubrechen;
    -   **Nachrichtenkopf**: wird, sofern vorhanden, als MIME-Attachment an den Anfang jeder über die Liste verschickten Nachricht gestellt;
    -   **Nachrichtenfuß:** wird, sofern vorhanden, als MIME-Attachment an das Ende jeder über die Liste verschickten Nachricht gestellt.

Sympa benutzt normalerweise vorgegebene Dateien; in diesem Falle sind die listenspezifischen Dateien für Ihre Liste leer. **Um eine Datei zu bearbeiten, wählen Sie sie aus der Auswahlliste und klicken Sie auf den 'Bearbeiten'-Knopf.** Sie können jeweils die **'From'-Zeile** (Absender), die **'Subject'-Zeile** (Betreffzeile) und den **Nachrichtentext** (Rumpf, Body) ändern.

| Note |
|------|
| Seien Sie vorsichtig: Die Werte zwischen eckigen Klammern sind Variablen. Ändern Sie sie nicht, es sei denn, Sie wissen wirklich genau, was Sie tun... |

#### <span id="manage_shared"></span>Den Bereich für gemeinsame Dokumente verwalten

Per Vorgabe haben Listen keinen Bereich für gemeinsame Dokumente. Sie müssen diesen daher einrichten. Um dies zu tun, wählen Sie das **Listen-Administrationsmodul** und klicken Sie auf den Link **'Gemeinsame Dokumente erstellen'.**

Damit Abonnenten Dokumente im Bereich für gemeinsame Dokumente veröffentlichen können, müssen Sie die **vorgegebenen Berechtigungen ändern:** Klicklen Sie im Listen-Administrationsmodul auf **'Listenkonfiguration bearbeiten'** und dann auf **'Privilegien'.** Am Fuß der Seite ist ein Auswahlmenü namens [**'Wer kann bearbeiten';**](listconfig#docsrights.md) wählen Sie die Option **'Beschränkt auf Abonnenten (privat)'.**

| Note |
|------|
| Seien Sie vorsichtig: Wenn Sie bereits vor dieser Rechteänderung Ordner angelegt haben, bleiben diese weiterhin schreibgeschützt. Wenn Sie sie beschreibbar machen wollen, müssen Sie die [Zugriffsrechte](shared#acces.md) für diesen Ordner ändern. |

Eventuell möchten Sie auch [**Quatos**](listconfig#docsrights.md) für den Bereich für gemeinsame Dokumente einrichten; tun Sie dies auf der Seite 'Privilegien' des Abschnitts 'Listenkonfiguration bearbeiten'.

Um **alles über die Verwaltung gemeinsamer Dokumente zu erfahren** (Organisation, Zugriffsrechte ändern, Dokumente benennen etc.), betrachten Sie den Abschnitt ['Den Bereich für gemeinsame Dokumente verwenden'](shared.md) im Benutzerhandbuch.

Um **den Zugriff zum Bereich für gemeinsame Dokumente zu sperren,** klicken Sie auf **'Gemeinsame Dokumente löschen'** im Untermenü 'Admin'. Sie können den Bereich jederzeit **wieder öffnen,** indem Sie auf **'Gemeinsame Dokumente wiederherstellen'** klicken. Löschen und Wiederherstellen des Bereichs für gemeinsame Dokumente hat **keinerlei Effekt auf die enthaltenen Dokumente.**

#### <span id="manage_members"></span>Abonnenten verwalten

In diesem Abschnitt können Sie die **Liste aller Listenabonnenten** einsehen. Für jeden Abonnenten sind die folgenden Informationen verfügbar:

-   **E-Mail-Adresse;**
-   **Domain** der E-Mail-Adresse (*@cru.fr*, *@sympa.org*, *@uni-marburg.de*, etc.);
-   **Bild** (falls diese Funktion für die Liste aktiviert wurde);
-   **Name** (abhängig von der Abonnementmethode wird dieser nicht immer angezeigt);
-   [**Empfangsmodus;**](#deliverymode)
-   **Datenquelle;** dies gibt die Herkunft des Eintrags an, falls der Abonnent in die Liste eingebunden wurde und sie nicht direkt abonniert hat;
-   **Datum des Abonnements** der Liste;
-   **letzte Änderung** der Abonnementoptionen.

| Note |
|------|
| Per Vorgabe zeigt jede Seite 25 Abonnenten an. Sie können die Seiten mit den Blätterpfeilen durchblättern oder mehr Abonnenten pro Seite darstellen. Sie können die Abonnenten auch nach verschiedenen Kriterien sortieren, indem Sie auf den entsprechenden Spaltenkopf klicken. |

Um **einen Abonnenten zu suchen,** geben Sie seinen Namen oder seine E-Mail-Adresse ganz oder teilweise in das Eingabefeld ein und klicken Sie auf den Knopf **'Suchen'.**

Sie können auf dieser Seite **andere Personen in die Liste eintragen:**

-   Um eine **Einzelperson** einzutragen, geben Sie Ihre E-Mail-Adresse in das Eingabefeld ein und klicken Sie auf den Knopf **'Hinzufügen'.**
-   Um **mehrere Personen einzutragen,** klicken Sie auf den Knopf **'Mehrfaches Hinzufügen'.** Geben Sie in dem dann angezeigten Eingabefeld die E-Mail-Adressen und Namen der Personen, die Sie in die Liste eintragen möchten, ein, und klicken Sie auf **'Abonnenten hinzufügen'.**

| Note |
|------|
| Falls Sie Personen eintragen möchten, ohne dass sie darüber benachrichtigt werden, kreuzen Sie das Feld 'leise' an. Es ist allerdings wesentlich besser, wenn Betroffene erfahren, dass sie abonniert werden! |

Auch wenn es möglich ist, Personen zu Ihren Mailinglisten hinzuzufügen, ist es **stets viel besser, wenn Personen selbst die entsprechenden Schritte ausfzühren, um eine Liste zu abonnieren.** Sie können daher mit dem INVITE-Befehl auch **Personen einladen, eine Liste zu abonnieren:** Senden Sie eine E-Mail an {{conf.email}}@{{conf.host}} und geben Sie den folgenden Befehl in den Nachrichtentext ein: **invite listenname mailadresse** (Beispiel: *invite beispielliste max.mustermann(@)uni-marburg.de*).

Um **Abonnementanfragen für die Liste anzunehmen oder abzulehnen,** klicken Sie auf **'Unbestätigte Abonnements.'** Die Liste aller Personen, die ein Abonnement beantragt haben, erscheint. Um eine Anfrage anzunehmen oder abzulehnen, kreuzen Sie das Feld vor dem Namen der Person an und klicken Sie auf den Knopf Ihrer Wahl.

Um **eine Abonnementerinnerung an alle Abonnenten zu schicken,** klicken Sie auf den Knopf **'Alle erinnern'.** Die Abonnement-Erinnerungsnachricht enthält:

-   den **Namen der Liste,** die der Abonnent abonniert hat;
-   die **E-Mail-Adresse,** unter der der Abonnent abonniert ist;
-   das **Listenpasswort** des Abonnenten;
-   einen **Link zur Informationsseite** der Liste;
-   eine **klickbare Adresse, unter der Abonnenten die Liste abbestellen können.**

| Note |
|------|
| Sie können auf der Seite ['Verschiedenes'](listconfig#other.md) des Abschnitts 'Listenkonfiguration bearbeiten' auch eine automatische Abonnementerinnerung einrichten. |

Um auf dieser Seite **Abonnenten auszutragen,** wählen Sie sie, indem Sie die Felder vor ihren Namen ankreuzen, und klicken Sie auf den Knopf **'Ausgewählte E-Mail-Adressen löschen'.**

| Note |
|------|
| Falls Sie die Abonnenten darüber nicht informieren wollen, kreuzen Sie das Feld 'leise' an. Dies ist allerdings nicht empfehlenswert, es sei denn, es handle sich um Abonnenten mit Zustellfehlern. |

| Note |
|------|
| Tipp: Um alle Abonnenten auf einmal auszuwählen, sorgen Sie dafür, dass alle auf der Seite angezeigt werden, und klicken Sie den Knopf 'Auswahl invertieren': Alle Abonnenten werden mit einem einzigen Klick angewählt! |

Um **die Abonnementoptionen eines Abonnenten zu ändern,** klicken Sie auf seine E-Mail-Adresse.

Auf dieser Seite können Sie **den Namen, die E-Mail-Adresse und den Nachrichten-Empfangsmodus des Abonnenten ändern.** Sie können ihn auch **aus der Liste austragen.**

Falls der Abonnent [Zustellfehler verursacht,](#manage_bounces) wird unter dem Abschnitt 'Abonnenten-Information' ein weiteres Formular angezeigt:

Die angezeigten Informationen umfassen:

-   die Art des Fehlers (auf Englisch);
-   die Zahl der Fehler;
-   den Zeitraum, in dem die Fehler aufgetreten sind

Sie können **den jüngsten Fehler überprüfen** oder **die Fehler zurücksetzen.** Wenn Sie die Fehler zurücksetzen, wird die [Zustellfehler-Punktzahl](listconfig#bouncers.md) des Abonnenten auf null zurückgesetzt.

Um Adressen mit Zustellfehlern leichter zu verwalten, wählen Sie die Seite ['Zustellfehler'](#manage_bounces) im Listen-Administrationsmodul aus.

#### <span id="manage_bounces"></span>Zustellfehler verwalten

Wenn ein **Problem mit den E-Mail-Adressen der Abonnenten auftritt** (veraltete Mailadressen, zum Versandzeitpunkt zeitweise nicht verfügbare Adressen, überschrittene Postfachkapazitäten etc.), wird der Prozentsatz der Adressen mit Zustellfehlern im linken Menü unter dem Titel **'Fehlerrate'** angezeigt. Um die Adressen mit Fehlern zu überprüfen, wählen Sie die Seite **'Zustellfehler'** im Listen-Administrationsmodul aus,

Die Software Sympa verwaltet Abonnenten mit Zustellfehlern automatisch: Je nach der Fehlerzahl und der Auslastung der Liste werden Abonnenten mit Zustellfehlern entweder benachrichtigt, ausgetragen, oder ihre Punktzahl wird auf null zurückgesetzt, wenn die Adresse keine Zustellfehler mehr erzeugt.

Um **Zustellfehler an Adressen zu beenden,** wählen Sie sie aus, indem Sie ihre Felder anklicken, und klicken Sie den Knopf **'Fehler für gewählte Benutzer zurücksetzen'.** Falls der Fehler verbleibt, werden die Adressen wieder als mit Zustellfehlern behaftet markiert, sobald eine Nachricht über die Liste versandt wird.

Sie können auch **Abonnenten austragen, deren Adressen Zustellfehler verursachen:** zu viele Adressen mit Zustellfehlern verursachen eine nicht zu unterschätzende Belastung auf dem Mailinglistenserver. Um Abonnenten auszutragen, wählen Sie sie an, indem Sie die Felder vor ihren Namen ankreuzen, und klicken Sie auf den Knopf **'Ausgewählte E-Mail-Adressen löschen'.**

| Note |
|------|
| Tipp: Um alle Abonnenten auf einmal auszuwählen, sorgen Sie dafür, dass alle auf der Seite angezeigt werden, und klicken Sie den Knopf 'Auswahl invertieren': Alle Abonnenten werden mit einem einzigen Klick angewählt! |

#### <span id="moderate"></span>An die Liste gesendete Nachrichten moderieren

Wenn eine Liste moderiert ist, **müssen alle Nachrichten von einem Moderator bestätigt werden, bevor sie an die Liste verteilt werden.** Wenn eine Nachricht an eine Liste geschickt wurde, werden die Abonnenten automatisch per Mail darüber benachrichtigt, dass ihre Nachricht moderiert wird. Auch die Moderatoren erhalten eine Benachrichtigung von Sympa, die die zu moderierende Nachricht enthält.

Es gibt zwei Arten, **Moderationsaufgaben auszuführen:** einmal **per Mail,** indem Sie die von Sympa empfangenen Nachrichten beantworten, oder **über die WWW-Mailinglistenoberfläche.** Klicken Sie hierfür auf den Link **'Nachricht'** im Untermenü 'Moderieren': Eine Seite mit allen zu moderierenden Nachrichten erscheint (die neuesten Nachrichten stehen oben). **Klicken Sie, um eine Nachricht zu lesen, ihre Betreffzeile an.**

Sie haben **zwei Optionen**:

-   **dem Versand der Nachricht über die Liste zustimmen;**
-   **die Nachricht ablehnen und ihren Absender informieren:** Wenn Sie eine Nachricht ablehnen, ist es besser, den Absender darüber zu benachrichtigen.

Alle Moderatoren können entscheiden, ob eine Nachricht verteilt wird oder nicht. Allerdings ist die **Entscheidung des ersten Moderators, der die Nachricht bearbeitet, definitiv.** Sympa benachrichtigt Sie, wenn Sie versuchen, eine Nachricht zu bearbeiten, die bereits moderiert wurde. Falls es mehrere Moderatoren gibt, ist es **einfacher, Nachrichten über die WWW-Oberfläche der Mailingliste zu moderieren:** Sie können so alle verbleibenden unmoderierten Nachrichten auf einmal sehen.

| Note |
|------|
| **Ganz gleich, wann sie moderiert wurde, bleiben Versanddatum und -zeit einer Nachricht unverändert.** Falls der Versand extrem verzögerter Nachrichten erlaubt ist, kann man daher theoretisch am 31. Dezember eine auf den 1. Januar datierte Mail empfangen! |

Falls die Nachricht mit Benachrichtigung abgelehnt wurde, wird der Abonnent, der sie abgeschickt hat, per Mail benachrichtigt. Sie können [anpassen, welche Nachricht er erhält.](#customize)

Indem Sie das Feld **'Ohne Benachrichtigung ablehnen'** ankreuzen, können Sie verhindern, dass der Nachrichtenurheber benachrichtigt wird.

Indem Sie das Feld **'Zur schwarzen Liste hinzufügen'** ankreuzen, verzichten Sie nicht nur auf eine Ablehnungsbenachrichtignug, sondern fügen den Urheber der Nachricht auch zur schwarzen Liste der Liste hinzu. Sie können die schwarze Liste über den Knopf **'schwarze Liste bearbeiten'** am Fuß der Seite verwalten.

Wenn Sie die Ablehnungsbenachrichtigung, die der Nachrichtenurheber erhält, anpassen möchten, können Sie dies mit dem Knopf **'Ablehnungsnachrichten verwalten'** tun. Diese Verwaltungsseite lässt Sie eine Reihe von Ablehnungsnachrichten erstellen und definieren, welche per Vorgabe verwendet wird.

**Hinweis:** Sie können über das Listen-Administrationsmodul [Moderatoren hinzufügen oder entfernen.](listconfig#description.md) Klicken Sie dafür auf der Listen-Informationsseite auf **'Admin',** auf **'Listenkonfiguration bearbeiten',** und schließlich auf **'Listendefinition'.**

Sie können auch **Nachrichten bearbeiten, nachdem sie über die Liste verteilt wurden;** dies kann sinnvoll sein, wenn eine Liste nicht moderiert ist. Wenn Sie eine **Nachricht löschen** möchten, [suchen Sie sie im Online-Nachrichtenarchiv auf](arc#arcsearch.md) und klicken Sie auf den Knopf **'Diese E-Mail zum Löschen markieren'** in der oberen rechten Ecke der Nachricht. Eine Bestätigungsanfrage erscheint; klicken Sie auf 'OK'. Die Nachricht wird nach einigen Sekunden gelöscht. **Seien Sie vorsichtig: Diese Aktion ist unumkehrbar! Wenn Sie eine Nachricht löschen, kann sie nicht mehr zurückgeholt werden.**

#### <span id="manage_archives"></span>Das Nachrichtenarchiv verwalten

Die Mailinglisten-Verwaltungssoftware Sympa kann **herunterladbare, im .ZIP-Format komprimierte Archive der an die Liste geschickten Nachrichten** erzeugen. Um diese Archive herunterzuladen, **wählen Sie die Monate aus,** die Sie bei dieser Liste interessieren, und klicken Sie auf den Knopf **'ZIP-Datei herunterladen'.**

| Note |
|------|
| Tipp: Um in der Liste 'Archivauswahl' alle Monate zu wählen, in denen Nachrichten versandt wurden, klicken Sie auf den ersten Monat, halten Sie die Umschalttaste (Shift) gedrückt, und klicken Sie auf den letzten Monat in der Liste. |

Sie werden eine Datei des Namens **'listenname\_archive.zip'** erhalten, die **Ordner namens 'listenname\_jahr-monat'** (Beispiel: *beispielliste\_2005-06*) für jeden Monat enthält. In jedem Ordner **sind die Dateinamen laufende Nummern** für die Nachrichten in chronologischer Ordnung (Beispiel: die Datei '1' enthält die erste Nachricht des Monats). Die Nachrichtendateien haben **kein Suffix;** benutzen Sie den Texteditor Ihrer Wahl (Notepad, TextEdit, Vim etc.) um sie zu öffnen. **Jede Datei stellt eine vollständige Nachricht (mit allen Kopfzeilen) dar.**

Auf der Seite 'Archive verwalten' können Sie auch **Nachrichten löschen** (monatsweise, nicht nachrichtenweise). Um dies zu tun, **wählen Sie in der Liste die Monate aus,** die Sie interessieren, und klicken Sie auf den Knopf **'Ausgewählte Monate löschen'.**

| Note |
|------|
| **Seien Sie vorsichtig: Diese Aktion ist unumkehrbar! Wenn Sie auf 'Ausgewählte Monate löschen' klicken, denken Sie daran, dass Sie nicht nur eine Archivdatei, sondern das gesamte Nachrichtenarchiv des betreffenden Monats löschen!** |

#### <span id="renamelist"></span>Die Liste umbenennen

Klicken Sie im **Listen-Administrationsmodul** auf **'Liste umbenennen'.** Geben Sie den Namen Ihrer Wahl ein und klicken Sie auf den Knopf 'Diese Liste umbenennen'. Eine Bestätigungsanfrage erscheint; klickeN Sie auf 'OK'.

| Note |
|------|
| Falls Sie es sich anders überlegen, reicht es, umgekehrt vorzugehen und der Liste ihren alten Namen wieder zu geben. |

**Seien Sie vorsichtig: Wenn Sie eine Liste umbenennen, müssen dies die Listmasters wissen; andernfalls wird die Änderung keine Wirkung haben.**

Ein paar Tipps zur Benennung von Listen:

-   **Verwenden Sie keine Leerzeichen, Umlaute, Akzente oder Sonderzeichen** in Listennamen: diese Zeichen könnten Schwierigkeiten machen.
-   Wählen Sie einen **aussagekräftigen, aber kurzen Namen:** Denken Sie an die Abonnenten, die diesen Namen jedesmal, wenn sie eine Nachricht an die Liste schicken, werden tippen müssen!
-   Wenn Sie eine Reihe von Listen verwalten, können Sie **Ihren Listennamen ein gemeinsames Präfix geben;** Sie werden dann zusammen sortiert und sind leichter erkennbar (Bespiel: *xx-benutzer@{{conf.host}}, xx-support@{{conf.host}}* usw.).

#### <span id="supprlist"></span>Die Liste löschen

Klicken Sie im **Listen-Administrationsmodul** auf **'Liste löschen'.** Eine Bestätigungsanfrage erscheint; klicken Sie auf 'OK'.

| Note |
|------|
| **Seien Sie vorsichtig: Wenn Sie die Liste löschen, können Sie sie nicht selber wiederherstellen! Falls Sie sie wiederherstellen möchten, müssen Sie einen Listmaster darum bitten.** |

Was sind nun die faktischen **Konsequenzen** einer Listenlöschung?

-   Abonnenten werden sofort automatisch ausgetragen (einschließlich Eigentümer und Moderatoren).
-   **Das Nachrichtenarchiv bleibt erhalten,** aber niemand kann mehr darauf zugreifen.
-   **Die im Bereich für gemeinsame Dokumente veröffentlichten Dokumente bleiben erhalten,** aber niemand kann mehr auf sie zugreifen.
-   **Nur ein Listmaster hat die Macht, eine Liste wiederherzustellen;** wenn er das tut, werden die früheren Abonnenten automatisch wieder eingetragen.

| Note |
|------|
| Seien Sie vorsichtig: Wegen interner Verzögerungen bleiben die Listenseiten noch eine Weile unter den direkten Adressen erreichbar. Erst nach einiger Zeit werden sie verschwinden. |

**Wenn Sie möchten, dass die Liste und alle mit ihr verbundenen Dateien auf Dauer gelöscht werden,** müssen Sie einen Listmaster darum bitten.

### <span id="rulesadmin"></span>Empfohlene Methodik

Um vitale Listen zu haben, **müssen Sie sich an den Diskussionen darauf aktiv beteiligen:** Wenn eine Liste von ihren Eigentümern weder kontrolliert noch mit Leben erfüllt wird, kann das Niveau der Nachrichten sinken oder die Liste kann mit der Zeit einfach absterben.

**Die Verwendung von E-Mail im Allgemeinen und von Mailinglisten im Besonderen wird durch eine Reihe von Regeln, die für angenehme Kommunikation unerlässlich sind, bestimmt: die "Netiquette".** Als Listeneigentümer oder -moderator ist es Ihre Aufgabe, dafür zu sorgen, dass Abonnenten sich an sie halten. Sie können die allgemenien Prinzipien der Netiquette und viele weiterführende Links auf der [Wikipedia-Seite zum Thema Netiquette](http://de.wikipedia.org/wiki/Netiquette) finden.

<span id="charter"></span>Sie sollten eine **Charta für Ihre Liste schreiben,** die die für ihre Nutzung geltenden Regeln festschreibt:

erlaubte, tolerierte und verbotene Themen;

Stilregeln (beispielsweise Angabe der Sprachen, die Abonnenten in ihren Nachrichten verwenden dürfen, Verbot von

Note

Damit alle Abonnenten die Listencharta lesen, sollten Sie sie in die Willkommensnachricht aufnehmen, die sie nach dem Abonnieren erhalten. Um dies zu tun, müssen Sie diese Nachricht auf der Seite 'Vorlagen anpassen' des Listen-Administrationsmoduls [anpassen.](#customize)

Falls verfügbar, gibt eine Eigentümer- und Moderatorencharta Listeneigentümern und -moderatoren alle nötigen Informationen, um ihre Ämter auszuüben. Eine solche Charta beschreibt alle Rechte und Pflichten von Eigentümern und Moderatoren.

------------------------------------------------------------------------
