Listy mailingowe - Wprowadzenie
-------------------------------

### Co to jest lista mailingowa?

Lista mailingowa to **lista dystrybucyjna, dzięki której grupa subskrybentów automatycznie otrzymuje wszystkie wiadomości wysyłane na adres listy**: każda wiadomość wysłana przez subskrybenta na adres listy jest dostarczana pozostałym subskrybentom. Subskrybenci listy mogą wysyłać wiadomości na jej adres, odpowiadać na wiadomości lub tylko je czytać.

**Przypadki szczególne:**

-   Czasem osoby nie będące subskrybentami listy także mogą wysyłać na nią wiadomości. Aby jednak otrzymywać wiadomości z listy, trzeba być jej subskrybentem.
-   Czasem nawet subskrybenci listy nie mogą wysyłać na nią wiadomości. Dotyczy to list dystrybucyjnych, które są używane jedynie do rozsyłania wiadomości pochodzących od konkretnych nadawców do większej grupy odbiorców.

### Zastosowanie list mailingowych

Ludzie zapisują się na listy mailingowe, aby **otrzymywać wiadomości związane z konkretnymi tematami** i **uczestniczyć w wymianie informacji**. Oto kilka przykładów:

-   lista mailingowa dla wszystkich pracowników firmy;
-   lista mailingowa uczestników projektu;
-   lista mailingowa studentów uczestniczących w danych zajęciach;
-   lista mailingowa na temat nowości związanych z bezpieczeństwem w IT;
-   lista mailingowa na temat wzajemnej pomocy w drobnych pracach domowych;
-   lista mailingowa rodziny wspomagająca organizowanie dużych spotkań rodzinnych;
-   i tak dalej!

### Rodzaje list mailingowych:

W internecie istnieją **tysiące list mailingowych** różnego rodzaju: publiczne i prywatne, darmowe i płatne, z subskrypcją otwartą i warunkową, itd. Listy mogą mieć od kilku do kilku tysięcy uczestników.

W zależności od sposobu działania, listy mailingowe można podzielić na **dwa rodzaje**:

-   **Listy dystrybucyjne** dostarczają wiadomości do subskrybentów, ale nie pozwalają im wysyłać wiadomości. Takie wiadomości to newslettery: magazyny w formie elektronicznej, różne usługi (horoskopy, raporty pogodowe, itp.), informacje o zmianach na stronach internetowych, itd. W przypadku takiej listy, wiadomości rozsyłane są przez konkretnych nadawców do większej grupy odbiorców.
-   **Listy dyskusyjne**, gdzie wszyscy subskrybenci biorą udział w wymianie wiadomości. Takie listy mogą być moderowane lub nie:
    -   W przypadku **moderowanych list dyskusyjnych** wiadomości są rozsyłane do subskrybentów po zaakceptowaniu przez moderatorów. Moderacja jest środkiem zapewniania jakości wiadomości: zabezpiecza przez rozsyłaniem wiadomości niezwiązanych z tematem listy, spamu, wiadomości z dużymi załącznikami, itp.
    -   W przypadku **niemoderowanej listy dyskusyjnej** wiadomości są rozsyłane do wszystkich subskrybentów natychmiast po otrzymaniu ich przez serwer.

### <span id="features"></span>Funkcje

Jako subskrybent listy, możesz:

