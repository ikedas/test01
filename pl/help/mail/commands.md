Lista poleceń interfejsu mailowego Sympy
----------------------------------------

Wszystkie polecenia należy wysyłać na adres {{conf.email}}@{{conf.host}}.

W jednej wiadomości można zawrzeć kilka poleceń. Polecenia należy umieścić w treści wiadomości (każde polecenie w osobnej linii).

### Polecenia dla użytkowników

`HELP`: pobierz listę dostępnych poleceń

`LISTS`: pobierz listę wszystkich list zainstalowanych na serwerze

`WHICH`: pobierz listę wszystkich list, na które jesteś zapisany

`CONFIRM klucz`: zatwierdź wysyłanie wiadomości (zgodnie z konfiguracją listy)

`QUIT`: zaznaczenie końca poleceń (używane do zignorowania sygnatury)

`INFO lista`: pobierz informacje o liście

`REVIEW lista`: pobierz listę subskrybentów listy

`SUBSCRIBE lista nazwa`: subskrypcja (lub potwierdzenie subskrypcji) listy

`INVITE lista email`: zaproszenie do subskrypcji listy

`UNSUBSCRIBE lista email`: wypisanie się z listy. Adres email jest wymagany tylko, jeśli chcesz wypisać inny adres niż ten, z którego wysyłasz wiadomość

`UNSUBSCRIBE * email`: wypisanie z wszystkich list, które subskrybujesz

`SET lista NOMAIL`: zawieszenie otrzymywania wiadomości z listy

`SET lista DIGEST`: ustawienie trybu otrzymywania wiadomości digest

`SET lista DIGESTPLAIN`: ustawienie trybu otrzymywania wiadomości digest (plain text)

`SET lista SUMMARY`: otrzymywanie tylko listy wiadomości

`SET lista NOTICE`: otrzymywanie tylko tematów wiadomości

`SET lista MAIL`: ustawienie zwykłego trybu otrzymywania

`SET lista CONCEAL`: ukrycie adresu subskrybenta na liście

`SET lista NOCONCEAL`: udostępnienie adresu subskrybenta na liście

`INDEX lista`: otrzymanie listy plików archiwum

`GET lista plik`: otrzymanie pliku archiwum listy

`LAST lista`: otrzymanie najnowszych wiadomości z listy

### Polecenia dla właścicieli list

`ADD lista email nazwa`: dodanie osoby do listy

`DEL lista email`: usunięcie subskrybenta z listy

`STATS lista`: sprawdzenie statystyk listy

`REMIND lista`: wysłanie do wszystkich subskrybentów spersonalizowanej wiadomości przypominającej z adresem, którym dana osoba subskrybuje listę

### Polecenia dla właścicieli list

`DISTRIBUTE lista klucz`: zatwierdzenie wiadomości

`REJECT lista klucz`: odrzucenie moderowanej wiadomości

`MODINDEX lista`: sprawdzenie listy wiadomości do moderacji
