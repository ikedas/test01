### Preguntes freqüents dels usuaris

#### No puc sucriure'm a una llista

Aquest problema pot ser conseqüència de les raons següents:

-   **Els propietaris de la llista han oblidat processar la vostra petició de subscripció**: d'homes és errar, i potser que la vostra petició s'haja perdut entre molts altres missatges. Torna a enviar una petició abans de [contactar directament amb els propietaris de la llista](#contactadmin).
-   **La subscripció a la llista está reservada a un tipus determinat de persones**. Per a saber més, [contacteu els propietaris de la llista](#contactadmin).

#### No puc iniciar sessió en la interfície web de la llista de correu

Aquest problema pot ser conseqüència de les raons següents:

-   ~~**You have no password**. To be given a password, follow the [First login?](%7B%7Bpath_cgi%7D%7D/firstpasswd) link from the homepage. You will receive your new password by email.~~
-   **Heu picat una contrasenya incorrecta**. Si heu oblidat la contrasenya, podeu reestablir la contrasenya. Per a fer-ho, aneu a la pàgina principal i seguiu l'enllaç [Contrasenya perduda?](%7B%7Bpath_cgi%7D%7D/renewpasswd).
-   **No heu emprat el nom d'usuari correcte** (l'adreça amb que us heu subscrit a la llista).

| Note |
|------|
| Per a evitar errors en escriure la contrasenya, podeu escriure-la en una altra aplicació (com el client de correu electrònic) i copiar-la i enganxar-la en el navegador web. |

#### No rebeu (tots) els missatges enviats a una llista

Aquest problema pot tenir moltes causes:

-   <span id="notsubscribedyet"></span>**Mai heu estat subscrits a la llista**:
    -   Potser us vau equivocar en l'adreça de correu quan vau intentar subscriure-us.
    -   Potser us vau subscriure amb una adreça diferent de la que esteu comprovant.
    -   Potser que la vostra petició de subscripció haja estat rebutjada pels propietaris de la llista.

    En qualsevol cas, intenteu [subscriure-us-hi](user#subscribe.md) una altre cop.
-   <span id="notsubscribedanymore"></span>**Ya no estic subscrit a la llista**:
    -   Si la vostra adreça ha causat retornats durant un temps, potser el sistema (o fins i tot el propietari) us haja donat de baixa automàticament. Intenteu [subscriure-us una altre cop](user#subscribe.md) desprès que us hageu assegurat que l'adreça de correu no donarà problemes més endavant.
    -   Si no heu respectat les diferents normes de la llista de correu, els propietaris us poden haver «expulsat»...
    -   Potser algun malintencionat us haja donat de baixa arbitràriament, en cas que la llista no estiga configurada per a rebre una confirmació de petició de subscripció o de donada de baixa... En aquest cas, intenteu [subscriure-us](user#subscribe.md) un altre cop.
-   **La [modalitat d'entrega](user#deliverymode.md) no us permet rebre missatges**: per exemple, en la modalitat d'entrega «Nomail».
-   **Teniu la safata d'entrada plena**. Atenció: quan no teniu la safata d'entrada completament plena, només rebeu els missatges petits, fet que dificulta saber quin és el problema... A més a més, si l'adreça de correu normalment causa problemes, els propietaris o el sistema us poden donar de baixa. De manera que cal que netejeu la safata d'entrada amb regularitat.
-   **La safata d'entrada té algunes restriccions**: no us permet rebre missatges amb adjunts, rebutja alguns tipus d'adjunts o limita la mida màxima dels missatges d'entrada; en aquest cas, cal que elegiu la [modalitat d'entrega urlize](user#deliverymode.md).

#### No puc enviar missatges a la llista

Aquest problema pot tenir moltes causes:

-   **[Mai no us havieu subscrit](#notsubscribedyet)** a la llista.
-   **[Ja no esteu subscrits a la llista](#notsubscribedanymore)**.
-   **Esteu emprant una adreça diferent** de què us vau subscriure a la llista.
-   **Si la llista està moderada, la distribució del missatge depèn de la disponibilitat del moderador**: no poden estar pendents de la llista nit i dia! De manera que la distribució de la llista es pot endarrerir un poc.
-   **Si la llista està moderada, el moderador pot haver rebutjar el missatge**. Si no rebeu un avís, podeu enviar un missatge a nomdelallista-request@{{conf.host}} per a demanar una explicació.
-   **El missatge que intenteu enviar no compleix les condicions per què es distribueixi** en la llista: pot ser massa gran, que continga algún adjunt prohibit o fins i tot qualsevol mena d'adjunt (en cas que els adjunts estiguen prohibits en la llista).
-   **El problema també el pot causar el vostre compte de correu**:
    -   El servidor de correu està temporalment inaccessible.
    -   Teniu la safata d'entrada plena i no us deixa envia rmissatges nous.
    -   La safata d'entrada té algunes restriccions: no us permet enviar missatges amb adjunt, no permet alguns tipus d'adjunts o límita la grandària màxima dels missatges de sortida.
-   Per acabar, **pot ser us hageu equivocat en la direcció de la llista** en enviar el missatge!

#### No em puc donar de baixa de la llista

Aquest problema pot tenir moltes causes:

-   **Esteu emprant una adreça diferent** de què us vau subscriure a la llista.
-   **Us heu subscrit a través d'una font de dades dinàmica** (exemples: bases de dades, directoris LDAP, etc.) que no permeten donar-se de baixa. [Contacteu amb els propietaris de la llista](#contactadmin)per a saber-ne més.
-   **Els propietaris de la llista han oblidat processar la vostra petició de donada de baixa**: errar és humà, i potser la vostra petició s'ha perdut entre altres missatges. Torneu a enviar la petició abans de [contactar directament els propietaris de la llista](#contactadmin).

#### <span id="contactadmin"></span>Vull contactar amb els propietaris de la llista

Els noms dels propietaris i moderadors apareixen en el menú de l'esquerra. No obstant això, no heu d'escriure mai directament al propietari o moderador de la llista: primer de tot, la persona a qui esciviu potser no estiga, i a més a més, és millor informar a tots els propietaris i moderadors de la vostra petició. Quan tingueu un dubte o suggerencia, **heu d'escriure a l'adreça: nomdelallista-request@{{conf.host}}** (canvieu «nomdelallista» pel nom de la llista).
