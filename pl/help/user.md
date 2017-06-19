Listy mailingowe - Podręcznik użytkownika
-----------------------------------------

### <span id="howitworks"></span>Jak działa lista mailingowa

Usługa list mailingowych jest obsługiwana przez **oprogramowanie Sympa**. Częścią Sympy jest **środowisko webowe**.

**Istnieją dwa sposoby wykonywania operacji związanych z listami mailingowymi** (zapisywania się, zmiany preferencji, itp.):

-   **po zalogowaniu do środowiska webowego**;
-   **wysyłając polecenia w wiadomościach email** do zarządcy list mailingowych na adres **{{conf.email}}@{{conf.host}}**.

**Aby wysłać polecenie do Sympy**, należy wykonać następujące czynności:

-   **Jeśli wysyłane jest pojedyncze polecenie**, powinno znaleźć się w temacie wiadomości email, a treść wiadomości powinna pozostać pusta.
-   **Jeśli wysyłanych jest kilka poleceń**, temat wiadomości email powinien pozostać pusty, a polecenia powinny znaleźć się w treści wiadomości. Sympa nie przetworzy poleceń, jeśli nie zastosujesz się do następujących zasad:
    -   Każde polecenie powinno znaleźć się w osobnej linii.
    -   Wiadomość email powinna być wysyłana jako plain text, nie jako HTML.
    -   Wiadomość nie może zawierać nic oprócz poleceń dla Sympy (brak sygnatury).

Opis wszystkich poleceń, które mogą być wysyłane do Sympy, można znaleźć tutaj: [file:///help/mail\_commands](mail_commands.md).

### <span id="subscribe"></span>Subskrybowanie list mailingowych

Zapisywanie się na listę mailingową jest bardzo łatwe:

1.  **Wybierz adres email**, który chcesz dodać do listy subskrybentów.

    | Note |
    |------|
    | Lepiej wybrać adres, którego często używasz, i na którym masz dużo wolnego miejsca: niektóre listy przesyłają wiele wiadomości, które czasami zawierają spore załączniki. |

    | Note |
    |------|
    | Oczywiście możesz subskrybować listę za pośrednictwem kilku adresów email. W takim wypadku cały proces subskrypcji trzeba wykonać dla każdego adresu z osobna. |

2.  Wyślij **wiadomość na adres {{conf.email}}@{{conf.host}}** z adresu, którego chcesz użyć do subskrypcji.

    | Note |
    |------|
    | Sympa to nie osoba, tylko serwer zarządzający listami mailingowymi. Dlatego wysyłanie pozdrowień nie ma sensu! ;-) |

