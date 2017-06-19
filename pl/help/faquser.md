### Często zadawane pytania użytkowników

#### Nie możesz subskrybować listy

Przyczyny tego problemu mogą być następujące:

-   **Właściciele listy zapomnieli przetworzyć Twojej prośby o subskrypcję**: błądzić jest rzeczą ludzką, a Twoja prośba mogła zagubić się pomiędzy wieloma innymi wiadomościami! Zanim [skontaktujesz się bezpośrednio z właścicielami](#contactadmin), wyślij jeszcze raz prośbę o subskrypcję.
-   **Subskrypcja ograniczona jest do konkretnej grupy ludzi**. Aby dowiedzieć się więcej, [skontaktuj się z właścicielami listy](#contactadmin).

#### Nie możesz zalogować się do interfejsu webowego list mailingowych

Przyczyny tego problemu mogą być następujące:

-   ~~**You have no password**. To be given a password, follow the [First login?](%7B%7Bpath_cgi%7D%7D/firstpasswd) link from the homepage. You will receive your new password by email.~~
-   **Wpisujesz nieprawidłowe hasło**. Jeśli nie pamiętasz swojego hasła, możesz je zresetować. Aby to zrobić, użyj linku [Zapomniałeś hasło?](%7B%7Bpath_cgi%7D%7D/renewpasswd), który znajdziesz na stronie domowej.
-   **Używasz nieprawidłowego loginu** (adresu email, którym subskrybujesz listę).

| Note |
|------|
| Aby uniknąć błędów przy wprowadzaniu hasła, możesz wpisać jest do innej aplikacji (na przykład klienta poczty elektronicznej), a następnie skopiować i wkleić je do przeglądarki. |

#### Nie otrzymujesz (części) wiadomości wysyłanych na listę

Problem może mieć następujące przyczyny:

-   <span id="notsubscribedyet"></span>**Nigdy nie subskrybowałeś listy**:
    -   Być może błędnie wpisałeś swój adres email, gdy próbowałeś zasubskrybować listę.
    -   Być może subskrybujesz listę innym adresem niż ten, z którego wiadomości sprawdzasz.
    -   Być może Twoja prośba o subskrypcję została odrzucona przez właścicieli listy.

    W każdym razie, spróbuj [zasubskrybować listę](user.md#subscribe) ponownie.
-   <span id="notsubscribedanymore"></span>**Już nie jesteś uczestnikiem listy**:
    -   Jeśli Twój adres przez jakiś czas zwracał wiadomości, być może zostałeś wypisany z listy przez system (lub przez właścicieli). Spróbuj [zapisać się ponownie](user.md#subscribe) po upewnieniu się, że adres email działa prawidłowo.
    -   Jeśli nie stosowałeś się do reguł panujących na liści, być może właściciele listy zablokowali Ci dostęp...
    -   Być może zostałeś wypisany z listy przez inną osobę, jest to możliwe w sytuacji, gdy lista nie wysyła wiadomości potwierdzających prośby o zapisanie lub wypisanie się z listy... W takiej sytuacji, spróbuj [zapisać się](user.md#subscribe) ponownie.
-   **Twój [tryb dostarczania](user.md#deliverymode) nie pozwala na otrzymywanie wiadomości**: na przykład gdy masz ustawiony tryb 'Brak wiadomości'.
-   **Twoja skrzynka pocztowa jest przepełniona**. Uwaga: jeśli Twoja skrzynka nie jest całkowicie przepełniona, dostajesz jedynie niewielkie wiadomości, i trudno jest zrozumieć, co stanowi problem... Jeśli Twój adres email regularnie powoduje problemy, możesz być wypisany z listy przez właścicieli listy lub system. Dlatego powinieneś często czyścić swoją skrzynkę.
-   **Twoja skrzynka pocztowa ma jakieś ograniczenia**: nie pozwala odbierać wiadomości z załącznikami, wycina załączniki konkretnego typu lub ogranicza maksymalny rozmiar przychodzących wiadomości. W takie sytuacji, radzimy skorzystać z [trybu url](user.md#deliverymode).

#### Nie możesz wysyłać wiadomości na listę

Problem może mieć następujące przyczyny:

-   **[Nigdy nie byłeś uczestnikiem](#notsubscribedyet)** listy.
-   **[Już nie jesteś uczestnikiem listy](#notsubscribedanymore)**.
-   **Używasz innego adresu** niż ten, którym subskrybujesz listę.
-   **Jeśli lista jest moderowana, dystrybucja wiadomości zależy od dostępności moderatorów**: nie są w stanie monitorować listy całą dobę! Dlatego dystrybucja wiadomości może być nieco opóźniona.
-   **Jeśli lista jest moderowana, być może Twoja wiadomość została odrzucona przez moderatora**. Jeśli nie otrzymałeś żadnej informacji, możesz wysłać wiadomość na adres nazwalisty-request@{{conf.host}} i poprosić o wyjaśnienie.
-   **Wiadomość, którą próbujesz wysłać, nie spełnia pewnych warunków i nie może być rozesłana** na liście: być może jest za duża, zawiera zabroniony rodzaj załącznika albo po prostu zawiera załącznik (jeśli załączniki są zabronione na tej liście).
-   **Problem może być także związany z Twoim kontem email**:
    -   Serwer poczty jest czasowo niedostępny.
    -   Twoja skrzynka jest pełna i nie pozwala wysyłać nowych wiadomości.
    -   Twoja skrzynka ma jakieś ograniczenia: nie pozwala na wysyłanie wiadomości z załącznikami, blokuje pewne typy załączników albo ogranicza maksymalny rozmiar wysyłanych wiadomości.
-   **Być może popełniłeś błąd w adresie listy** przy próbie wysyłania wiadomości!

#### Nie możesz wypisać się z listy

Problem może mieć następujące przyczyny:

-   **Używasz innego adresu** niż ten, którym subskrybujesz listę.
-   **Zostałeś zapisany na listę za pośrednictwem dynamicznego źródła danych** (na przykład: bazy danych, katalogu LDAP, itp.). [Skontaktuj się z właścicielami](#contactadmin), aby dowiedzieć się więcej.
-   **Właściciele listy zapomnieli przetworzyć Twoją prośbę o wypisanie z listy**: błądzić jest rzeczą ludzką, a Twoja prośba mogła zagubić się pomiędzy innymi wiadomościami! Zanim [skontaktujesz się bezpośrednio z właścicielami](#contactadmin), spróbuj wysłać prośbę jeszcze raz.

#### <span id="contactadmin"></span>Chcesz skontaktować się z właścicielami listy

Nazwy właścicieli i moderatorów listy są wymienione w lewym menu. Jednak nie powinieneś nigdy pisać bezpośrednio do właściciela lub moderatora: po pierwsze, osoba do której piszesz może być nieobecna, poza tym, lepiej poinformować wszystkich właścicieli i moderatorów o swojej prośbie. Jeśli masz pytania lub uwagi, **powinieneś użyć adresu nazwalisty-request@{{conf.host}}** (zamień 'nazwalisty' na nazwę listy).
