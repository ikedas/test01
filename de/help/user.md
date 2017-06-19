Mailinglisten - Benutzerhandbuch
--------------------------------

### <span id="howitworks"></span>Wie der Mailinglistendienst funktioniert

Der Mailinglistendienst wird durch die **Mailinglistensoftware Sympa** verwaltet. Zu dieser Software gehört eine **WWW-Oberfläche.**

**Um Aktionen auszuführen, die Mailinglisten betreffen** (abonnieren, Optionen ändern etc.), haben Sie zwei Möglichkeiten:

-   **sich bei der WWW-Oberfläche anmelden;**
-   **Befehle per Mail** an den Sympa-Mailinglistenmanager senden **({{conf.email}}@{{conf.host}}).**

**Um einen Befehl an Sympa zu senden,** gehen Sie folgendermaßen vor:

-   **Wenn Sie einen einzelnen Befehl senden,** geben Sie Ihn in die Betreffzeile Ihrer E-Mail ein und lassen Sie den Nachrichtentext leer.
-   **Wenn Sie mehrere Befehle senden,** lassen Sie die Betreffzeile Ihrer Mail leer und schreiben Sie alle Befehle in den Nachrichtentext. **Seien Sie vorsichtig:** sympa wird Ihre Nachricht nicht verarbeiten, solange Sie sich nicht an die folgenden Regeln halten:
    -   Jeden Befehl in eine neue Zeile schreiben.
    -   Ihre Mail in reinem Text, nicht in HTML schicken (also nicht formatieren).
    -   Ihre Nachricht darf nichts außer Sympa-Befehlen enthalten (keine Signatur).

Eine Beschreibung aller Befehle, die Sie an Sympa schicken können, ist unter [file:///help/mail\_commands](mail_commands.md) verfügbar.

### <span id="subscribe"></span>Mailinglisten abonnieren

Eine Mailingliste zu abonnieren ist sehr einfach:

1.  **Wählen Sie die Adresse,** unter der Sie die Liste abonnieren möchten.

    | Note |
    |------|
    | Sie sollten eine Adresse auswählen, deren Postfach Sie häufig überprüfen und die eine große Speicherkapazität für Ihre Mails bietet: Manche Listen verteilen viele Nachrichten, die manchmal große Anlagen enthalten. |

    | Note |
    |------|
    | Natürlich können Sie dieselbe Liste unter mehreren E-Mail-Adressen abonnieren. Sie müssen dann das ganze Prozedere mit jeder weiteren E-Mail-Adresse wiederholen. |

2.  Schicken Sie von der Adresse, unter der Sie die Liste abonnieren wollen, eine **Nachricht an {{conf.email}}@{{conf.host}}.**

    | Note |
    |------|
    | Sympa ist keine Person, sondern eine Listenverwaltungssoftware. Daher ist es nutzlos, eine liebenswürdige Anfrage zu schicken! ;-) |