3.  W temacie wiadomości wpisz: **subscribe nazwalisty Imię Nazwisko** (zamiast 'nazwalisty' podaj nazwę listy, którą chcesz subskrybować i wpisz swoje imię i nazwisko).
4.  **Treść wiadomości pozostaw pustą**.

    | Note |
    |------|
    | Aby zaoszczędzić czas, w jednej wiadomości można przesyłać kilka komend. Więcej informacji na ten temat znajduje się w sekcji [Jak działa lista mailingowa](#howitworks). |

**Po wykonaniu powyższych kroków otrzymasz wiadomość z informacją, czy Twoja prośba zostały zaakceptowana**: jeśli subskrybowanie listy wymaga zatwierdzenia, właściciel może zdecydować o odrzuceniu prośby. Jeśli tak się stanie, nie wysyłaj kolejnych próśb: wynik będzie taki sam. Możesz w takiej sytuacji wysłać wiadomość bezpośrednio do właściciela listy (nazwalisty-request@{{conf.host}}) z wyjaśnieniem, dlaczego chcesz subskrybować listę...

| Note |
|------|
| Uwaga: czasem prośba o subskrypcję wymaga Twojego zatwierdzenia zanim zostanie przetworzona. W takim przypadku postępuj zgodnie z instrukcjami zawartymi w otrzymanej wiadomości. |

W zależności od typu listy (lista z subskrypcją wymagającą zatwierdzenia lub otwartą) i dostępności właściciela listy, **wiadomość z informacjami może nie nadejść natychmiast**. Nie ma jednak potrzeby wysyłania kilku próśb o subskrypcję.

**Jeśli Twoja prośba zostanie zaakceptowana, otrzymasz wiadomość potwierdzającą subskrypcję. Wiadomość powitalna** (statut listy) **zawiera kilka istotnych informacji:**

-   Twoje **hasło do listy**. Hasło jest takie samo dla wszystkich list, które subskrybujesz przy użyciu danego adresu email. Możesz [zmienić je](#global_pref "How to change your password") po zalogowaniu się do środowiska list mailingowych;
-   **szczegółowe informacje na temat listy**: jej cel, gdzie można znaleźć jej archiwa, itp.
-   **zasady korzystania z listy**: dozwolone i zabronione tematy, netykieta, informacje prawne, ochrona prywatności, itp.

**Powinieneś zachować otrzymane potwierdzenie subskrypcji**: możesz jej potrzebować w przyszłości, aby sprawdzić swoje hasło albo wysłać polecenie do Sympy (na przykład wypisać się z listy). Ogólnie, **radzimy zachowywać wszystkie informacje o subskrypcjach list mailingowych**.

**Listę można subskrybować także za pomocą interfejsu webowego**. Aby to zrobić, wykonaj następujące czynności:

1.  Przejdź do **[strony startowej](%7B%7Bpath_cgi%7D%7D/home)** środowiska list mailingowych i zaloguj się.
2.  **Przejdź do strony informacyjnej listy**, którą chcesz subskrybować.
3.  W lewym menu **kliknij link 'Subskrybuj'**.

### <span id="sympa_auth"></span>Logowanie do środowiska list mailingowych

Aby zalogować się do środowiska list mailingowych, skorzystaj z formularza uwierzytelniania, który znajduje się na górze w lewej kolumnie interfejsu. Jeśli jesteś zalogowany, w miejscu formularza wyświetla się adres email i profil (subskrybent, moderator lub właściciel).

Proces uwierzytelniania różni się w zależności od Twojej sytuacji:

-   **Jeśli usługa list mailingowych używa technologii pojedynczego logowania** (jednoznaczne konta i uwierzytelnianie, na przykład za pośrednictwem systemu CAS), najprawdopodobniej powinieneś logować się właśnie w ten sposób. Aby to zrobić, kliknij przycisk 'Przejdź' znajdujący się obok napisu '**Logowanie \[nazwa systemu\]**'. Następnie wpisz swój login i hasło, aby zalogować się w systemie uwierzytelniania.

    | Note |
    |------|
    | Jeśli zalogowałeś się wcześniej do innej usługi przy użyciu zewnętrznego systemu uwierzytelniania, nie potrzebujesz logować się ponownie. Jeśli to konieczne, odśwież stronę. |

-   **Jeśli pojedyncze logowanie Ciebie nie dotyczy, użyj swojego hasła związanego z listami**. W takim przypadku zaloguj się tradycyjną metodą: wprowadź w formularzu adres email, którym subskrybujesz listę jako login i hasło.

    | Note |
    |------|
    | Jeśli nie pamiętasz swojego hasła, kliknij link 'Zapomniałeś hasła?'. Po podaniu adresu email otrzymasz wiadomość z URL-em walidującym. |

-   **Jeśli pojedyncze logowanie Ciebie nie dotyczy i nie masz jeszcze hasła do list**, kliknij przycisk '**Pierwsze logowanie?**' i wpisz swój adres email. Otrzymasz wiadomość zawierającą URL do strony, na której będziesz mógł ustawić swoje hasło.

| Note |
|------|
| Pamiętaj: hasło związane z listami to specjalne hasło, które odnosi się tylko do usługi list mailingowych. |

### Zarządzanie subskrypcjami

Aby zobaczyć wszystkie listy, które subskrybujesz, najpierw musisz się [zalogować](#sympa_auth). Po zalogowaniu lista wszystkich Twoich list, wraz z krótkim opisem każdej z nich, zostanie wyświetlona w formularzu 'Twoje listy' w lewej kolumnie.

**Aby zobaczyć stronę informacyjną danej listy, kliknij jej nazwę**. Strona informacyjna zawiera opis listy (jej temat, reguły dotyczące wysyłania wiadomości, itp.) o różnej długości w zależności od listy.

Na stronie informacyjnej możesz:

-   zmienić [opcje subskrybenta](#options);
-   czytać [archiwa listy](arc.md);
-   [przeszukiwać archiwa wiadomości](arc.md#arcsearch);
-   [wysyłać nowe wiadomości](sendmsg.md);
-   [pobierać dokumenty](shared.md#shared_read) z przestrzeni dokumentów współdzielonych;
-   [dodawać dokumenty](shared.md#shared_upload) do przestrzeni dokumentów współdzielonych;
-   [przeglądać uczestników](#subscribers) listy (jeśli funkcja jest dostępna);
-   ~~[suspend or resume](suspend.md) your subscription of each list;~~
-   [wypisać się](#unsubscribe) z listy.

<span id="subscribers"></span>W **lewym menu** wyświetlana jest **ilość subskrybentów listy**. **Aby przejrzeć subskrybentów listy, kliknij link 'Przejrzyj subskrybentów'**, znajdujący się w lewym menu (jeśli właściciel listy zdecydował się wyłączyć tę funkcję, link jest niedostępny). Lista subskrybentów pokazuje **adres email** i **nazwę** każdego z nich (znaczenie nazwy zależy od użytej metody subskrypcji).

| Note |
|------|
| Domyślnie każda strona wyświetla 25 subskrybentów. Można nawigować pomiędzy stronami przy użyciu strzałek lub wyświetlić więcej wpisów na stronie. Klikając na nagłówek odpowiedniej kolumny można sortować listę subskrybentów na podstawie adresu email, domeny lub nazwy. |

**Właściciele i moderatorzy listy są wyświetlani w lewym menu**. Nie powinno się pisać wiadomości bezpośrednio do właściciela listy lub moderatora. Jeśli chcesz zadać pytanie lub coś skomentować, powinieneś użyć następującego adresu: **nazwalisty-request@{{conf.host}}** (zamień 'nazwalisty' na nazwę listy, której dotyczyć ma wiadomość).

Aby sprawdzić, **kiedy zasubskrybowałeś listę** lub **kiedy ostatnio edytowałeś opcje subskrypcji**, **kliknij link 'Opcje subskrybenta'** w lewym menu.

### <span id="pref"></span>Zarządzanie preferencjami

Aby **korzystanie z listy było wygodne**, **możesz zdefiniować kilka osobistych preferencji**. Są dwa rodzaje preferencji, które możesz zmieniać:

-   **opcje subskrybenta**, które różnią się w zależności od listy;
-   **ogólne preferencje**, które odnoszą się do całego środowiska list mailingowych Sympa.

#### <span id="options"></span>Zmiana opcji subskrybenta

**Twoje opcje subskrypcji mogą różnić się w zależności od listy mailingowej**. Aby je zmienić, wykonaj następujące kroki:

1.  Przejdź do **[strony startowej](%7B%7Bpath_cgi%7D%7D/home)** środowiska list mailingowych i zaloguj się.
2.  **Przejdź do strony informacyjnej listy**, dla której chcesz zmienić opcje subskrypcji.
3.  W lewym menu, **kliknij link 'Opcje subskrybenta'**.
4.  <span id="deliverymode"></span>**Wybierz tryb dostarczania wiadomości** (opcje się wzajemnie wykluczają, więc można wybrać tylko jedną):
    -   **format digest MIME**: zamiast otrzymywać wiadomości z listy w zwykły sposób, będziesz dostawać regularnie wiadomość zbiorczą. Wiadomość zbiorcza składa się z pewnej ilości wiadomości z listy, przy użyciu formatu multipart/digest MIME. Częstotliwość wysyłania wiadomości zbiorczej ustala właściciel listy.
    -   **format digest plain text**: zamiast otrzymywać wiadomości z listy w zwykły sposób, będziesz dostawać regularnie wiadomość zbiorczą. Wiadomość zbiorcza składa się z pewnej ilości wiadomości z listy, przy użyciu formatu plain text. Częstotliwość wysyłania wiadomości zbiorczej ustala właściciel listy.
    -   **tryb podsumowania**: zamiast otrzymywać wiadomości z listy w zwykły sposób, będziesz dostawać regularnie spis wiadomości. Aby przeczytać ich treść, będziesz musiał przeglądać archiwum listy online.
    -   **tryb powiadamiania**: przy takim ustawieniu, będziesz dostawać wiadomości bez treści: w ten sposób otrzymujesz natychmiast informacje o każdej wiadomości wysłanej na listę, bez ryzyka przepełnienia skrzynki pocztowej.
    -   **brak wiadomości (przydatne na wyjazdach)**: tryb umożliwia przerwy w otrzymywaniu wiadomości z listy. Może być przydatny w sytuacjach, gdy przez dłuższy czas nie masz dostępu do swojej skrzynki pocztowej, ale chcesz nadal być zapisany na listę.
    -   **tryb tekstowy**: tryb pozwala na otrzymywanie wiadomości tylko w formacie tekstowym (text/plain), jeśli są wysyłane zarówno w formacie tekstowym jak i HTML.
    -   **tryb HTML**: tryb pozwala na otrzymywanie wiadomości tylko w formacie HTML, jeśli są wysyłane zarówno w formacie tekstowym jak i HTML
    -   **tryb url**: tryb pozwala na pomijanie załączników w otrzymywanych wiadomościach. Załączniki będą dostępne poprzez archiwum listy, i można do nich dotrzeć za pośrednictwem adresów URL przesyłanych w wiadomościach.
    -   **nie dostajesz swoich wiadomości**: tryb pozwala na nie otrzymywanie kopii swoich własnych wiadomości.
    -   **standardowy (odbiór bezpośredni)**: tryb domyślny, usuwa wszelkie inne ustawienia trybu odbierania.
    -   **zawieszony**: tryb pozwala zawiesić subskrypcję na określony okres czasu lub bezterminowo. W przeciwieństwie do wypisania się z listy, tryb pozwala na zarządzanie swoją subskrypcją i łatwe odnowienie jej w każdym momencie przy użyciu sekcji "Zarządzaj subskrypcjami".
5.  **Wybierz opcje widoczności**:
    -   **wyświetlanie na stronie listy**: Twoja nazwa i adres email będą widoczne na liście uczestników listy (jeśli właściciel listy zezwala subskrybentom na przeglądanie listy uczestników).
    -   **ukryty**: Twoja nazwa i adres email nie będą wyświetlane na liście uczestników listy. Twój adres email będzie jednak widoczny w archiwach listy, jeśli wysyłasz jakieś wiadomości.
6.  **Kliknij przycisk 'Aktualizuj'**.

#### <span id="global_pref"></span>Zmiana globalnych preferencji

Globalne preferencje odnoszą się do wszystkich Twoich subskrypcji i do interfejsu list mailingowych. Aby zmienić preferencje, wykonaj następujące kroki:

1.  Przejdź do **[strony startowej](%7B%7Bpath_cgi%7D%7D/home)** środowiska list mailingowych i zaloguj się.
2.  W formularzu wyświetlonym na górze lewej kolumny **kliknij link 'Twoje preferencje'**.
3.  **Dokonaj zmian w preferencjach**.
4.  **Kliknij przycisk 'Zastosuj' dla każdej opcji**, którą zmieniasz.

Możesz zmienić:

-   swoją **nazwę**; jeśli zapisałeś się na listę za pomocą interfejsu webowego, nazwa automatycznie uaktualni się na liście uczestników listy;
-   **język interfejsu webowego Sympy** (język można zmieniać na każdej stronie interfejsu webowego; Twoja zmiana zostanie zachowana mimo zmiany języka na stronie innej niż strona 'Preferencje');
-   **czas życia ciasteczka zachowywanego na Twoim komputerze przez Sympę** ('Connection expiration period', czas wygaśnięcia połączenia). Domyślnie sesja wygasa w momencie zamknięcia przeglądarki; jeśli jednak często używasz usługi list mailingowych, radzimy ustawić dłuższy czas trwania sesji;

    | Note |
    |------|
    | Ciasteczko to mały plik, który serwer webowy przechowuje na Twoim twardym dysku, zwykle tymczasowo, po to abyś był rozpoznawany przez jego usługi. Ciasteczko zawiera kilka informacji na Twój temat: nazwę, adres email, czas ostatniego logowania, itp. |

-   **adres email, którego używasz do subskrypcji list** (jeśli używasz wielu adresów email, zmieniony zostanie adres, z którego jesteś zalogowany);

    | Note |
    |------|
    | Uwaga: zmiana tej opcji spowoduje zmianę Twoich subskrypcje na wszystkich listach. Jeśli chcesz zmienić adres na jednej liście, lepiej wypisz się z niej i zapisz ponownie z dobrym adresem. |

-   Twoje **hasło do list**.

Sekcja '**Twoje pozostałe adresy email**' służy do zmiany adresu email.

### Wyszukiwanie listy mailingowej

Czasem potrzebujesz znaleźć konkretną listę mailingową. Są trzy możliwości:

-   **przeglądać kategorie list** wyświetlone na [stronie domowej środowiska list mailingowych](%7B%7Bpath_cgi%7D%7D/home);
-   wyszukać listę za pomocą **formularza wyszukiwania**: formularz zwróci wszystkie listy, których nazwa lub opis pasuje do podanego wyrazu (opis listy zwykle zawiera krótkie zdanie);
-   kliknąć zakładkę '[Spis list](%7B%7Bpath_cgi%7D%7D/lists)' na górze strony, aby wyświetlić wszystkie dostępne listy.

| Note |
|------|
| W zależności od domeny Twojego adresu email (przykład: *cru.fr*, *fai.com*, etc.) i miejsca skąd się logujesz, prawa dostępu do list mogą się różnić. Możesz zapisać się na listę, która nie jest wyświetlana, jeśli znasz jej nazwę. Aby to zrobić, [skorzystaj z klienta pocztowego](#subscribe). |

### <span id="archives"></span>Czytanie archiwum listy online

Przejdź do [**dokumentacji na temat archiwów**](arc.md).

### <span id="sendmsg"></span>Wysyłanie wiadomości

Przejdź do [**dokumentacji na temat wysyłania wiadomości**](sendmsg.md).

### <span id="shared"></span>Korzystanie z przestrzeni dokumentów współdzielonych

Przejdź do [**dokumentacji na temat przestrzeni dokumentów współdzielonych**](shared.md).

### <span id="suspend"></span>~~Suspending or resuming your subscription of each list~~

~~Please refer to the [**subscription management documentation**](suspend.md).~~

### <span id="unsubscribe"></span>Wypisywanie się z list

Aby wypisać się z listy, wykonaj następujące kroki:

1.  Wyślij **wiadomość na adres {{conf.email}}@{{conf.host}}**. z adresu, którym subskrybujesz listę.
2.  W temacie wiadomości wpisz: **unsubscribe nazwalisty** (zamień 'nazwalisty' na nazwę listy, z której chcesz się wypisać).
3.  **Treść wiadomości pozostaw pustą**.

    | Note |
    |------|
    | Aby zaoszczędzić czas, w jednej wiadomości można przesyłać kilka komend. Więcej informacji na ten temat znajduje się w sekcji [Jak działa lista mailingowa](#howitworks). |

Możesz także wypisać się z listy za pomocą interfejsu webowego (trzeba powtarzać operację dla każdej listy, z której chcesz się wypisać):

1.  Przejdź do **[strony startowej](%7B%7Bpath_cgi%7D%7D/home)** środowiska list mailingowych i zaloguj się.
2.  **Przejdź do strony informacyjnej listy**, z której chcesz się wypisać.
3.  **W lewym menu, kliknij link 'Wypisz się z listy'**.

------------------------------------------------------------------------
