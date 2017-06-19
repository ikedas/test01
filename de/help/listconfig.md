<span id="listconfig"></span>Die Liste konfigurieren:
-----------------------------------------------------

Da die Listenkonfiguration ziemlich komplex ist, ist sie in mehrere Teile auf jeweils einer eigenen Seite aufgeteilt:

-   [Listendefinition;](#description)
-   [Senden/Empfangen;](#sending)
-   [Privilegien;](#command)
-   [Archive;](#archives)
-   [Zustellfehler;](#bounces)
-   [Verschiedenes.](#other)

Wir empfehlen, **Konfigurationsänderungen in möglichst kleinen Einzelschritten zu vollziehen:** auf diese Weise können Sie Änderungen leichter wieder zurücknehmen, wenn das Ergebnis Ihren Erwartungen nicht entspricht.

Das Listen-Administrationsmodul bietet **viele Optionen zur Konfiguration Ihrer Liste.** Allerdings entsprechen diese Optionen vielleicht nicht Ihren eigenen Bedürfnissen. Um dieses Problem zu beheben, können Sie **einen Listmaster bitten, neue Optionen einzurichten** (selbstverständlich nur innerhalb deren Möglichkeiten): Zugriffs- und/oder Rechtebeschränkungen für bestimmte Kategorien von Benutzern entsprechend des Login-Orts, der Domain ihrer E-Mail-Adresse, ihrer Benutzergruppen-Zugehörigkeit etc.

### <span id="description"></span>Listendefinition

Im Feld **'Thema der Liste'** können Sie das Thema ändern, das Sie der Liste bei der Einrichtung gegeben haben. Dieses Thema wird als Kopfzeile für alle Listenseiten angezeigt und ist auch auf den Listen-Indexseiten (Listenübersicht, Abonnementübersicht etc.) und in der Titelleiste des Browsers zu sehen.

Sie können auch die **'Sichtbarkeit der Liste'** ändern. Folgende Optionen sind verfügbar:

-   verbergen außer für Abonnenten - *Vorgabe;*
-   Intranet-Zugang;
-   sichtbar;
-   unsichtbar - sogar für Abonnenten;

| Note |
|------|
| Wenn Sie die Sichtbarkeit der Liste nach anderen Kriterien beschränken möchten, sollten Sie einen Listmaster fragen: er kann eventuell eine neue Option, die Ihrem Bedarf entspricht, einrichten (Liste beispielsweise nur für Mitglieder einer Benutzergruppe oder Nutzer einer bestimmten Internet-Domain sichtbar etc.). |

In den Berichen 'Eigentümer' und 'Moderatoren' können Sie **Eigentümer und Moderatoren zur Liste hinzufügen** oder **deren persönliche Daten ändern:**

-   Für jeden Eigentümer/Moderator müssen Sie eine **E-Mail-Adresse** und einen **Namen** angeben.
-   Sie können auch die Informationen Ihrer Wahl ins Eingabefeld **'Private Informationen'** eintragen (Telefonnummer, Stellenbezeichnung etc.); diese Information ist nur für Listmasters und privilegierte Listeneigentümer zugänglich.
-   Sie können den **Nachrichten-Empfangsmodus** ändern (die einzigen auf dieser Seite verfügbaren Optionen sind 'mail' und 'nomail').
-   Der Parameter 'Profil' kann nicht geändert werden: das **'privilegierte' Profil** ist dem Listeneinrichter vorbehalten (andere Eigentümer haben ein 'normales' Profil).

| Note |
|------|
| Beachten Sie: Wenn Sie Eigentümer oder Moderator einer Liste werden, heißt dies nicht, dass Sie diese Liste automatisch abonnieren. Auch Eigentümer und Moderatoren müssen sich daher selbst als Abonnenten eintragen. |

Um **Eigentümer bzw. Moderatoren zu löschen,** löschen Sie den Inhalt der Eingabefelder zur Person, die Sie löschen möchten, und klicken Sie auf den Knopf 'Aktualisieren'.

Sie können auch die **Themen der Liste** und ihre **Sprache** verstellen. Wenn Sie die Listensprache verändern, werden alle vordefinierten Nachrichten in der gewählten Sprache verschickt (beachten Sie: dies gilt nur, soweit Übersetzungen vorliegen!).

Sie können die **Internet-Domäne** der Liste nicht ändern: nur ein Listmaster kann diesen Parameter bearbeiten.

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Aktualisieren' am Fuß der Seite zu klicken,** um all Ihre Änderungen zu speichern.

### <span id="sending"></span>Senden/Empfangen

Auf dieser Seite können Sie **entscheiden, wer Nachrichten über die Liste verschicken darf.**

Im Bereich **'Häufigkeit der Kompilierung'** können Sie definieren, wie häufig Nachrichtenkompilate verschickt werden (Empfangsmodi Kompilat und Zusammenfassung): Wählen Sie in der Liste alle **Tage** aus, an denen Kompilate verschickt werden sollen. Wählen Sie dann eine **Auslieferungszeit** für Kompilate (bitte vermeiden Sie es, eine Zeit zwischen 23 Uhr und Mitternacht zu wählen).

Wählen Sie in der Liste **'Verfügbare Abonnement-Optionen'** alle Abonnement-Optionen aus, die Sie Ihren Abonnenten anbieten wollen. Per Vorgabe sind alle Optionen ausgewählt.

Im Feld **'Antwortadresse'** können Sie auswählen, welche Empfänger per Vorgabe für Antworten an über die Liste geschickte Nachrichten angegeben sind:

-   Mit dem Wert **'Alle'** wird die Antwort sowohl an den **Nachrichtenabsender** als auch an die **Liste** geschickt.
-   Mit der Option **'Liste'** wird die Antwort an die **Liste** geschickt.

    | Note |
    |------|
    | Vorsicht: Verwenden Sie diese Option mit Bedacht! Die Erfahrung zeigt, dass Abonnenten nicht immer überprüfen, an welche Adresse sie ihre Antwort schicken. Daher kann es sein, dass sie private Nachrichten an die ganze Liste schicken, wenn sie versuchen, einer Einzelperson zu antworten. |

-   Mit der Option **'other\_email'** wird die Antwort an eine **Vordefinierte Adresse** geschickt. Falls Sie diese Option wählen, müssen Sie eine **E-Mail-Adresse im Feld 'andere E-Mail-Adresse' angeben.**
-   Mit dem Wert **'sender'** wird die Antwort an den **Nachrichtenabsender** geschickt. Diese Option sollten Sie wahrscheinlich auswählen.

Die Auswahlliste **'Berücksichtigung existierende Felder im Nachrichtenkopf'** erlaubt es Ihnen zu wählen, wie die SMTP-Kopfzeile 'Reply-To' in eingehenden Nachrichten verarbeitet wird. Die Option **'respect'** behält deren Wert bei, mit der Option **'forced'** wird sie überschrieben.

Zu guter Letzt lässt Sie die Option **'Titelmarkierung'** den **Text wählen, der in allen Nachrichten der Liste am Anfang der Betreffzeile eingefügt wird:** dies erlaubt Abonnenten, ihre Nachrichten einfach zu sortieren, sie automatisch mit Filtern zu verarbeiten usw. Per Vorgabe besteht dieser Text aus dem **Listennamen in eckigen Klammern** (die eckigen Klammern werden durch das System hinzugefügt, daher ist es sinnlos, wenn Sie sie selbst eintragen).

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Aktualisieren' am Fuß der Seite zu klicken,** um all Ihre Änderungen zu speichern.

### <span id="command"></span>Privilegien

Auf dieser Seite können Sie entscheiden:

-   **wer Listeninformationen sehen kann.** Folgende Optionen sind verfügbar:
    -   jeder (open) - *Vorgabe;*
    -   beschränkt auf Abonnenten (private).
-   **wer die Liste abonnieren kann.** Folgende Optionen sind verfügbar:
    -   Abonnement-Anfrage bestätigt (auth);
    -   benötigt Legitimierung (den Eigentümern wird eine Benachrichtigung geschickt) (auth\_notify);
    -   benötigt Legitimierung, dann Bestätigung durch einen Eigentümer (auth\_owner);
    -   Abonnieren nicht möglich (closed);
    -   lokale Abonnenten oder lokale Domäne (intranet);
    -   Benutzer der lokalen Domäne oder nach Bestätigung durch den Eigentümer (intranetorowner);
    -   jeder ohne Legitimierung (open) - *Vorgabe;*
    -   jeder mit Benachrichtigung an die Eigentümer (open\_notify);
    -   jeder, keine Begrüßungs-E-Mail (open\_quiet);
    -   Bestätigung durch Eigentümer (owner);
    -   muss mit S/MIME signiert sein (smime);
    -   muss mit S/MIME signiert sein oder nach Bestätigung durch einen Eigentümer (smimeorowner).

        | Note |
        |------|
        | Sie sollten immer eine Option, die 'auth' enthält, wählen: auf diese Weise muss der zukünftige Abonnent eine E-Mail-Bestätigung bearbeiten, bevor er in die Liste eingetragen wird. Dies verhindert Abonnements mit ungültigen E-Mail-Adressen und garantiert, dass niemand in eine Liste eingetragen wird, ohne es zu erfahren. |

-   **wer eine Liste abbestellen kann.** Folgende Optionen sind verfügbar:
    -   braucht Legitimierung (auth);
    -   Legitimierung notwendig, Bestätigung an den Eigentümer (auth\_notify);
    -   unmöglich (closed);
    -   offen (open) - *Vorgabeoption;*
    -   offen mit E-Mail-Bestätigung, der Eigentümer wird benachrichtigt (open\_notify);
    -   Bestätigung durch Eigentümer (owner).

        | Note |
        |------|
        | Sie sollten immer eine Option mit 'auth' wählen: auf diese Weise benötigt das System eine zusätzliche Bestätigung des Abonnenten, bevor dieser aus der Liste ausgetragen wird. Dies hindert Übelgesinnte daran, andere aus Listen auszutragen, ohne dass diese es erfahren. |

-   **wer Personen zum Abonnieren der Liste einladen kann.** Folgende Optionen sind verfügbar:
    -   geschlossen (closed);
    -   Einladung durch Listeneigentümer, keine Legitimierung (owner);
    -   beschränkt auf Abonnenten (privat) - *Vorgabe;*
    -   öffentlich (public).
-   **wer Abonnenten auflisten kann.** Folgende Optionen sind verfügbar:
    -   niemand darf die Benutzer auflisten (closed);
    -   beschränkt auf Abonnenten oder Benutzer der lokalen Domäne (intranet);
    -   nur Listmaster (listmaster);
    -   nur Eigentümer (und Listmaster) (owner) - *Vorgabe;*
    -   beschränkt auf Abonnenten (private);
    -   jeder! (public)

        | Note |
        |------|
        | Sie sollten die Abonnentenliste in keinem Fall uneingeschränkt zugänglich machen. Die Option 'beschränkt auf Abonnenten' mag sinnvoll sein, um Abonnenten die Möglichkeit zu geben, untereinander außerhalb der Liste zu kommunizieren. Dies ist jedoch im Falle eines Newsletters, dessen Abonnenten keine Beziehung zueinander haben, unangebracht. |

<span id="docsrights"></span>Auf dieser Seite können Sie auch **Zugriffsrechte für den Bereich für gemeinsame Dokumente bestimmten** (Abschnitt 'Gemeinsame Dokumente' der Liste, zu erreichen über einen Link im linken Menü). Sie können sowohl Lese- als auch Schreibrechte für Dokumente bestimmten:

-   Die folgenden Optionen sind in der Auswahlliste **'Wer kann ansehen'** verfügbar:
    -   beschränkt auf Abonnenten oder Benutzer der lokalen Domäne (intranet);
    -   beschränkt auf Listeneigentümer (owner);
    -   beschränkt auf Abonnenten (privat) - *Vorgabe;*
    -   öffentliche Dokumente (public).
-   Die folgenden Optionen sind in der Auswahlliste **'Wer kann bearbeiten'** verfügbar:
    -   beschränkt auf Listeneigentümer (owner) - *Vorgabe;*
    -   moderiert für Abonnenten (editor);
    -   beschränkt auf Abonnenten (private);
    -   öffentliche Dokumente (public).

Das Eingabefeld **'Quota'** lässt Sie eine **maximale Größe, die der Bereich für gemeinsame Dokumente nicht überschreiten darf,** festlegen. Diese Größe gibt nicht die Maximalgröße für *ein* Dokument im Bereich für gemeinsame Dokumente an, sondern die Maximalgröße für alle veröffentlichten Dokumente der Liste zusammen. Sie ist in Kilobyte angegeben. Wenn ein Abonnent versucht, eine Datei zu veröffentlichen, die größer als der restliche verfügbare Platz ist, erhält er eine Fehlermeldung.

Um mehr über **die Verwaltung des Bereichs für gemeinsame Dokumente** zu erfahren (Organisation, Änderung von Zugriffsrechten, Benennung von Dokumenten etc.), betrachten Sie bitte den Abschnitt ['Den Bereich für gemeinsame Dokumente benutzen'](shared.md) des Benutzerhandbuchs.

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Aktualisieren' am Fuß der Seite zu klicken,** um all Ihre Änderungen zu speichern.

### <span id="archives"></span>~~Archive~~

Auf dieser Seite können Sie **entscheiden, wer auf das Online-Listenarchiv zugrifen kann** (d.h. auf die über die WWW-Oberfläche der Mailingliste lesbaren nachrichten). Folgende Optionen sind verfügbar:

-   geschlossen (closed);
-   lokale Abonnenten oder lokale Domäne (intranet);
-   Listmaster (listmaster);
-   Eigentümer (owner);
-   Moderator (moderator);
-   nur Abonnenten (private);
-   öffentlich (public).

Das Eingabefeld **'Quota'** erlaubt Ihnen, eine **maximale Größe, die das Nachrichtenarchiv nicht überschreiten darf,** festzulegen. Listeneigentümer werden benachrichtigt, wenn die Archivgröße 95 % der erlaubten Größe erreicht. Wenn die Maximalgröße erreicht ist, werden keine eingehenden Nachrichten mehr archiviert.

| Note |
|------|
| Auch wenn die Archivierung von Nachrichten eingestellt wurde, ist es natürlich weiterhin möglich, Nachrichten an die Liste zu senden. |

Es ist auch möglich, **per E-Mail auf das Nachrichtenarchiv zuzugreifen.** Hierzu wird folgender Befehl an **{{conf.email}}@{{conf.host}}** geschickt: <span class="commande">**GET listenname jahr-monat**</span> (example: *GET beispielliste 2009-07*). Sie erhalten dann ein Kompilat aller im ausgewählten Monat versandten Nachrichten. Dieses Kompilat wird als reiner Text verschickt und enthält HTML-Tags statt der Originalformatierung; sie enthält auch die vollständigen Kopfzeilen jeder Nachricht. Der Parameter **'Textarchive'** erlaubt Ihnen zu definieren:

-   **wer das Recht hat,** das Nachrichtenarchiv der Liste per E-Mail abzufragen;
-   **in welchem Turnus diese Archivdateien erzeugt werden.** Wird der Turnus zum Beispiel auf 'month' eingestellt, werden jeweils die in einem Monat über die Liste verteilten Nachrichten in einer Archivdatei gebündelt.

Wenn dieser Parameter nicht definiert ist, wird die Liste kein per E-Mail zugängliches Archiv haben. Beachten Sie: **nur ein Listmaster hat das Recht, diesen Parameter zu verstellen.**

Es ist möglich, **mit S/MIME verschlüsselte Nachrichten** an die Liste zu schicken. Die Option **'Verschlüsselte E-Mails im Klartext archivieren'** lässt Sie bestimmen, wie diese Nachrichten archiviert werden:

-   Die Option **'decrypted'** archiviert die Nachricht nach Entfernen der Verschlüsselung.
-   Die Option **'original'** archiviert die Nachricht in ihrer ursprünglichen verschlüsselten Form.

Diese Option betrifft sowohl das Textarchiv als auch das Online-Archiv und die Kompilate, die Abonnenten geschickt werden, die einen Kompilat-Empfangsmodus ausgewählt haben.

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Update'** am Fuß der Seite zu klicken, um all Ihre Änderungen zu speichern.

### <span id="bounces"></span>Zustellfehler

**"Zustellfehler"** zeigt die **Abonnenten, deren Adressen Probleme verursachen,** d.h., Abonnenten, die die an die Liste geschickten Nachrichten nicht erhalten können. Dies kann viele Gründe haben: veraltete E-Mail-Adressen, beim Verschicken von Nachrichten zeitweilig nicht verfügbare Adressen, übervolle Eingangspostfächer etc.

Der Abschnitt **'Verwaltung der Zustellfehler'** definiert zwei Raten:

-   Die **Warnungsrate** gibt den Anteil von Adressen mit Zustellfehlern an, ab dem der Listeneigentümer eine **Benachrichtigung 'Zustellfehlerrate zu hoch'** erhält, die ihm nahe legt, Abonnenten mit Zustellfehlern aus der Liste zu löschen.
-   Die **Stopprate** gibt den Anteil von Adressen mit Zustellfehlern an, ab dem **die Verteilung von Nachrichten automatisch gestoppt wird,** bis das Problem gelöst ist (normalerweise durch Löschen von Abonnenten mit Zustellfehlern).

<span id="bouncers"></span>Die Abschnitte **'Benutzer mit Zustellfehlern verwalten, 1. Ebene'** und **'Benutzer mit Zustellfehlern verwalten, 2. Ebene'** erlauben Ihnen, automatisch erledigte Aufgaben hinsichtlich Benutzern mit Zustellfehlern auszuführen. Sie können Folgendes definieren:

-   die **Punktegrenzwerte, die Zustellfehlern die Ebene 1 und Ebene 2 anweisen.** Per Vorgabe haben Zustellfehler der Ebene 1 eine Punktzahl zwischen 45 und 74, der Ebene  2 zwischen 75 und 100;

    | Note |
    |------|
    | Die Punktzahl hängt von der Anzahl, der Art und der Häufigkeit von Fehlern ab. Wenn die Dauer des Problems zu kurz ist oder nur wenige Fehler aufgetreten sind, erhält die fehlerhafte Adresse keine Punktzahl. |

-   die **Aktion, die auf betroffene Abonnenten angewandt werden soll:** keine Aktion, Benachrichtigung, Entfernen aus der Liste;
-   die **zu benachrichtigende Person,** wenn eine Aktion ausgeführt wird: niemand, die Listeneigentümer, die Listmasters. Die Benachrichtigung, die verschickt wird, wenn eine Aktion ausgeführt wird, enthält die Namen aller betroffenen Abonennten und genaue Informationen über die Aktion.

**Um Zustellfehler zu verwalten,** (Fehlerstand für Abonnenten zurücksetzen, Abonnenten mit Zustellfehlern austragen, Abonnementerinnerungen verschicken usw.), **gehen Sie zur Seite ['Zustellfehler'](admin.md#manage_bounces)** des Listen-Administrationsmoduls.

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Update'** am Fuß der Seite zu klicken, um all Ihre Änderungen zu speichern.

### <span id="other"></span>Verschiedenes

Die Option **'Periodische Aufgabe zum Abonnement-Ablauf'** erlaubt Ihnen, eine **automatische Ablaufzeit für Abonnements** einer Liste festzulegen: in regelmäßigem Turnus (zum Beispiel jährlich) erhalten Abonnenten eine Nachricht, die sie bittet, ihr Listenabonnement zu erneuern. Falls sie dies nicht tun, werden sie ausgetragen. Dieses Prozedere stellt sicher, dass alle Abonnenten einer Liste wirklich interessiert und angesprochen sind.

Die Option **'Periodische Aufgabe zur Abonnenten-Erinnerung'** erlaubt ihnen, den Listenabonnenten in regelmäßigem Turnus **Abonnement-Erinnerungen zu schicken.**

Die Option **'Methode zum Schutz der E-Mail-Adresse'** stellt sicher, dass die E-Mail-Adressen der Abonnenten nicht durch automatische Adresssammler ("Harvester") eingesammelt werden, um ihnen später Spam zu schicken. Diese Option betrifft alle Seiten der WWW-Listenoberfläche.

Auf dieser Seite können Sie auch **Informationen zur letzten Änderung an der Liste** (wer etwas geändert hat und wann) sowie die **Anzahl von Konfigurationsänderungen** seit Einrichtung der Liste einsehen.

**VORSICHT: Vergessen Sie nicht, auf den Knopf 'Aktualisieren' am Fuß der Seite zu klicken,** um all Ihre Änderungen zu speichern.