3.  Geben Sie in der Betreffzeile Ihrer Nachricht ein: **subscribe listenname Vorname Name** (ersetzen Sie 'listenname' durch den Namen der Liste, die Sie abonnieren möchten, und geben Sie Ihren eigenen Namen und Vornamen an).
4.  **Lassen Sie den Nachrichtentext leer.**

    | Note |
    |------|
    | Um etwas Zeit zu sparen, können Sie auch mehrere Befehle in einer einzelnen Nachricht schicken. Um dies zu tun, folgen Sie den Anweisungen im Abschnitt [Wie der Mailinglistendienst funktioniert.](#howitworks) |

**Danach werden Sie eine Nachricht erhalten, die Ihnen mitteilt, ob Ihr Antrag angenommen wurde:** Falls Abonnements der Liste bestätigt werden müssen, kann der Listeneigentümer eventuell entscheiden, Sie nicht aufzunehmen. Falls dies geschieht, schicken Sie bitte nicht noch viele weitere Anträge: Dies ist nutzlos, das Ergebnis ändert sich nicht mehr. Sie können allerdings eine Nachricht direkt an den Listeneigentümer schicken (listenname-request@{{conf.host}}) um zu erklären, warum Sie unbedingt in die Liste aufgenommen werden sollten...

| Note |
|------|
| Hinweis: Sie werden gegebenenfalls aufgefordert, Ihre Abonnementanfrage zu bestätigen, bevor sie verarbeitet werden kann. Falls ja, halten Sie sich bitte an die Anweisungen in der Nachricht, die Sie erhalten werden. |

Je nach Art der Liste (Abonnementeinschränkungen oder nicht) und je nach den Arbeitszeiten des Listeneigentümers **werden Sie die Reaktion eventuell nicht sofort erhalten.** Es ist nutzlos, mehrere Anfragen zu schicken.

**Falls Ihr Antrag angenommen wird, bestätigt die Nachricht, die Sie erhalten, Ihr Abonnement der Liste. Diese Nachricht** (die Listencharta) **enthält diverse wichtige Informationen:**

-   Ihr **Listenpasswort.** Dieses Passwort ist für alle Listen, die Sie mit einer einzigen E-Mail-Adresse abonniert haben, dasselbe. Sie können es [online ändern,](#global_pref "Wie Sie Ihr Passwort ändern können") nachdem Sie sich bei der WWW-Oberfläche angemeldet haben;
-   **detaillierte Informationen über die Liste:** ihr Zweck, die WWW-Adresse, unter der das Nachrichtenarchiv verfügbar ist usw.
-   die **Regeln für die Liste und ihre Abonnenten:** erlaubte und unzulässige Themen, Netiquette, Rechtliches, Datenschutzregeln usw.

**Sie sollten Ihre Abonnementbestätigung nicht löschen:** Eventuell brauchen Sie sie später, um sich an Ihr Passwort zu erinnern oder um ein bestimmtes Kommando an Sympa zu schicken (z.B. zum Abbestellen). Allgemein **empfehlen wir, dass Sie alle Ihre Mailinglisten-Abonnementbestätigungen behalten.**

**Sie können eine Liste auch über die WWW-Mailinglisten-Oberfläche abonnieren.** Gehen Sie hierfür folgendermaßen vor:

1.  Öffnen Sie die **[Homepage](%7B%7Bpath_cgi%7D%7D/home)** der WWW-Oberfläche und **melden Sie sich an.**
2.  **Wählen Sie die Informationsseite der Liste,** die Sie abonnieren möchten.
3.  Klicken Sie im linken Menü **den Link 'Abonnieren'.**

### <span id="sympa_auth"></span>Anmelden bei der WWW-Oberfläche

Um sich bei der WWW-Oberfläche anzumelden, verwenden Sie das Anmeldeformular am oberen Rand der Seite. Wenn Sie angemeldet sind, werden dort Ihre E-Mail-Adresse und Ihr Benutzerprofil (Abonnent, Moderator oder Eigentümer) angezeigt.

Der Login-Prozess ist je nach Situation unterschiedlich:

-   **Wenn die Betreiberorganisation des Mailinglistendienstes eine Single-Sign-On-Technik verwendet** (diensteübergreifender Account und Legimierung, zum Beispiel über das CAS-System), sollten Sie sich mit Ihrem einheitlichen Account anmelden. Klicken Sie dazu auf den Knopf 'Los' neben dem Text **'Legitimierung über \[verwendeter Dienst\]'.** Geben Sie dann Ihren Benutzernamen und Ihr Passwort ein, um sich über den Legitimierungsserver anzumelden.

    | Note |
    |------|
    | Falls Sie sich über das Legitimierungssystem bereits bei einem anderen Dienst angemeldet haben, werden Sie automatisch angemeldet. Laden Sie gegebenenfalls die Seite neu. |

-   **Wenn der Single-Sign-On-Prozess Sie nicht abdeckt, dann können Sie Ihr Listenpasswort verwenden.** Melden Sie sich in diesem Fall auf klassische Weise an: Geben Sie die **E-Mail-Adresse, unter der Sie die Liste abonniert haben** als Login und Ihr **Listenpasswort** im 'Passwort'-Feld ein.

    | Note |
    |------|
    | Falls Sie sich nicht an Ihr Listenpasswort erinnern, klicken Sie auf 'Passwort vergessen?'. Sie müssen dann Ihre E-Mail-Adresse eingeben, und Sie werden eine Mail mit einer Bestätigungs-URL erhalten. |

-   **Falls Sie der Single-Sign-On-Prozess nicht abdeckt und Sie noch kein Listenpasswort haben,** klicken Sie auf **'Erste Anmeldung?'** und geben Sie Ihre E-Mail-Adresse ein. An diese Adresse wird eine Bestätigungs-URL geschickt. Dann können Sie Ihr Passwort wählen.

| Note |
|------|
| Beachten Sie: Das Listenpasswort ist ein besonderes Passwort, das Sie nur für den Mailinglistendienst brauchen. |

### Ihre Abonnements überprüfen

Um alle Listen zu sehen, die Sie abonniert haben, müssen Sie sich zunächst [anmelden.](#sympa_auth) Eine Liste all Ihrer Listen, inklusive einer Kurzbeschreibung für jede einzelne, wird im Formular 'Ihre Liste' in der linken Spalte angezeigt.

**Um die Informationsseite einer Liste zu sehen, klicken Sie auf ihren Namen.** Die Informationsseite enthält eine Beschreibung der Liste (Thema, Regel für neue Nachrichten etc.), deren Länge von der Liste abhängig ist.

Von dieser Informationsseite aus können Sie:

-   Ihre [Abonnementoptionen](#options) ändern;
-   das [Listenarchiv](arc.md) lesen;
-   [das Listenarchiv durchsuchen;](arc#arcsearch.md)
-   [neue Nachrichten senden;](sendmsg.md)
-   Dokumente aus dem Bereich für gemeinsame Dokumente [herunterladen;](shared#shared_read.md)
-   Dokumente in den Bereich für gemeinsame Dokumente [hochladen;](shared#shared_upload.md)
-   die Abonnenten der Liste [auflisten](#subscribers) (sofern verfügbar);
-   [Aussetzen oder Wiederaufnehmen](suspend.md) von Abonnements einzelner Listen
-   die Liste [abbestellen.](#unsubscribe)

<span id="subscribers"></span>Die **Anzahl der Abonnenten** der Liste wird im **linken Menü** ständig angezeigt. **Um die Listenabonnenten aufzulisten, klicken Sie auf den Link 'Abonnenten auflisten'** im linken Menü (falls der Listeneigentümer entschieden hat, die Abonnentenliste vertraulich zu halten, ist dieser Link nicht verfügbar). Die Abonnentenliste zeigt alle Abonnenten mit **E-Mail-Adresse** und **Name** an (die Namensanzeige hängt davon ab, auf welche Weise sich die Abonnenten eingetragen haben).

| Note |
|------|
| Per Vorgabe zeigt jede Seite 25 Abonnenten an. Sie können mit den Blätterpfeilen durch diese Seiten blättern oder einstellen, dass mehr Abonnenten pro Seite angezeigt werden. Sie können die Abonnenten außerdem nach E-Mail-Adresse, Domain oder Name sortieren, indem Sie auf den entsprechenden Spaltenkopf klicken. |

**Die Namen der Listeneigentümer und -moderatoren werden im linken Menü angezeigt.** Sie sollten nie direkt an einen Listeneigentümer oder -moderator schreiben. Wenn Sie eine Frage oder einen Kommentar an sie richten wollen, sollten Sie die folgende Adresse verwenden: **listenname-request@{{conf.host}}** (ersetzen Sie 'listenname' durch den Namen der entsprechenden Liste).

Um zu wissen, **wann Sie die Liste abonniert haben** und **wann Sie Ihre Abonnementoptionen zum letzten Mal geändert haben, klicken Sie auf den Link 'Abonnementoptionen'** im linken Menü.

### <span id="pref"></span>Ihre Einstellungen verwalten

Um **einfacher mit Listen zu arbeiten, können Sie eine Anzahl persönlicher Einstellungen treffen.** Es gibt zwei Arten von Einstellungen, die Sie ändern können:

-   Ihre **Abonnementoptionen,** die je nach Liste unterschiedlich sein können;
-   Ihre **allgemeinen Einstellungen,** die das gesamte Sympa-Mailinglistensystem betreffen.

#### <span id="options"></span>Ihre Abonnementoptionen ändern

**Ihre Abonnementoptionen können von Liste zu Liste unterschiedlich sein.** Um sie zu ändern, gehen Sie folgendermaßen vor:

1.  Öffnen Sie die **[Homepage](%7B%7Bpath_cgi%7D%7D/home)** der WWW-Oberfläche und **melden Sie sich an.**
2.  **Wählen Sie die Informationsseite der Liste,** für die Sie Ihre Abonnementoptionen ändern wollen.
3.  Klicken Sie im linken Menü auf **'Abonnementoptionen'.**
4.  <span id="deliverymode"></span>**Wählen Sie einen Nachrichten-Versandmodus** (diese Optionen schließen sich gegenseitig aus, daher können Sie nur eine einzelne davon wählen):
    -   **MIME-Kompilat:** Statt wie normalerweise als einzelne Mails, werden Ihnen die Listennachrichten regelmäßig als Zusammenstellung zugestellt. Dieses Kompilat stellt eine Reihe von Nachrichten der Liste im MIME-Format multipart/digest zu. Der Turnus der Kompilate wird vom Listeneigentümer bestimmt.
    -   **Reintext-Kompilat:** Statt wie normalerweise als einzelne Mails, werden Ihnen die Listennachrichten regelmäßig als Zusammenstellung zugestellt. Dieses Kompilat stellt eine Reihe von Nachrichten der Liste im einfachen Textformat zusammen. Der Turnus der Kompilate wird vom Listeneigentümer bestimmt.
    -   **Zusammenfassungs-Modus:** Statt die Listennachrichten auf normale Weise zu erhalten, wird Ihnen regelmäßig eine Liste davon zugeschickt. Um die Nachrichten zu lesen, müssen Sie das Online-Listenarchiv aufsuchen.
    -   **Benachrichtigungsmodus:** In diesem Modus erhalten Sie alle Nachrichten mit leerem Narichtentext; so werden Sie über jede Nachricht, die an die Liste geschickt wird, in Echtzeit informiert, aber Sie riskieren nicht, dass Ihr Eingangspostfach überschwemmt wird.
    -   **keine Mail (nützlich für Urlaube):** Dieser Modus ermöglicht es, gar keine Nachrichten von der Liste zu erhalten. Er ist besonders nützlich, wenn Sie längere Zeit keinen Zugriff auf Ihre E-Mail haben und die Liste trotzdem weiter abonnieren möchten.
    -   **Nur-Text-Modus:** In diesem Modus erhalten Sie nur die Textversion (text/plain) von Nachrichten, die in beiden Formaten (Reintext und HTML) verschickt werden.
    -   **Nur-HTML-Modus** In diesem Modus erhalten Sie nur die HTML-Version (text/html) von Nachrichten, die in beiden Formaten verschickt werden.
    -   **URL-Modus:** In diesem Modus erhalten Sie keine Dateianlagen (Attachments). Diese Dokumente bleiben aber im Listenarchiv verfügbar und Sie können auf Sie über einen URL in der Nachricht zugreifen.
    -   **Sie empfangen Ihre eigenen Nachrichten nicht:** In diesem Modus wird Ihnen keine Kopie der von Ihnen selbst verschickten Nachrichten zugesandt.
    -   **Standard (direkter Empfang):** Dieser Modus ist die Vorgabe; er setzt alle anderen Auslieferungsmodi außer Kraft.
    -   **stillgelegt**: Dieser Modus erlaubt es Ihnen, das Abonnement einer oder mehrer Listen für eine bestimmte oder unbestimmte Zeit zu deaktivieren. Anders als bei der Abbestellung können Sie Ihr Abonnement beibehalten und im Abschnitt "Abonnements verwalten" jederzeit wieder aktivieren.
5.  **Eine Sichtbarkeitsoption auswählen:**
    -   **gelistet in der Listenübersicht:** Ihr Name und Ihre E-Mail-Adresse werden in der Abonnentenliste angezeigt (sofern der Listeneigentümer Abonnenten erlaubt hat, die Abonnenten aufzulisten).
    -   **verborgen:** Ihr Name und Ihre E-Mail-Adresse werden nicht in der Abonnentenliste angezeigt. Trotzdem wird Ihre E-Mail-Adresse in den Listenarchiven sichtbar, wenn Sie Nachrichten verschicken.
6.  **Klicken Sie auf den Knopf 'Aktualisieren'.**

#### <span id="global_pref"></span>Ihre allgemeinen Einstellungen ändern

Die allgemeinen Einstellungen betreffen alle Ihre Abonnements und die Darstellungsweise der Sympa-WWW-Mailinglistenoberfläche. Um Ihre Einstellungen zu ändern, gehen Sie folgendermaßen vor:

1.  Öffnen Sie die **[Homepage](%7B%7Bpath_cgi%7D%7D/home)** der WWW-Oberfläche und **melden Sie sich an.**
2.  **Klicken Sie auf 'Ihre Einstellungen'** in der Leiste am oberen Rand.
3.  **Ihre Einstellungen ändern.**
4.  **Klicken Sie bei jeder Option, die Sie geändert haben, auf den Absendeknopf.**

Sie können Folgendes ändern:

-   Ihren **Namen;** wenn Sie eine Liste über die WWW-Oberfläche des Mailinglistenservers abonnieren, wird Ihr Namensfeld in der Abonnentenliste automatisch ausgefüllt;
-   die **Sprache, in der die Sympa-WWW-Oberfläche angezeigt wird** (Sie können die Sprache auf jeder Seite der WWW-Oberfläche ändern; Ihre Auswahl wird dieselbe bleiben, auch wenn Sie auf einer anderen Seite als 'Einstellungen' die Dialogsprache ändern;
-   die **Lebensdauer des von Sympa auf Ihrem Computer abgelegten Cookies** ('Ablauf der Verbindungszeit'). Per Vorgabe endet Ihre Sitzung, wenn Sie Ihren Browser schließen; falls Sie den Mailinglistendienst viel benutzen, sollten Sie eine längere Dauer wählen;

    | Note |
    |------|
    | Ein Cookie ist eine kleine Datei, die ein Webserver - meistens zeitweise - auf Ihrer Festplatte speichert, um Sie als Benutzer seines Dienstes wiederzuerkennen. Es enthält einige persönliche Informationen über Sie: Name, E-Mail-Adresse, Zeit des letzten Logins etc. |

-   die **E-Mail-Adresse, unter der Sie für Listen registriert sind** (falls Sie mehrere E-Mail-Adressen registriert haben, wird diejenige zum Ersetzen angezeigt, mit der Sie sich angemeldet haben);

    | Note |
    |------|
    | Seien Sie vorsichtig: Dies wird all Ihre Listenabonnements ändern. Wenn Sie die Adresse nur für eine einzelne Mailingliste ändern möchten, sollten Sie sich eher von dieser Liste ab- und sich mit der neuen E-Mail-Adresse wieder anmelden. |

-   Ihr **Listenpasswort.**

Der Abschnitt **'Ihre anderen E-Mail-Adressen'** erledigt ebenfalls E-Mail-Adressänderungen.

### Nach einer Mailingliste suchen

Sie möchten vielleicht nach einer Mailingliste suchen. Hierfür haben Sie drei Möglichkeiten:

**die verschiedenen Kategorien,** die auf der Homepage der Listen-WWW-Oberfläche angezeigt werden, durchblättern;

mit dem **Suchfeld** nach einer Liste suchen: Die Suche nach einer Zeichenketten gibt alle Listen zurück, deren Name oder Beschreibung Ihren Suchkriterien entspricht (Listenbeschreibungen bestehen normalerweise aus einem kurzen Satz);

klicken Sie auf den Reiter [](file:///lists%3E'Listenübersicht'%3C/a%3E%20oben%20auf%20der%20Seite,%20um%20%3Cstrong%3Ealle%20verfügbaren%20Listen%20anzuzeigen.%3C/strong%3E%3C/li%3E%0A%20%20%20%20%20%20%20%20%3C/ul%3E%0A%20%20%20%20%20%20%20%20%3Cp%3E%3Ctable%20class=)

Note

Je nach der Domain, zu der Ihre E-Mail-Adresse gehört (Beispiel: *uni-marburg.de, cru.fr* etc.) und dem Ort, von dem Sie sich anmelden, ändert es sich eventuell, auf welche Listen Sie Zugriff haben. Sie können allerdings eine Liste abonnieren, die nicht angezeigt wird, wenn Sie ihren Namen kennen. Um dies zu tun, [verwenden Sie Ihr E-Mail-Programm.](#subscribe)

### <span id="archives"></span>Ein Listenarchiv online lesen

Bitte betrachten Sie hierzu die [**Archivdokumentation.**](arc.md)

### <span id="sendmsg"></span>Eine Nachricht senden

Bitte betrachten Sie hierzu die [**Dokumentation zum Senden von Nachrichten.**](sendmsg.md)

### <span id="shared"></span>Den Bereich für gemeinsame Dokumente nutzen

Bitte betrachten Sie hierzu die [**Dokumentation zum Bereich für gemeinsame Dokumente.**](shared.md)

### <span id="suspend"></span>Aussetzen oder Wiederaufnehmen von Abonnements einzelner Listen

Bitte betrachten Sie hierzu die [**Dokumentation zur Abonnementverwaltung**](suspend.md)

### <span id="unsubscribe"></span>Listen abbestellen

Um eine Liste abzubestellen, gehen Sie folgendermaßen vor:

1.  Senden Sie von der Adresse, unter der Sie die Liste abonniert haben, eine **Nachricht an {{conf.email}}@{{conf.host}}.**
2.  Schreiben Sie in die Betreffzeile Ihrer Mail: **unsubscribe listenname** (ersetzen Sie 'listenname' durch den Name der Liste, die Sie abbestellen wollen).
3.  **Lassen Sie den Nachrichtentext leer.**

    | Note |
    |------|
    | Um etwas Zeit zu sparen, können Sie auch mehrere Befehle in einer einzelnen Nachricht schicken. Um dies zu tun, folgen Sie den Anweisungen im Abschnitt [Wie der Mailinglistendienst funktioniert.](#howitworks) |

Sie können auch über die Mailinglisten-WWW-Oberfläche abbestellen (Sie müssen dies für jede Liste wiederholen, die Sie abbestellen wollen):

1.  Öffnen Sie die **[Homepage](%7B%7Bpath_cgi%7D%7D/home)** der WWW-Oberfläche und **melden Sie sich an.**
2.  **Gehen Sie zur Informationsseite der Liste,** die Sie abbestellen wollen.
3.  **Klicken Sie im linken Menü auf den Link 'Abbestellen'.**

------------------------------------------------------------------------
