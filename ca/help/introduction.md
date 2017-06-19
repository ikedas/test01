Llistes de correu: Introducció general
--------------------------------------

### Què es una llista de correu?

Una llista de correu és una **llista de distribució que permet a un grup de subscriptors rebre pel correu electrònic i de manera automàtica tots els correus que s'envien a la llista**: tots els correus que envie un subscriptor a la llista els rebran tots els altres subscriptors. Quan us subscriviu a una llista de correu, es poden enviar missatges, respondre'ls o llegir-los sense col·laborar (p.ex. «que només està a l'aguait»).

**Casos especials:**

-   De vegades es poden enviar correus a una llista de correus sense haver-se inscrit. Tot i això, cal estar-hi subscrit per a rebre els missatges.
-   De vegades no es poden enviar correus a una llista, encara que n'estigues subscrit: és el cas de les llistes d'avís, que s'empren per a transmetre informació des d'un únic remitent a un gran nombre de destinataris.

### Utilitats de les llistes de correu

La gent es subscriu a una llista de correu (a vegades abreujat com LC) per a **estar informat d'un tema concret** i per a **participar en l'intercanvi d'informació d'aquest**. Alguns exemples són:

-   una llista de correu per a tots els empleats d'una empresa;
-   una llista de correu reservada per als participants d'un projecte;
-   una llista de correu dedicada a una classe d'estudiants;
-   una llista de correu amb les últimes noticies de seguretat informàtica;
-   llista de correu d'ajuda mútua per a persones amb una afició concreta;
-   una llista de correu restringida a una familia i dedicada a l'organització de grans reunions familiars;
-   etcètera!

### Classes de llistes de correu

Hi ha **milers de llistes de correu** de tota mena en Internet: públiques o privades, grauïtes o no, amb condicions de subscripció o sense, etc. Aquestes llistes poden tenir des d'una dotzena a milers de membres.

Segons la manera en què funcionen, es pode distingir **dos tipus de llistes**:

-   **Llistes d'avís** permeten rebre missatges als subscriptors, però aquests no poden enviar-ne. De fet, aquests missatges son butlletís: revistes electròniques, serveis diaris (l'horòscop, l'informe diari del temps, alertes de securetat, etc.), notícies actualitzades d'un web, etc. Amb aquesta mena de llistes de correu, la informació només flueix d'un únic remitent a un gran nombre de destinataris.
-   **Llistes de distribució** permeten que tots els subscriptors participen en els intercanvis d'informació. Aquestes llistes poden estar o no moderades:
    -   En una **llista de distribució moderada**, els missatges es transmeten a tots els subscriptors després què hagen sigut revisats per un dels moderadors de la llista. La moderació és un signe de qualitat. Per exemple, garanteix que els subscriptors no rebran missatges fora de tema, missatges comercials que no hagen sol·licitat (correus brossa), missatges amb adjunts molt grans, etc.
    -   En una **llista de distribució no moderada**, els missatges es transmeten a tots el subscriptors, tan bon punt el robot de gestió de la llista de correu els rep.

### <span id="features"></span>Funcions

Quan estigueu subscrit a un servei de llista de correu, podreu:

-   **cercar llistes de correu** segons els vostres interessos o situació particular;
-   **gestionar les subscripcions**:
    -   [subscriure-us](user#subscribe.md) a les llistes,
    -   [donar-se de baixa](user#unsubscribe.md) de les llistes en què us heu inscrit,
    -   canviar les [opcions de subscripció](user#options.md) llista per llista,
    -   canviar les [preferències generals](user#pref.md), que afecten tot l'entorn de la llista de correu (nom, contrasenya, llengua de la interfície web de la llista de correu, etc.);
-   **emprar les llistes de correu**:
    -   llegir els [arxius del missatges en línia de les llistes a què no esteu subscrits](arc.md) se l'arxiu és públic i si els drets que teniu us permeten accedir a aquests llistes,
    -   llegir l'[arxiu de les llistes a què esteu subscrits](arc.md),
    -   realitzar [cerques en l'arxiu de la llista](arc#arcsearch.md),
    -   [enviar missatges](sendmsg.md) a les llistes que esteu subscrits,
    -   [baixar-se documents](shared#shared_read.md) de l'espai compartit de documents del web,
    -   [carregar documents](shared#shared_upload.md) en l'espai compartit de documents del web;
-   **gestionar llistes de correu**:
    -   [crear llistes noves](admin#create_list.md) (accés restringit) - s'ha d'estar autoritzat,
    -   [configurar les llistes](admin#edit_list.md) que teniu,
    -   [gestionar subscripcions](admin#manage_members.md),
    -   [gestionar l'espai web per a compartir documents](admin#manage_shared.md),
    -   [moderar les llistes](admin#moderate.md) de què sou moderador.

### <span id="roles"></span>Com funciona el servei de llistes de correu: funcions i responsabilitats

Un servei de llistes de correu té cuatre classes de funcions:

-   **administrador;**
-   **propietari;**
-   **moderador;**
-   **subscriptor.**

Es poden tenir diverses funcions al mateix temps (per exemple, es pot ser el propietari i un moderador de la llista i estar subscrit a unes altres).

#### Administradors

Els administradors s'encarrguen de **gestionar el servei de llistes de correu**. Tasques que tenen:

-   **gestionar el servidor de la llista de correu** (desplegament, manteniment, etc.);
-   **definir les indicacions generals del servei de llistes de correu**:
    -   qui tindrà permís per a demanar poder crear una llista nova,
    -   quines opcions hi haurà per gestionar les llistes (definició de l'escenari),
    -   què contindran els fitxers predeterminats (creació de plantilles),
    -   com serà la interfície web de la llista de correu
-   **definir com s'ha d'emprar el servei de llistes de correu** per als subscriptors, moderadors i propietaris i **fer-los saber les normes de funcionament**;
-   **aprovar les peticions per crear una llista de correu**;
-   **reemplaçar temporalment els propietaris de la llista** quan siga necessari; d'altra banda, se suposa que els administradors no han de fer les tasques dels moderadors.

**Els propietaris i moderadors de la llista poden dirigir-se als administradors** quand es troben un problema que no estiga resolt en la documentació o en cap comentari. Tot i això, per no inundar els administradors amb missatges, es recomana als subscriptors que es dirigisquen als propietaris de la llista.

#### Propietaris

**El propietari de la llista, normalment, és el creador** o, si no ho és el creador, és qui haja sol·licitat que es cree la llista o qui s'en haja fet responsable. **Les funcions que té són**:

-   **definir [com s'ha d'emprar la llista](admin#edit_list.md)**;
-   **escriure les [normes de funcionament de la llista](admin#charter.md)** adreçades als subscriptors;
-   **dessignar un o diversos [moderadors](listconfig#description.md)**;
-   **gestionar [les subcripcions i les baixes](admin#manage_members.md)**;
-   **decidir si és rellevant crear un [espai web per a compartir documents](admin#manage_shared.md)** disponible per als subscriptors;
-   **respondres les preguntes sobre la llista dels subscriptors i potencials subscriptors;**
-   etcetera.

Una llista pot tenir diversos propietaris. Tot i això, el **perfil «Privilegiat»** es reserva per al creador de la llista; la resta de propietaris tenen un perfli «Normal», que té menys drets.

#### Moderadors

**Els moderadors els elegeix el propietari de la llista**. **S'encarreguen de [controlar la rellevància dels missatges](admin#moderate.md)** que s'envien a la llista: després de llegir-los, **decideixen si els accepten o els rebutgen**. El procés de moderació es fa abans que els missatges no s'envien als subscriptors. Després de rebutjar un missatge es pot enviar un avís al remitent per explicar-li la causa del rebuig.

Una llista por tenir **un o diversos moderadors**; en general, el propietari de la llista també és un moderador.

Això és només per a les llistes moderades.

### <span id="policy"></span>Marc regulador

La utilització del servei de llistes de correu implica l'aceptació de unes normes:

-   ~~In most mailing list services, subscribers receive a 'List subscribers charter' on subscription. Then they are obliged to respect all the rules contained in that charter.~~
-   ~~If available, list owners and moderators have to conform to the 'Owner and moderator charter'.~~
-   ~~The use of mailing lists naturally means respecting the rules of good practices as regards to email.~~

Per saber més, cal anar a la secció dedicada a [bones pràctiques per als subscriptors](sendmsg#rulesuser.md) i la secció de [bones pràctiques per als propietaris i moderadors](admin#rulesadmin.md).

------------------------------------------------------------------------
