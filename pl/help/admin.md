<span id="docadmin"></span>Listy mailingowe - podręcznik właściciela i moderatora
---------------------------------------------------------------------------------

### Wprowadzenie: kto zarządza listami mailingowymi?

Przypomnienie: usługa list mailingowych definiuje cztery typy ról:

-   **administrator;**
-   **właściciel;**
-   **~~moderator;~~**
-   **subskrybent.**

Aby dowiedzieć się więcej o rolach, zapoznaj się z [opisami ról](introduction#roles.md).

### <span id="create_list"></span>Prośba o utworzenie listy mailingowej

**Prośba o utworzenie listy** może **podlegać pewnym warunkom**. Nawet po spełnieniu warunków **utworzenie listy** musi zostać **zatwierdzone przez administratora serwera**.

Aby poprosić o utworzenie listy mailingowej, wykonaj następujące kroki:

1.  Przejdź do **[strony domowej środowiska list](%7B%7Bpath_cgi%7D%7D/home)** i [**zaloguj się**](user#sympa_auth.md).
2.  W górnym menu **kliknij link 'Nowa lista'**.

    | Note |
    |------|
    | Jeśli nie widzisz tego linku, oznacza to że nie masz uprawnień do tworzenia list. |

3.  Nadaj swojej liście **nazwę** (wpisz tylko nazwę, bez znaku '@' i domeny, na przykład: *algebra* zamiast *algebra@{{conf.host}}*).

    | Note |
    |------|
    | Nie używaj spacji, akcentów lub znaków specjalnych w nazwach list: takie znaki mogą powodować problemy. |

    | Note |
    |------|
    | Wybierz konkretną i krótką nazwę: pamiętaj o subskrybentach, którzy będą wpisywać nazwę listy za każdym razem, kiedy będą wysłać na nią wiadomość! Jeśli zarządzasz kilkoma listami, możesz używać wspólnego prefiksu w ich nazwach; wtedy będą występować obok siebie i będą łatwo rozpoznawalne (na przykład: *xx-users@{{conf.host}}, xx-hotline@{{conf.host}}*, itp.). |

4.  Wybierz **typ listy** z listy predefiniowanych typów (typy predefiniowane stanowią przykłady typowych konfiguracji, które po utworzeniu listy mogą być modyfikowane przez właściciela; z pomocą administratora możliwa jest nawet konfiguracja wykraczająca poza opcje z modułu administratorskiego).
5.  Wpisz **temat** listy. Temat wyświetlany jest jako nagłówek na wszystkich stronach listy, będzie też widoczny na stronach indeksów (spis list, lista subskrypcji, itp.), a także na pasku przeglądarki.
6.  Wybierz **kategorię** z rozwijalnej listy.

    | Note |
    |------|
    | Jeśli żadna kategoria nie jest odpowiednia, możesz poprosić administratorów o utworzenie nowej. |

7.  Wpisz **opis** listy. Opis będzie wyświetlany na stronie informacyjnej listy, a także rozsyłany w wiadomości powitalnej do nowych subskrybentów, pod sekcją 'Temat listy'. W opisie można zawrzeć informacje na temat:

    -   przeznaczenia i celów listy;
    -   dyskutowanych tematów;
    -   odpowiedzialności i statusu listy;
    -   obowiązujących reguł;
    -   typowych subskrybentów (ich zajęcia, powiązanych projektów, narodowości, itp.).

    | Note |
    |------|
    | Możesz sformatować opis listy za pomocą tagów HTML. Uwaga: jeśli opis jest długi, podziel go ręcznie (klawisz ENTER na klawiaturze); w przeciwnym wypadku może nie być w całości widoczny w oknie przeglądarki. |

8.  Kliknij przycisk '**Utwórz listę**'.

Następnie zostanie wyświetlona informacja, że prośba o utworzenie została wysłana do administratorów i od tego momentu możesz dostosowywać listę za pomocą przycisku 'Admin'. Wiadomość jednak ostrzega, że dopiero po zatwierdzeniu przez administratora lista zostanie zainstalowana i będzie widoczna na serwerze.

Następnie należy **poczekać na zatwierdzenie prośby o utworzenie listy przez jednego z administratorów**. Po zatwierdzeniu otrzymasz wiadomość zatytułowaną '**Utworzenie listy nazwalisty**', potwierdzającą faktyczne utworzenie listy.

**Na końcu zapisz się na swoją listę**: utworzenie listy, czy zostanie jej właścicielem lub moderatorem nie oznacza automatycznie subskrypcji!

### Zarządzanie listą

Aby zarządzać swoją listą, należy wykonać kolejno kroki:

1.  Przejdź do **strony domowej środowiska list** i **[zaloguj się](user#sympa_auth.md)**.

    | Note |
    |------|
    | Jeśli używasz kilku adresów email, użyj tego, z którym prosiłeś o utworzenie listy. |

2.  **Przejdź do strony informacyjnej listy**.
3.  W lewym menu **kliknij link 'Admin'**.

Aby zobaczyć sekcje w module administracyjnym, użyj linków poniżej linku 'Admin' w lewym menu.

Różne sekcje pozwalają na:

-   [konfigurowanie listy](listconfig.md);
-   [dostosowanie plików związanych z listą](#customize);
-   [zarządzanie subskrybentami](#manage_members);
-   [zarządzanie archiwum listy](#manage_archives);
-   [zarządzanie obiciami](#manage_bounces);
-   [tworzenie, usuwanie i przywracanie przestrzeni dokumentów współdzielonych](#manage_shared);
-   [zmianę nazwy listy](#renamelist);
-   [usunięcie listy](#supprlist).

Opcje dostępne w sekcji 'Moderacja' pozwalają na:

-   [moderację wiadomości](#moderate) wysyłanych na listę;
-   [moderację dokumentów](shared.md) dostępnych w przestrzeni dokumentów współdzielonych;
-   [moderowanie oczekujących subskrypcji](#manage_members).

#### <span id="edit_list"></span>Konfigurowanie listy

Informacje jak konfigurować listę znajdziesz w [**dokumentacji na temat konfigurowania list**](listconfig.md).

#### <span id="customize"></span>Dostosowywanie listy

Na tej stronie, możesz **edytować pliki związane z listą**, w tym:

-   typowe wiadomości wysyłane do subskrybentów w konkretnych sytuacjach:
    -   **wiadomość powitalna**: wiadomość wysyłana jest do nowych subskrybentów. Powinieneś stworzyć statut listy i dołączyć go do wiadomości powitalnej. Możesz utworzyć wiadomość powitalną w formacie MIME;
    -   **wiadomość opuszczenia listy**: wiadomość jest wysyłana do osób, które przestają subskrybować listę;
    -   **wiadomość usunięcia**: wiadomość wysyłana jest do osób, które zostały usunięte z listy (polecenie DEL), w szczególności z powodu zwrotów wiadomości wysyłanych na ich adres;
    -   **wiadomość przypominająca**: wiadomość wysyłana jest do subskrybentów w efekcie użycia polecenia REMIND. Ponieważ wiele zwrotów wiadomości powodowanych jest tym, że adres zapisany na listę nie jest już aktualnym adresem subskrybenta, poza tym niektórzy ludzie zapominają o swoich subskrypcjach, polecenie REMIND jest niezwykle istotne dla dobrego zarządzania listą,
    -   **wiadomość z zaproszeniem**: wiadomość jest wysyłana do osób, które zostały zaproszone na listę przy użyciu polecenia INVITE;
    -   **informacja o odrzuceniu wiadomości przez moderatora**: wiadomość jest wysyłana do nadawców wiadomości odrzuconych przez moderatora;
    -   **informacja o odrzuceniu wiadomości z powodu wirusa**: wiadomość jest wysyłana do nadawców, w których wiadomości znaleziono wirus.
-   różne pliki:
    -   **opis listy**: opis listy wysyłany jest jako wiadomość email w efekcie użycia polecenia INFO. Domyślnie dołączony jest także do wiadomości powitalnej. Opis nie jest tym samym, co strona listy wyświetlana w interfejsie webowym;
    -   **strona domowa listy**: ten opis dostępny jest na stronie informacyjnej listy. Może być w formacie HTML. Nawet jeśli nie używasz tego formatu, użyj tagów `<br />` do oznaczenia końców linii;
    -   **nagłówek wiadomości**: jeśli zdefiniowany, umieszczany jest w postaci załącznika MIME na początku każdej wiadomości wysyłanej na listę;
    -   **stopka wiadomości**: jeśli zdefiniowana, umieszczana jest jako załącznik MIME na końcu każdej wiadomości wysyłanej na listę.

Domyślnie Sympa używa plików domyślnych; w takiej sytuacji specyficzne pliki związane z Twoją listą są puste. **Aby wyedytować plik, wybierz go z rozwijalnej listy i kliknij przycisk 'Edytuj'**. Będziesz mieć możliwość zmiany **pola 'Od'** (nadawca), **pola 'Temat'** (temat wiadomości) i **treści wiadomości**.

| Note |
|------|
| Uwaga: wartości pomiędzy nawiasami kwadratowymi to zmienne. Nie zmieniaj ich, chyba że naprawdę wiesz co robisz... |

#### <span id="manage_shared"></span>Zarządzanie przestrzenią dokumentów współdzielonych

Domyślnie, listy nie mają przestrzeni plików współdzielonych, trzeba więc ją utworzyć. Aby to zrobić, przejdź do **modułu administracyjnego listy** i kliknij link '**Utwórz współdzielone**'.

Aby zezwolić subskrybentom publikować dokumenty w przestrzeni dokumentów współdzielonych, musisz **zmienić domyślne uprawnienia**: w module administracyjnym listy kliknij '**Edytuj konfigurację listy**', a potem '**Uprawnienia**'. Na dole strony jest rozwijalna lista zatytułowana '[**Kto może edytować**](listconfig#docsrights.md)'; tam wybierz opcję '**Ograniczone do subskrybentów (private)**'.

| Note |
|------|
| Uwaga: jeśli stworzyłeś katalogi przed poprawieniem uprawnień, nadal nie będzie się dało do nich nic zapisać. Jeśli chcesz to poprawić, musisz [zmienić prawa dostępu](shared#acces.md) do każdego z katalogów. |

Istotne może być też [ustawienie **kwot**](listconfig#docsrights.md) dla przestrzeni dokumentów współdzielonych na stronie 'Uprawnienia' sekcji 'Edytuj konfigurację listy'.

Aby **dowiedzieć się więcej na temat zarządzania przestrzenią dokumentów współdzielonych** (jak ją zorganizować, zmieniać prawa dostępu, nazywać dokumenty, itp.), przejrzyj sekcję '[Korzystanie z przestrzeni dokumentów współdzielonych](shared.md)' podręcznika użytkownika.

Aby **zabronić dostępu do przestrzeni dokumentów współdzielonych**, kliknij '**Usuń współdzielone**' w sekcji 'Admin'. W ten sposób zachowasz możliwość **przywrócenia przestrzeni** za pomocą kliknięcia '**Przywróć współdzielone**'. Usuwanie i przywracanie przestrzeni dokumentów współdzielonych **nie ma żadnego wpływu na zawierane przez nią dokumenty**.

#### <span id="manage_members"></span>Zarządzanie subskrybentami

Ta sekcja pozwala przeglądać **spis subskrybentów listy**. Dla każdego subskrybenta dostępne są następujące informacje:

-   **adres email**;
-   **domena** adresu email (*@cru.fr*, *@sympa.org*, *@fai.com*, itp.);
-   **zdjęcie** (jeśli funkcjonalność została aktywowana dla tej listy);
-   **nazwa** (w zależności od metody subskrypcji, nie zawsze jest wyświetlana);
-   [**tryb dostarczania wiadomości**](#deliverymode);
-   **źródło danych** określające pochodzenie subskrybenta w przypadku, gdy nie jest zapisany na listę bezpośrednio;
-   **data subskrybowania** listy;
-   **ostatnia aktualizacja** opcji subskrybenta.

| Note |
|------|
| Domyślnie każda strona wyświetla 25 subskrybentów. Możesz nawigować pomiędzy stronami używając strzałek lub wyświetlać więcej subskrybentów na stronę. Klikając na nagłówek odpowiedniej kolumny można sortować subskrybentów według danego kryterium. |

Aby **wyszukać subskrybenta**, wpisz cały lub część adresu email w pole tekstowe i kliknij przycisk '**Szukaj**'.

Na tej stronie możesz **dodawać inne osoby do listy**:

-   Aby dodać **pojedynczą osobę**, wpisz jej/jego adres email w pole tekstowe i kliknij przycisk '**Dodaj**'.
-   Aby dodać **kilka osób**, kliknij przycisk '**Wielokrotne dodanie**'. Następnie w polu tekstowym wpisz adresy email i nazwy osób, które chcesz dodać do listy i kliknij '**Dodaj subskrybentów**'.

| Note |
|------|
| Jeśli chcesz dodać ludzi bez wysyłania im informacji, zaznacz opcję 'Cisza'. Jednak dużo lepiej jest ostrzegać nowo dodanych subskrybentów! |

Mimo, że masz możliwość dodawania ludzi do Twoich list, zawsze **jest lepiej, gdy zapisują się sami**. Możesz także **zaprosić ludzi do uczestnictwa w liście** za pomocą polecenia INVITE. W tym celu wyślij wiadomość email na adres {{conf.email}}@{{conf.host}} w jej treści wpisując **invite nazwalisty adresemail** (przykład: *invite list\_example john.doe(@)fai.com*).

Aby **zaakceptować lub odrzucić prośby o subskrypcję**, kliknij '**Oczekujące subskrypcje**'. Wyświetli się lista wszystkich osób, które poprosiły o subskrypcję. Aby zaakceptować lub odrzucić prośbę, zaznacz daną osobę i kliknij odpowiedni przycisk.

Aby **wysłać przypomnienie o subskrypcji do wszystkich subskrybentów**, kliknij przycisk '**Przypomnij wszystkim**'. Wiadomość przypominająca zawiera:

-   **nazwę listy** subskrybowanej przez subskrybenta;
-   **adres email** subskrybenta;
-   **hasło do list** subskrybenta;
-   **link do strony informacyjnej** listy;
-   **klikalny adres pozwalający subskrybentom na opuszczenie** listy.

| Note |
|------|
| Możesz także skonfigurować automatyczne wysyłanie przypomnienia o subskrypcji poprzez stronę '[Różne](listconfig#other.md)' sekcji 'Edytuj konfigurację listy'. |

Aby **wypisać subskrybentów z listy**, zaznacz ich a następnie kliknij przycisk '**Usuń zaznaczone adresy email**'.

| Note |
|------|
| Jeśli nie chcesz powiadamiać subskrybentów, zaznacz opcję 'Cisza'. Nie polecamy tego jednak, oprócz przypadku odbijających subskrybentów. |

| Note |
|------|
| Aby zaznaczyć wszystkich subskrybentów na raz, upewnij się że widoczni są na jednej stronie, a następnie kliknij przycisk 'Zaznacz wszystkich': w ten sposób wszyscy zostaną zaznaczeni pojedynczym kliknięciem! |

Aby **zmienić opcje subskrypcji danego subskrybenta**, kliknij jej/jego adres email.

Na tej stronie, możesz **zmienić nazwę, adres email i tryb dostarczania wiadomości subskrybenta**. Możesz także **wypisać subskrybenta z listy**.

Jeśli adres subskrybenta [zwraca wiadomości](#manage_bounces), pod formularzem 'Informacje o subskrybencie' wyświetla się kolejny formularz:

Wyświetlane informacje zawierają:

-   rodzaj błędu (w języku angielskim);
-   ilość błędów;
-   okres kiedy występowały błędy.

Możesz **sprawdzić ostatnie błędy** lub **zresetować błędy**. Jeśli zresetujesz błędy, [licznik błędów](listconfig#bouncers.md) subskrybenta będzie wynosić zero.

Aby w łatwy sposób zarządzać zwracanymi wiadomościami, przejdź do strony '[Zwrotki](#manage_bounces)' modułu administracyjnego.

#### <span id="manage_bounces"></span>Zarządzanie odbiciami

Jeśli występuje **problem z adresem email subskrybenta** (adres nieaktualny, czasowo niedostępny, przekroczona kwota skrzynki, itp.), procent zwrotów wyświetlany jest w lewym menu pod tekstem '**Współczynnik błędu**'. Aby sprawdzić adresy zwracające wiadomości, przejdź do strony '**Zwrotki**' modułu administracyjnego.

Oprogramowanie Sympa automatycznie zarządza subskrybentami, których adresy zwracają wiadomości: w zależności od liczby błędów i ruchu na liście takie osoby są powiadamiane, usuwane z listy, a jeśli zwrotki przestają przychodzić, ich liczniki błędów są zerowane.

Aby **wyzerować liczniki błędu**, zaznacz odpowiednie adresy i kliknij przycisk '**Zresetuj błędy dla zaznaczonych użytkowników**'. Jeśli błąd nadal występuje, adresy będą ponownie oznaczone jako wysyłające zwrotki, jak tylko na listę zostanie wysłana następna wiadomość.

Możesz także **wypisać z listy subskrybentów, których adresy zwracają wiadomości**: zbyt dużo takich adresów powoduje znaczące zwiększenie obciążenia serwera list mailingowych. Aby wypisać użytkowników, zaznacz ich i kliknij przycisk '**Usuń zaznaczone adresy email**'.

| Note |
|------|
| Aby zaznaczyć wszystkich subskrybentów na raz, upewnij się że widoczni są na jednej stronie, a następnie kliknij przycisk 'Zaznacz wszystkich': w ten sposób wszyscy zostaną zaznaczeni pojedynczym kliknięciem! |

#### <span id="moderate"></span>Moderacja wiadomości wysyłanych na listę

Jeśli lista jest moderowana, **wszystkie wiadomości muszą być zaakceptowane przez jednego z moderatorów, zanim zostaną rozesłane na listę**. Po wysłaniu wiadomości na adres listy, subskrybenci są automatycznie powiadamiani mailowo, że wiadomość trafiła do moderacji. Moderatorzy natomiast otrzymują od Sympy informację zawierającą nadesłaną wiadomość.

**Zadania związane z moderowaniem** możesz wykonywać albo **za pośrednictwem maili**, odpowiadając na wiadomości otrzymane od Sympy, albo **za pośrednictwem interfejsu webowego**. Aby skorzystać z drugiego sposobu, kliknij link '**Wiadomości**' w sekcji 'Moderacja': zostaną wyświetlone wszystkie wiadomości wymagające decyzji moderatora (najnowsze są na górze strony). **Aby przeczytać wiadomość, kliknij jej temat**.

Masz **dwie opcje**:

-   **pozwolić na rozesłanie wiadomości** na listę;
-   **odrzucić wiadomość i powiadomić nadawcę**: kiedy odrzucasz wiadomość, dobrze jest powiadomić o tym jej nadawcę...

Każdy z moderatorów może zadecydować o zaakceptowaniu lub odrzuceniu wiadomości. Jednak **decyzja należy do tego z nich, który pierwszy zajmie się daną wiadomością**. Jeśli spróbujesz przetworzyć wiadomość, która już była moderowana, dostaniesz powiadomienie od Sympy. Jeśli jest kilku moderatorów, **łatwiej jest moderować wiadomości za pomocą interfejsu webowego**: w ten sposób moderatorzy będą widzieli, które wiadomości zostały do przetworzenia.

| Note |
|------|
| **Niezależnie od czasu moderacji, data i godzina wysłania wiadomości pozostają bez zmian**. Dlatego, jeśli dystrybucja wiadomości jest bardzo opóźniona, 31 grudnia można dostać wiadomość datowaną na 1 stycznia! |

Jeśli wiadomość została odrzucona z powiadomieniem, subskrybent który ją wysłał, dostaje informację mailem. Możesz [dostosować powiadomienie o odrzuceniu wiadomości](#customize).

Zaznaczenie '**Odrzuć bez powiadamiania**' pozwala odrzucić wiadomość bez powiadamiania autora o tym fakcie.

Zaznaczenie '**Dodaj do czarnej listy**' powoduje niewysyłanie powiadomienia i dodaje autora wiadomości do czarnej listy. Czarną listą można zarządzać poprzez przycisk '**edytuj czarną listę**' na dole strony.

Jeśli chcesz dostosować wiadomość o odrzuceniu wiadomości wysyłaną do jej autora, możesz to zrobić przy pomocy przycisku '**Zarządzaj wiadomościami o odrzuceniu**'. Strona pozwoli zdefiniować zbiór wiadomości o odrzuceniu i wiadomość domyślną.

**Przypomnienie**: możesz [dodawać i usuwać moderatorów](listconfig#description.md) w module administracyjnym. Aby to zrobić, kliknij '**Admin**', następnie '**Edytuj konfigurację listy**', a na końcu '**Definicja listy**'.

Jest także możliwe **przetwarzanie wiadomości po ich rozdystrybuowaniu na listę**: może to być przydatne w przypadku list niemoderowanych. Jeśli chcesz **usunąć wiadomość**, [wyszukaj ją w archiwum online](arc#arcsearch.md) i kliknij przycisk '**Zaznacz wiadomość do usunięcia**' w prawym górnym rogu. Wyświetli się potwierdzenie, kliknij 'OK'. Wiadomość zostanie po kilku sekundach usunięta. **Uwaga: ta operacja jest nieodwracalna!!! Jeśli usuniesz wiadomość, nie będzie się dało jej odtworzyć.**

#### <span id="manage_archives"></span>Zarządzanie archiwami

Oprogramowanie Sympa może generować **skompresowane archiwum wiadomości w formacie ZIP**. Aby pobrać archiwum, **zaznacz miesiące**, które Cię interesują i kliknij przycisk '**Pobierz plik ZIP**'.

| Note |
|------|
| Wskazówka: na liście 'Wybór archiwum', aby zaznaczyć okres wysyłania wiadomości, kliknij pierwszy miesiąc, przytrzymaj klawisz SHIFT i kliknij ostatni miesiąc na liście. |

Otrzymasz plik o nazwie '**nazwalisty\_archive.zip**' zawierający **katalogi o nazwach 'nazwa listy\_rok-miesiąc'** (przykład: *lista\_2005-06*) na każdy miesiąc. W każdym z katalogów, **nazwy plików to liczby** oznaczające kolejność wysyłania wiadomości (przykład: plik o nazwie '1' zawiera pierwszą wiadomość z danego miesiąca). Pliki z wiadomościami **nie mają żadnych rozszerzeń**; do ich otwarcia można użyć dowolnego edytora (Notepad, WordPad, Vim, itp.). **Każdy plik reprezentuje całą wiadomość wraz z nagłówkami**.

Na stronie 'Zarządzaj archiwum' możesz także **usuwać wiadomości** (miesiąc po miesiącu, nie wiadomość po wiadomości). Aby to zrobić, **zaznacz miesiące** i kliknij przycisk '**Usuń zaznaczone miesiące**'.

| Note |
|------|
| **Uwaga: ta operacja jest nieodwracalna!!! Jeśli klikniesz 'Usuń zaznaczone miesiące', pamiętaj że usuwasz nie tylko pliki z archiwum, ale wszystkie wiadomości z zaznaczonych miesięcy!!!** |

#### <span id="renamelist"></span>Zmiana nazwy listy

W **module administracyjnym listy**, kliknij '**Zmień nazwę listy**'. Wpisz nową nazwę i kliknij przycisk 'Zmień nazwę listy'. Pojawia się potwierdzenie, kliknij 'OK'.

| Note |
|------|
| Jeśli zmienisz zdanie, wystarczy wykonać odwrotną operację aby przywrócić poprzednią nazwę listy. |

**Uwaga: przy zmianie nazwy listy należy powiadomić administratorów, w przeciwnym wypadku nazwa nie zostanie zmieniona**.

Kilka wskazówek, jak nazwać listę:

-   **Nie używaj spacji, akcentów ani znaków specjalnych** w nazwach list: takie znaki mogą powodować problemy.
-   Wybierz **znaczącą i jednocześnie krótką nazwę**: pamiętaj, że subskrybenci będą wpisywać nazwę przy każdym wysyłaniu wiadomości na listę!
-   Jeśli zarządzasz kilkoma listami, możesz **poprzedzić ich nazwy wspólnym prefiksem**; będą wtedy pojawiać się obok siebie w spisach i będą łatwo rozpoznawalne (przykład: *xx-users@lista.uw.edu.pl, xx-hotline@lista.uw.edu.pl.fr*, itp.).

#### <span id="supprlist"></span>Usuwanie listy

W **module administracyjnym**, kliknij '**Usuń listę**'. Pojawia się potwierdzenie, kliknij 'OK'.

| Note |
|------|
| **Uwaga: jeśli usuniesz listę, nie będziesz mógł samodzielnie jej odzyskać!!! Jeśli chcesz odzyskać usuniętą listę, musisz poprosić o to administratorów.** |

Jakie są **konsekwencje** usunięcia listy?

-   **Wszyscy subskrybenci są natychmiast usuwani z listy** (włączając w to właścicieli i moderatorów).
-   **Archiwum wiadomości jest zachowane**, ale nikt nie ma do niego dostępu.
-   **Dokumenty opublikowane w przestrzeni dokumentów współdzielonych są zachowane**, ale nikt nie ma do nich dostępu.
-   **Tylko administratorzy mają możliwość przywrócić listę**; jeśli to zrobią, byli subskrybenci zostaną automatycznie na nowo zapisani.

| Note |
|------|
| Uwaga: z uwagi na niewielkie opóźnienie, strony listy pozostaną przez jakiś czas dostępne, jeśli ktoś zna ich adresy. Po pewnym czasie staną się niedostępne. |

**Jeśli chcesz, aby lista i związane z nią pliki zostały całkowicie usunięte**, musisz poprosić o to administratorów.

### <span id="rulesadmin"></span>Dobre praktyki

Aby listy były dynamiczne, musisz **zaangażować się** w ich utrzymywanie: jeśli lista nie jest kontrolowana przez właścicieli, efektem może być spadek jakości wiadomości, a nawet zniknięcie listy...

**Używanie poczty elektronicznej w ogólności i na listach mailingowych wiąże się ze zbiorem precyzyjnych reguł: "Netykietą"**. Twoją rolą jako właściciela listy lub moderatora jest dbanie o to, aby subskrybenci jej przestrzegali. Ogólne zasady netykiety wraz z wieloma linkami znajdziesz na [stronie Wikipedii poświęconej Netykiecie](http://pl.wikipedia.org/wiki/Netykieta).

<span id="charter"></span>Powinieneś **stworzyć statut listy**, aby zdefiniować reguły związane z jej używaniem:

-   tematy dozwolone, tolerowane i zabronione;
-   reguły pisania wiadomości (w jakim języku powinny być pisane, itp.);
-   reguły związane z wysyłaniem wiadomości (częstotliwość, załączniki, itp.);
-   reguły związane z netykietą;
-   prawa i obowiązki subskrybentów;
-   informacje związane ze wstrzymywaniem wiadomości wysyłanych na listę;
-   informacje prawne i polityka prywatności;
-   sankcje grożące za nieprzestrzeganie reguł;
-   itd.

| Note |
|------|
| Aby umożliwić subskrybentom zapoznanie się ze statutem listy, powinieneś dołączyć dokument do wiadomości, którą ludzie dostają po zapisaniu się na listę. Aby to zrobić, musisz [dostosować tą wiadomość](#customize) poprzez stronę 'Dostosuj' modułu administracyjnego. |

~~When available, the 'Owner and moderator charter' provides list owners and moderators with all the necessary information to carry out their roles. This Charter involves all the rights and responsibilities of owners and moderators.~~

------------------------------------------------------------------------
