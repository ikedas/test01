~~This is a description of the reception modes available in Sympa. These options are mutually exclusive, which means that you can't set two different receive modes at the same time. Only some of the modes might be available to specific mailing lists.~~

-   Skrót (Uporządkowanie)
    Zamiast otrzymywania indywidualnych wiadomości pocztowych z listy, subskrybent otrzyma okresowo zgrupowane wiadomości w Skrócie. Ten Skrót zbiera grupę wiadomości z listy korzystając z wieloczęściowego/skróconego formatu MIME.
    Interwał wysyłania dla tych Skrótów jest zdefiniowany przez właściciela listy.
-   ProstySkrót (ProsteUporządkowanie)
    Podobne do opcji Skrótu (Digest) w tym, że subskrybent będzie okresowo otrzymywał zgrupowane wiadomości w Skrócie. Przy użyciu ProstegoSkrótu (DigestPlain) Skrót będzie wysyłany w formacie zwykłego tekstu, bez załączników. ProstySkrót jest użyteczny, jeśli twoje oprogramowanie do poczty nie wyświetla dobrze wiadomości w formacie wieloczęściowym/skróconym.
    Interwał wysyłania dla tych Skrótów jest zdefiniowany przez właściciela listy.
-   Podsumowanie
    Zamiast otrzymywać osobiste wiadomości pocztowe z listy, subskrybent będzie okresowo otrzymywał listę wiadomości. Ten tryb jest bardzo podobny do trybu Skróconego odbioru, ale subskrybent otrzymuje tylko listę wiadomości.
-   Brak poczty
    Ten tryb jest używany, gdy subskrybent nie chce już otrzymywać poczty z listy, ale chce zachować możliwość wysyłania wiadomości do listy. Ten tryb zapobiega sytuacjom, gdzie subskrybent wypisuje się z listy, a potem ponownie zapisuje.
-   Txt
    Ten tryb jest używany, gdy subskrybent chce otrzymywać wiadomości wysyłane w obu formatach HTML i zwykłego tekstu tylko w formacie HTML.
-   Html
    Ten tryb jest używany, gdy subskrybent chce otrzymywać wiadomości wysyłane w obu formatach HTML i zwykłego tekstu tylko w formacie HTML
-   Urlize
    Ten tryb jest używany, gdy subskrybent nie chce otrzymywać załączonych plików. Załączone pliki są podmieniane na adres URL kierujący do pliku zachowanego na stronie listy.
-   Not\_me
    Ten tryb jest używany, gdy subskrybent nie chce otrzymywać kopii wiadomości, które on lub ona wysłała do listy.
-   Normal
    Ta opcja jest głównie używana do anulowania trybów braku poczty, podsumowania lub paczek wiadomości (digest). Jeśli subskrybent był w trybie braku poczty, on lub ona będzie ponownie otrzymywała indywidualne wiadomości pocztowe z listy.

