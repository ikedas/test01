<span id="listconfig"></span>Konfigurowanie listy
-------------------------------------------------

Ze względu na złożoność, konfiguracja listy podzielona jest na kilka części z osobną stroną dla każdej z nich:

-   [Definicja listy](#description);
-   [Wysyłanie/otrzymywanie](#sending);
-   [Uprawnienia](#command);
-   [Archiwa](#archives);
-   [Zwroty](#bounces);
-   [Różne](#other).

Radzimy **dokonywać zmian w konfiguracji małymi krokami**: w ten sposób, jeśli wynik nie spełnia oczekiwań, można zmianę łatwo wycofać.

Moduł administracyjny zawiera **wiele opcji konfiguracyjnych listy**. Niestety, opcje niekoniecznie spełnią wszystkie potrzeby. Aby temu zaradzić, możesz **poprosić administratora o utworzenie nowych opcji** (na tyle na ile to możliwe...): dostęp i/lub uprawnienia ograniczone do pewnej kategorii osób w zależności od sposobu w jaki się logują, domeny ich adresów email, grup do których należą, itp.

### <span id="description"></span>Definicja listy

W polu '**Temat listy**' możesz zmienić temat, który wybrałeś podczas tworzenia listy. Temat wyświetlany jest jako nagłówek na wszystkich stronach związanych z listą, jest także widoczny na wszystkich stronach indeksów (spis list, lista subskrypcji, itp.), a także na pasku tytułowym przeglądarki.

Możesz także zmienić '**Widoczność listy**'. Dostępne opcje:

-   ukryta z wyjątkiem subskrybentów (conceal) - *opcja domyślna*;
-   dostęp z intranetu (intranet);
-   widoczna (noconceal);
-   ukryta nawet dla subskrybentów (secret);

| Note |
|------|
| Jeśli chcesz ograniczyć widoczność na podstawie innego kryterium, powinieneś poprosić o to administratorów: być może będą mogli utworzyć nową opcję spełniającą wymagania (na przykład: lista widoczna dla członków danej grupy, domeny internetowej, itp.). |

Za pomocą pól 'Właściciele' i 'Moderatorzy' możesz **dodawać właścicieli i moderatorów** do listy lub **zmieniać ich dane**.

-   Dla każdego właściciela/moderatora trzeba podać **adres email** i **nazwę**.
-   W polu '**Informacje prywatne**' możesz podać dodatkowe dane (przykładowo numer telefonu, funkcje, itp.); informacje te będą widoczne jedynie dla administratorów i właścicieli listy z profilem 'Uprzywilejowany'.
-   Możesz zmienić **tryb dostarczania wiadomości** (opcje dostępne na tej stronie obejmują zwykłe dostarczanie i brak wiadomości).
-   Parametr 'Profil' nie może być zmieniony: **profil 'Uprzywilejowany'** zarezerwowany jest dla twórcy listy (inni właściciele mają profil 'Normalny').

| Note |
|------|
| Uwaga: właściciele i moderatorzy listy nie są automatycznie na nią zapisywani. Powinni ręcznie zapisać się na listę. |

Aby **usunąć właścicieli/moderatorów**, usuń zawartość pól odnoszących się do osoby, którą chcesz usunąć i kliknij przycisk 'Zapisz'.

Możesz także zmienić **temat listy**, a także jej **język**. Jeśli zmienisz język listy, wszystkie wiadomości będą wysyłane w nowym języku (uwaga: na ile dostępne są odpowiednie tłumaczenia!).

Możesz zmienić **domenę** listy: tylko administratorzy mogą zmieniać wartość tego parametru.

**UWAGA: nie zapomnij kliknąć przycisku 'Zapisz'** na dole strony, aby zatwierdzić dokonane zmiany.

### <span id="sending"></span>Wysyłanie/odbieranie

Na tej stronie możesz **decydować, kto ma prawo wysyłać wiadomości na listę**.

W polu '**Częstotliwość wysyłania wiadomości zbiorczej**' możesz zdefiniować, jak często wysyłane są wiadomości zbiorcze (tryby Digest i Podsumowanie): wybierz **dni**, w które powinny być wysyłane wiadomości. Potem wybierz **czas wysyłania** wiadomości zbiorczej (unikaj wysyłania pomiędzy 23.00 a północą).

Na liście '**Dostępne opcje subskrypcji**' zaznacz wszystkie opcje, które powinny być dostępne dla subskrybentów. Domyślnie zaznaczone są wszystkie opcje.

Pole '**Adres Reply**' pozwala zdefiniować domyślnego odbiorcę wszystkich odpowiedzi na wiadomości wysyłane na listę:

-   Jeśli wartość to '**Wszyscy**', odpowiedzi wysyłane są zarówno do **nadawcy wiadomości** i na **listę**.
-   Jeśli wartość to '**Lista**', odpowiedzi wysyłane są na **listę**.

    | Note |
    |------|
    | Uwaga: używaj tej opcji ostrożnie! Doświadczenie pokazuje, że subskrybenci nie zawsze sprawdzają adres, na który wysyłają odpowiedź. Dlatego może się zdarzyć, że wyślą prywatną wiadomość na listę próbują ją wysłać do konkretnej osoby... |

-   Jeśli wartość to '**Inny adres**', odpowiedź wysyłana jest do **zdefiniowanego adresu**. Jeśli wybierzesz tą opcję, musisz **podać adres email w polu 'Inny adres email'**.
-   Jeśli wartość to '**Nadawca**', odpowiedź wysyłana jest do **nadawcy wiadomości**. Tą wartość powinieneś prawdopodobnie wybrać.

Rozwijalna lista '**Zachowaj nagłówek**' pozwala zdefiniować, jak nagłówek SMTP 'Reply-To' będzie przetwarzany. Opcja '**Respect**' zachowuje nagłówek, natomiast opcja '**Forced**' pozwala na jego nadpisywanie.

Opcja '**Tagowanie tematu**' pozwala wybrać **tekst dopisywany na początku tematu każdej wiadomości** wysyłanej na listę: to pomaga subskrybentom łatwo sortować otrzymywane wiadomości, automatycznie przetwarzać wiadomości za pomocą filtrów, itp. Domyślnie, prefiks zawiera **nazwę listy otoczoną nawiasami kwadratowymi** (nawiasy kwadratowe są automatycznie dodawane przez system, nie ma więc potrzeby dodawać je ręcznie).

**UWAGA: nie zapomnij kliknąć przycisku 'Zapisz'** na dole strony, aby zatwierdzić dokonane zmiany.

### <span id="command"></span>Uprawnienia

Na tej stronie możesz określać:

-   **kto może przeglądać informacje o liście**. Dostępne są następujące opcje:
    -   dla wszystkich (open) - *wartość domyślna*;
    -   zastrzeżone dla subskrybentów (private).
-   **kto może subskrybować listę**. Dostępne są następujące opcje:
    -   zatwierdzanie prośby o subskrypcję (auth);
    -   potrzeba uwierzytelnienia (powiadomienie wysyłane do właścicieli) (auth\_notify);
    -   potrzeba uwierzytelnienia, a następnie zgody właściciela (auth\_owner);
    -   subskrypcja niemożliwa (closed);
    -   zastrzeżone dla użytkowników lokalnej domeny (intranet);
    -   użytkownicy lokalnej domeny lub zgoda właściciela (intranetorowner);
    -   dla każdego bez uwierzytelniania (open) - *opcja domyślna*;
    -   dla każdego, powiadomienie wysyłane jest do właściciela listy (open\_notify);
    -   dla każdego, bez wiadomości powitalnej (open\_quiet);
    -   zgoda właściciela (owner);
    -   wymaga podpisu S/MIME (smime);
    -   wymaga podpisu S/MIME lub zgody właściciela (smimeorowner).

        | Note |
        |------|
        | Zawsze powinieneś wybierać opcje z parametrem 'auth': w ten sposób system będzie wymagać potwierdzenia prośby o subskrypcję od potencjalnego subskrybenta. Pozwala to uniknąć nieprawidłowych adresów email i zapewnia, że nikt nie zostanie zapisany na listę nie wiedząc o tym. |

-   **kto może wypisać się z listy**. Dostępne są następujące opcje:
    -   wymaga uwierzytelnienia (auth);
    -   wymagane uwierzytelnienie, powiadomienie wysyłane do właściciela (auth\_notify);
    -   niemożliwe (closed);
    -   otwarte (open) - *opcja domyślna*;
    -   otwarte z potwierdzeniem mailowym, właściciel jest powiadamiany (open\_notify);
    -   zgoda właściciela (owner).

        | Note |
        |------|
        | Powinieneś zawsze wybierać opcje zawierającą parametr 'auth': w ten sposób system wymaga od subskrybenta potwierdzenia chęci wypisania się z listy. To zapobiega wypisywania osób bez ich wiedzy. |

-   **kto może zapraszać ludzi do subskrybowania listy**. Dostępne są następujące opcje:
    -   zamknięte (closed);
    -   właściciel listy, bez uwierzytelniania (owner);
    -   zastrzeżone dla subskrybentów (private) - *opcja domyślna*;
    -   publiczne (public).
-   **kto może przeglądać subskrybentów**. Dostępne są następujące opcje:
    -   nikt nie może przeglądać (closed);
    -   zastrzeżone dla subskrybentów lub użytkowników lokalnej domeny (intranet);
    -   tylko administrator (listmaster);
    -   tylko właściciel (i administrator) (owner) - *opcja domyślna*;
    -   zastrzeżone dla subskrybentów (private);
    -   każdy! (public).

        | Note |
        |------|
        | Nie powinieneś pozwalać każdemu na dostęp do listy subskrybentów. Opcja 'Zastrzeżone dla subskrybentów' może przydać się do ułatwienia komunikacji między subskrybentami bez wysyłania wiadomości na listę. Jednak nie jest to właściwa opcja w przypadku listy dystrybucyjnej, której subskrybenci nie są powiązani. |

<span id="docsrights"></span>Na tej stronie możesz także **zdefiniować uprawnienia odnoszące się do przestrzeni dokumentów współdzielonych** (sekcja 'Dokumenty współdzielone' dostępna poprzez link w lewym menu). Możesz zdefiniować prawa do odczytu i zapisu dokumentów:

-   Następujące opcje są dostępne na liście rozwijalnej '**Kto może przeglądać**':
    -   zastrzeżone dla subskrybentów lub użytkowników lokalnej domeny (intranet);
    -   zastrzeżone dla właścicieli (owner);
    -   zastrzeżone dla subskrybentów (private) - *opcja domyślna*;
    -   publiczne dokumenty (public).
-   Następujące opcje są dostępne na liście rozwijalnej '**Kto może edytować**':
    -   zastrzeżone dla właścicieli (owner) - *opcja domyślna*;
    -   moderowane dla subskrybentów (editor);
    -   zastrzeżone dla subskrybentów (private);
    -   publiczne dokumenty (public).

Pole '**Kwota**' pozwala zdefiniować **maksymalny rozmiar przestrzeni dokumentów współdzielonych**. Nie dotyczy to rozmiaru *pojedynczego* opublikowanego dokumentu, ale sumy rozmiarów wszystkich opublikowanych dokumentów. Rozmiar wyrażony jest w kilobajtach. Subskrybent, który próbuje opublikować zbyt duży dokument, dostaje komunikat błędu.

Aby dowiedzieć się **więcej na temat zarządzania przestrzenią dokumentów współdzielonych** (jak ją zorganizować, zmieniać prawa dostępu, nazywać dokumenty, itp.), zapoznaj się z sekcją '[Używanie przestrzeni dokumentów współdzielonych](shared.md)'.

**UWAGA: nie zapomnij kliknąć przycisku 'Zapisz'** na dole strony, aby zatwierdzić dokonane zmiany.

### <span id="archives"></span>Archiwa

Na tej stronie możesz **decydować, kto może przeglądać archiwum listy online** (wiadomości wysyłane na listę dostępne z interfejsu webowego). Dostępne są następujące opcje:

-   zamknięte (closed);
-   zastrzeżone dla użytkowników lokalnej domeny (intranet);
-   administrator (listmaster);
-   właściciel (owner);
-   ~~moderator (moderator);~~
-   tylko subskrybenci (private);
-   publiczne (public).

Pole '**Kwota**' pozwala zdefiniować **maksymalny rozmiar archiwum listy**. Rozmiar wyrażony jest w kilobajtach. Właściciele listy są powiadamiani, gdy rozmiar archiwum przekroczy 95 % dozwolonej wartości. Jeśli archiwum osiągnie maksymalny rozmiar, wiadomości przestają być archiwizowane.

| Note |
|------|
| Nawet jeśli wiadomości nie są archiwizowane, oczywiście nadal jest możliwe wysyłać wiadomości na listę. |

Możliwy jest także **dostęp do archiwum listy za pośrednictwem email**, przez wysłanie na adres **{{conf.email}}@{{conf.host}}** następującego polecenia: <span class="commande">**GET nazwalisty rokmiesiąc**</span> (na przykład: *GET list\_example 2016-07*). W odpowiedzi otrzymasz zbiór wiadomości wysłanych w wybranym miesiącu. Zbiór jest wysyłany plain tekstem i zawiera tagi HTML zamiast oryginalnego formatowania; zawiera także pełne nagłówki każdej wiadomości. Parametr '**Archiwa tekstowe**' pozwala zdefiniować:

-   **kto jest uprawniony** do otrzymywania archiwów wiadomości za pośrednictwem email;
-   **jak często archiwa będą tworzone**. Na przykład, jeśli częstotliwość ustawiona jest na 'miesiąc', wszystkie wiadomości wysyłane na listę w danym miesiącu będą zbierane w jednym archiwalnym pliku.

Jeśli parametr nie jest zdefiniowany, archiwum listy nie będzie dostępne poprzez email. Uwaga: **tylko administratorzy mogą modyfikować ten parametr.**

Wiadomości wysyłane na listę mogą być **zaszyfrowane przy pomocy S/MIME**. Opcja '**Archiwizuj zakryptowane wiadomości jako zwykły tekst**' pozwala zdefiniować, jak takie wiadomości będą archiwizowane:

-   Opcja '**Odszyfrowane**' powoduje archiwizację wiadomości po usunięciu szyfrowania.
-   Opcja '**Oryginalne**' powoduje archiwizację wiadomości w oryginalnej zakryptowanej formie.

Opcja odnosi się zarówno do archiwum tekstowego i online-owego, a także do kompilacji wysyłanych do osób, których tryb odbierania to 'Digest'.

**UWAGA: nie zapomnij kliknąć przycisk 'Zapisz'** na dole strony, aby zatwierdzić zmiany.

### <span id="bounces"></span>Zwroty

"**Zwroty**" reprezentują **subskrybentów, których adresy email powodują błędy**, czyli osoby, które nie mogą otrzymywać wiadomości wysyłanych na listę. Przyczyn może być wiele: przestarzały adres email, adres czasowo niedostępny w czasie, gdy wiadomości były rozsyłane, przekroczona kwota skrzynki pocztowej, itp.

Sekcja '**Zarządzanie zwrotami**' definiuje dwa tryby:

-   **Tryb ostrzegania** wskazuje poziom zwracających adresów, dla których właściciel listy otrzymuje **wiadomość zatytułowaną 'Współczynnik zwrotów za wysoki'** proponując usunięcie danych subskrybentów z listy.
-   **Tryb blokowania** wskazuje poziom zwracających adresów, dla których **dystrybucja wiadomości będzie automatycznie zablokowana** do czasu rozwiązania problemu (zwykle przez usunięcie zwracających subskrybentów).

<span id="bouncers"></span>Sekcje '**Zarządzanie zwrotami, poziom pierwszy**' i '**Zarządzanie zwrotami, poziom drugi**' pozwalają przeprowadzić automatyczne operacje związane ze zwracającymi subskrybentami. Możesz zdefiniować:

-   **zakresy odpowiadające poziomom: pierwszemu i drugiemu**. Domyślnie, poziom pierwszy to współczynnik zwrotów o wartości pomiędzy 45 a 74, natomiast poziom drugi to współczynnik zwrotów o wartości pomiędzy 75 a 100;

    | Note |
    |------|
    | Współczynnik zależy od ilości, typu i częstotliwości zwrotów. Jeśli okres zwracania jest krótki lub jeśli błędów jest niedużo, współczynnik nie jest naliczany. |

-   **zadania do wykonania wobec zwracających subskrybentów**: brak, powiadomienie, usunięcie z listy;
-   **osoby do powiadamiania** w przypadku wykonania zadania: nikt, właściciele listy, administratorzy. Wysyłane powiadomienie zawiera nazwy zwracających subskrybentów i dokładne informacje o zadaniu.

**Aby zarządzać zwrotami** (zerować błędy, usuwać zwracających użytkowników, polecić przypomnienie subskrypcji, itp.), **przejdź do strony '[Zwroty](admin.md#manage_bounces)'** modułu administracyjnego listy.

**UWAGA: nie zapomnij kliknąć przycisk 'Zapisz'** na dole strony, aby zatwierdzić zmiany.

### <span id="other"></span>Różne

Opcja '**Wygasanie czasowych subskrypcji**' pozwala zdefiniować **automatyczne wygasania subskrypcji** listy: regularnie (na przykład raz w roku) subskrybenci będą otrzymywać wiadomości z prośbą o odnowienie subskrypcji. Jeśli tego nie zrobią, zostaną automatycznie wypisani z listy. Taka procedura zapewnia, że osoby zapisane na listy są faktycznie zainteresowane i zaangażowane.

Opcja '**Przypomnienia o subskrypcji**' pozwala **wysyłać regularnie przypomnienia o subskrypcji** do uczestników listy.

Opcja '**metoda ochrony adresów email**' zapewnia, że adresy email subskrybentów nie będą zbierane przez roboty w celu spamowania. Opcja dotyczy wszystkich stron listy.

Na tej stronie możesz także zobaczyć **informacje o ostatniej zmianie na liście** (kto jej dokonał i kiedy), a także **ilość zmian w konfiguracji** od powstania listy.

**UWAGA: nie zapomnij kliknąć przycisku 'Zapisz'** na dole strony, aby zatwierdzić dokonane zmiany.