-   **wyszukiwać listy mailingowe** związane z Twoimi zainteresowaniami albo konkretną sytuacją;
-   **zarządzać swoimi subskrypcjami**:
    -   [subskrybować](user#subscribe.md) listy,
    -   [wypisywać się](user#unsubscribe.md) z list, które subskrybujesz,
    -   zmieniać [opcje subskrybenta](user#options.md) dla poszczególnych list,
    -   zmieniać [ogólne preferencje](user#pref.md), które dotyczą całego środowiska list mailingowych (nazwę, hasło, język interfejsu webowego, itp.);
-   **korzystać z list mailingowych**:
    -   przeglądać [archiwa wiadomości list, których nie subskrybujesz](arc.md), jeśli archiwa są publiczne i masz prawa do ich odczytu,
    -   przeglądać [archiwa list, które subskrybujesz](arc.md),
    -   [przeszukiwać archiwa](arc#arcsearch.md),
    -   [wysyłać wiadomości](sendmsg.md) na listy, które subskrybujesz,
    -   [pobierać dokumenty](shared#shared_read.md) z przestrzeni dokumentów współdzielonych,
    -   [dodawać dokumenty](shared#shared_upload.md) do przestrzeni dokumentów współdzielonych;
-   **zarządzać listami mailingowymi**:
    -   [tworzyć nowe listy](admin#create_list.md) (ograniczony dostęp) - podlega autoryzacji,
    -   [konfigurować swoje listy](admin#edit_list.md),
    -   [zarządzać subskrypcjami](admin#manage_members.md),
    -   [zarządzać przestrzenią dokumentów współdzielonych](admin#manage_shared.md),
    -   [moderować listy](admin#moderate.md), których jesteś moderatorem.

### <span id="roles"></span>Jak funkcjonuje usługa list mailingowych: role i odpowiedzialność

Z usługą list mailingowych związane są cztery typy ról:

-   **administrator;**
-   **właściciel;**
-   ~~**moderator;**~~
-   **subskrybent.**

Jedna osoba może mieć przypisanych wiele ról (na przykład można być właścicielem i moderatorem listy, a także subskrybentem kilku innych).

#### Administratorzy

Administratorzy zajmują się **zarządzaniem usługą list mailingowych**. Ich obowiązki to:

-   **zarządzanie serwerem list mailingowych** (wdrażanie, obsługa, itp.);
-   **określenie ogólnych zasad dla danej usługi list mailingowych**:
    -   kto może prosić o utworzenie nowej listy,
    -   które opcje zarządzania listami będą dostępne (definicje scenariuszy),
    -   co powinny zawierać domyślne pliki (stworzenie szablonów),
    -   jak będzie wyglądać interfejs webowy;
-   **określenie sposobu używania usługi list mailingowych** i **udokumentowanie tych zasad przez stworzenie statutów** na potrzeby subskrybentów, moderatorów i właścicieli;
-   **zatwierdzanie próśb o utworzenie listy**;
-   **tymczasowe zastępowanie właścicieli list** w razie potrzeby; z drugiej jednak strony, administratorzy nie powinni wykonywać obowiązków moderatorów.

**Właściciele list i moderatorzy mogą zwrócić się do administratorów**, gdy natrafiają na nieudokumentowane problemy i po wszelkie wskazówki. Aby ograniczyć ilość wiadomości wysyłanych do administratorów, subskrybenci powinni zwracać się z problemami raczej do właścicieli list.

#### Właściciele

**Właściciel listy to jej twórca** lub osoba, która poprosiła o utworzenie listy lub stała się za nią odpowiedzialna. **Rola właściciela**:

-   **określenie [sposobu korzystania z listy](admin#edit_list.md)**;
-   **napisanie [statutu listy](admin#charter.md)** przeznaczonego dla subskrybentów;
-   **wskazanie jednego lub kilku [moderatorów](listconfig#description.md)**;
-   **zarządzanie [subskrypcjami](admin#manage_members.md)**;
-   **decyzja, czy udostępnić subskrybentom [przestrzeń dokumentów współdzielonych](admin#manage_shared.md)**;
-   **odpowiadanie na pytania subskrybentów i potencjalnych subskrybentów dotyczące listy;**
-   itd.

Lista może mieć kilku właścicieli. Jednak **'uprzywilejowany' profil** zarezerwowany jest dla twórcy listy, inni właściciele mają profile 'zwykłe', z mniejszymi przywilejami.

#### Moderatorzy

**Moderatorzy są wskazywani przez właściciela listy**. Ich rolą jest **[kontrola wiadomości](admin#moderate.md)** wysyłanych na listę: moderator po zapoznaniu się z wiadomością **akceptuje ją lub odrzuca**. Moderacja ma miejsce zanim wiadomość zostanie rozesłana do subskrybentów. Odrzucenie wiadomości z reguły skutkuje wysłaniem do nadawcy powiadomienia z wyjaśnieniem powodów odrzucenia.

Lista może mieć **jednego lub kilku moderatorów**; właściciel listy jest także moderatorem.

To dotyczy tylko moderowanych list.

### <span id="policy"></span>System regulacyjny

Używając usługi list mailingowych należy przestrzegać pewnych reguł:

-   ~~In most mailing list services, subscribers receive a 'List subscribers charter' on subscription. Then they are obliged to respect all the rules contained in that charter.~~
-   ~~If available, list owners and moderators have to conform to the 'Owner and moderator charter'.~~
-   ~~The use of mailing lists naturally means respecting the rules of good practices as regards to email.~~

Aby dowiedzieć się więcej, zapoznaj się z rozdziałami opisującymi [dobre praktyki dla subskrybentów](sendmsg#rulesuser.md) i [dobre praktyki dla właścicieli i moderatorów](admin#rulesadmin.md).

------------------------------------------------------------------------
