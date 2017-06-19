### Häufig gestellte Fragen für Benutzer

#### Sie können eine Liste nicht abonnieren

Dieses Problem kann auf folgende Gründe zurückgehen:

-   **Die Listeneigentümer haben vergessen, Ihre Abonnementanfrage zu bestätigen:** Irren ist menschlich, und vielleicht ist Ihr Antrag zwischen vielen anderen Nachrichten verloren gegangen! Stellen Sie eine neue Anfrage, bevor Sie [direkt Kontakt zu den Listeneigentümern aufnehmen.](#contactadmin)
-   **Die Liste darf nur von einer bestimmten Personengruppe abonniert werden.** Um mehr hierüber zu erfahren, [nehmen Sie Kontakt mit den Listeneigentümern auf.](#contactadmin)

#### Sie können sich nicht bei der WWW-Oberfläche der Mailingliste anmelden

Dieses Problem kann auf folgende Gründe zurückgehen:

-   **Sie haben kein Passwort.** Um ein Passwort zu erhalten, klicken Sie den Link [Erste Anmeldung?](%7B%7Bpath_cgi%7D%7D/firstpasswd) auf der Homepage. Sie werden per E-Mail Ihr neues Passwort erhalten.
-   **Sie haben ein ungültiges Passwort eingegeben.** Wenn Sie Ihr Passwort vergessen haben, können Sie es zurücksetzen. Klicken Sie hierfür den Link [Passwort vergessen?](%7B%7Bpath_cgi%7D%7D/renewpasswd) auf der Homepage an.
-   **Sie benutzen nicht den richtigen Benutzernamen** (die E-Mail-Adresse, unter der Sie die Liste abonniert haben).

| Note |
|------|
| Um Fehler zu vermeiden, wenn Sie Ihr Passwort eingeben, können Sie es in ein anderes Programm (zum Beispiel Ihre E-Mail-Software) eintippen, es kopieren und in Ihren Web-Browser einfügen. |

#### Sie erhalten (alle) Nachrichten, die auf die Liste gesendet werden, nicht

Dieses Problem kann mehrere Gründe haben:

-   <span id="notsubscribedyet"></span>**Sie haben die Liste nie abonniert**:
    -   Vielleicht haben Sie einen Fehler bei der Angabe Ihrer E-Mail-Adresse gemacht, als Sie versucht haben, die Liste zu abonnieren.
    -   Vielleicht haben Sie die Liste unter einer anderen E-Mail-Adresse abonniert als der, in deren Postfach Sie geschaut haben.
    -   Vielleicht wurde Ihre Abonnementanfrage von den Listeneigentümern zurückgewiesen.

    Versuchen Sie in jedem Fall, die Liste erneut zu [abonnieren.](user#subscribe.md)
-   <span id="notsubscribedanymore"></span>**Sie sind nicht mehr als Abonnent eingetragen**:
    -   Wenn Ihre Adresse eine Zeitlang Zustellfehler verursacht hat, sind Sie eventuell automatisch durch das System (oder sogar durch die Listeneigentümer) ausgetragen worden. Versuchen Sie, die Liste nochmals zu [abonnieren,](user#subscribe.md) nachdem Sie sich überzeugt haben, dass Ihre E-Mail-Adresse keine erneuten Schwierigkeiten verursachen wird.
    -   Falls Sie die verschiedenen auf der Mailingliste geltenden Regeln nicht beachtet haben, können Sie die Listeneigentümer eventuell gesperrt haben...
    -   Vielleicht sind Sie auch auf Veranlassung einer übel gesinnten Person ausgetragen worden, sofern die Liste nicht so konfiguriert ist, dass alle Abonnements und Abbestellungen bestätigt werden müssen... Versuchen Sie in diesem Fall, die Liste erneut zu [abonnieren.](user#subscribe.md)
-   **Ihr [Empfangsmodus](user#deliverymode.md) erlaubt Ihnen nicht, Nachrichten zu empfangen:** dies ist zum Beispiel beim Modus 'keine Mail' der Fall.
-   **Ihr Eingangspostfach ist voll.** Beachten Sie: Wenn Ihr Eingangspostfach nicht vollständig gefüllt ist, empfangen Sie nur kleine Nachrichten, was es erschwert, das eigentliche Problem zu erkennen... Falls Ihre E-Mail-Adresse außerdem regelmäßig Probleme macht, kann es sein, dass die Listeneigentümer oder das System Sie aus der Liste austragen. Sie sollten daher regelmäßig Platz in Ihrem Eingangspostfach machen.
-   **Ihr Eingangspostfach ist Beschränkungen unterworfen:** Es erlaubt Ihnen nicht, Nachrichten mit Anlagen (Attachments) zu empfangen, sperrt manche Typen von Anlagen oder begrenzt den Maximalumfang eingehender Nachrichten; in diesem Falle sollten Sie den [URL-Empfangsmodus](user#deliverymode.md) wählen.

#### Sie können keine Nachrichten an eine Liste senden

Dieses Problem kann mehrere Gründe haben:

-   **Sie waren [noch nie Abonnent](#notsubscribedyet)** der Liste.
-   **Sie sind [kein Abonnent mehr.](#notsubscribedanymore)**
-   **Sie benutzen eine andere Adresse** als die, unter der Sie die Liste abonniert haben.
-   **Wenn die Liste eine moderierte Liste ist, hängt der Versand der Nachricht vom Terminkalender der Moderatoren ab:** diese können die Liste nicht Tag und Nacht überwachen! Die Verteilung Ihrer Nachricht kann daher etwas auf sich warten lassen.
-   **Falls die Liste moderiert ist, ist Ihre Nachricht eventuell von einem Moderator abgelehnt worden.** Falls Sie darauf nicht hingewiesen worden sind, können Sie möglicherweise eine Nachricht an listenname-request@{{conf.host}} senden, um um eine Erklärung zu bitten.
-   **Die Nachricht, die Sie senden möchten, erfüllt die Bedingungen für den Versand über die Liste nicht:** Sie ist vielleicht zu groß, enthält einen verbotenen Typ von Anlage oder überhaupt irgendeine Anlage (sofern Attachments auf der Liste verboten sind).
-   **Das Problem mag auch von Ihrem E-Mail-Account herrühren:**
    -   Der Mailserver ist zeitweilig nicht verfügbar.
    -   Ihr Eingangspostfach ist voll und verhindert so, dass Sie neue Nachrichten senden können.
    -   Ihr Eingangspostfach ist gewissen Einschränkungen unterworfen: Es erlaubt Ihnen nicht, Nachrichten mit Anlagen zu versenden oder sperrt bestimmte Typen von Anlagen beziehungsweise es begrenzt die Größe ausgehender Nachrichten.
-   Zu guter Letzt **haben Sie vielleicht die Listenadresse falsch eingegeben,** als Sie Ihre Nachricht abgeschickt haben!

#### Sie können eine Liste nicht abbestellen

Dieses Problem kann mehrere Gründe haben:

-   **Sie benutzen eine andere Adresse** als die, unter der Sie die Liste abonniert haben.
-   **Sie sind über eine dynamische Datenquelle abonniert** (Beispiele: Datenbanken, LDAP-Verzeichnisse usw.), so dass Sie sich nicht austragen können. [Setzen Sie sich mit den Listeneigentümern in Verbindung,](#contactadmin) um mehr hierüber zu erfahren.
-   **Die Listeneigentümer haben vergessen, Ihre Abbestellungsanfrage zu bearbeiten:** Irren ist menschlich, und vielleicht ist Ihr Antrag zwischen vielen anderen Nachrichten verloren gegangen! Stellen Sie Ihre Anfrage erneut, bevor Sie [direkten Kontakt zu den Listeneigentümern aufnehmen.](#contactadmin)

#### <span id="contactadmin"></span>Sie möchten sich mit den Listeneigentümern in Verbindnug setzen

Die Namen der Listeneigentümer und -moderatoren sind im linken Menü erwähnt. Sie sollten allerdings nie direkt an einen Listeneigentümer oder -moderator schreiben: zum einen könnte die Person, an die Sie sich wenden, abwesend sein, zum anderen ist es besser, wenn alle Eigentümer und Moderatoren von Ihrem Anliegen erfahren. Wenn Sie eine Frage oder Anmerkung haben, **sollten Sie an folgende Adresse schreiben: listenname-request@{{conf.host}}** (ersetzen Sie 'listenname' durch den Namen der Liste).
