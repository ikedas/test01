<span id="docadmin"></span>Llistes de correu - Guia per a propietaris i moderadors
----------------------------------------------------------------------------------

### Introducció: qui és l'encarregat de gestionar les llistes de correu?

Recordatori: un servei de llistes de correu té cuatre tipus de càrrecs:

-   **administrador;**
-   **propietari;**
-   **moderador;**
-   **subscriptor.**

Aneu a [descripció de cada càrrec](introduction#roles.md) per a saber-ne més.

### <span id="create_list"></span>Com sol·licitar la creació de una llista de correu

La **sol·licitud de creació d'una llista** pot estar **subjecte a condicions**. Tot i que compliu aquestes condicions, la **creació de la llista** estarà **dependrà de l'aprovació dels administradors**.

Per a sol·licitar la creació d'una llista de correu, seguiu els passos següents:

1.  Aneu a la **[pàgina d'inici de l'entorn de la llista](%7B%7Bpath_cgi%7D%7D/home)** i [**inicieu sessió**](user#sympa_auth.md).
2.  En el menú de dalt, **feu clic en l'enllaç «Crea una llista»**.

    | Note |
    |------|
    | Si no podeu accedir a l'enllaç, significa que no teniu els privilegis necessaris per a crear una llista. |

3.  Poseu un **nom** a la llista (només poseu el nom, sense l'«@» i el nom del domini; per exemple: *llengues\_catala* i no *llengues\_catala@{{conf.host}}*).

    | Note |
    |------|
    | No empreu espais, accents o qualsevol caràcter especial en els noms de les llistes: aquests caràcters poden causar problemes. |

    | Note |
    |------|
    | Elegiu un nom explícit però curt: penseu en els subscriptors que hauran d'escriure el nom cada vegada que envien un missatge a la llista! Si gestioneu un grup de llistes, podeu posar-les un prefix comú; de manera que apareixeran totes juntes i es reconeixeran fàcilment (exemple: *xx-users@{{conf.host}}, xx-hotline@{{conf.host}}*, etc.). |

4.  Elegiu un **tipus de llista** entre els tipus que n'hi ha predefinits (les que ja estan predefinides solament són exemples de configuracions clàssiques que el propietari pot canviar, una vegada que s'haja creat; fins i tot es pot configurar la llista més enllà de les opcions que s'ofereixen en el mòdul d'administració de la llist, si pregunteu els administradors).
5.  Indiqueu un **assumpte** per a la llista. Aquest assumpte apareixerà com a capçalera de totes les pàgines de la llista i també estarà visible en les pàgines d'índex de la llista (llista de llistes, llista de subscripcions, etc.) i en la barra del títol del navegador.
6.  Elegiu un **tema** de les opcions de la pestanya «Tema» en el menú desplegable.

    | Note |
    |------|
    | Si no n'hi ha cap tema adequat, podeu sol·licitar la creació d'un nou tema als administradors. |

7.  Indiqueu una **descripció** per a la llista. La descripció es mostrarà en la pàgina d'informació de la llista i en les «normes de funcionament per als subscriptors» enviada per correu a cada nou subscriptor, el cap 'Assumpte' de la capçalera. Aquesta descripció pot incloure explicacions sobre les següents qüestions:

    -   motius i objectius de la llista;
    -   temes de discussió;
    -   funcionament de la llista (responsabilitats, estat de la llista, etc.);
    -   normes que s'apliquen;
    -   descripció dels subscriptors típics (ocupacióm projectes que gestionen, nacionalitat, etc.).

    | Note |
    |------|
    | Podeu formatar la descripció de la llista amb etiquetes d'HTML. Atenció: si la descripció és llarga, talleu-la amb salts de línia manuals (tecla ENTER del teclat); sinó, pot haver problemes perquè es veja sencera en la finestra del navegador. |

8.  Feu clic en el botó «**Envia sol·licitut de creació**».

Apareixerà un missatge per a informar que s'ha enviat la sol·licitut de creació als administradors i que, a partir d'aquest moment, es pot modificar la llista fent clic en el botó «Administrar». Tot i això, el missatge adverteix que la llista no s'instalarà i serà visible fins què l'administrador l'haja aprovat.

Després d'això, haureu d'**esperar que un dels administradors aprove la creació de la llista**. Aleshores, rebreu un missatge d'avís amb el títol «**Creació de la llista nomdelallista**», per informar que la llista s'ha creat.

**Per últim, sucribiu-vous a la llista**: crear una llista o ser-ne el propietari o moderador no implica que us subscriviu automàticament!

### Com gestionar una llista

Per a gestionar una llista en què sou el propietari, seguiu els passos següents:

1.  Aneu a la **pàgina d'inici de l'entorn de la llista** y **[iniciu sessió](user#sympa_auth.md)**.

    | Note |
    |------|
    | Si esteu subscrit a la llista amb més d'una adreça, empreu l'adreça amb què heu demanat la creació de la llista. |

2.  **Aneu a la pàgina d'informació de la llista** que voleu gestionar.
3.  En el menú de l'esquerra, **feu clic en l'enllaç «Admin»**.

Aneu al menú de l'esquerra i feu clic en «Admin», per a navegar per les seccions del mòdul d'administració.

Les diferents seccion permeten:

-   [configurar la llista](listconfig.md);
-   [personalitzar fitxers relacionats amb la llista](#customize);
-   [gestionar subscriptors](#manage_members);
-   [gestionar l'arxiu dels missatges de la llista](#manage_archives);
-   [gestionar rebots](#manage_bounces);
-   [crear, eliminar o restaurar l'espai web per a compartir documents](#manage_shared);
-   [canviar el nom de la llista](#renamelist);
-   [eliminar la llista](#supprlist).

Les opcions que hi ha en «Moderar» dins del submenú us permeten:

-   [moderar missatges](#moderate) enviar a la llista;
-   [moderar documents](shared.md) que està en l'espai web per a compartir documents;
-   [moderar subscripcions pendents](#manage_members).

#### <span id="edit_list"></span>Com configurar la llista

Per a aprendre a configurar la llista, aneu a [**documents sobre la configuració de llistes**](listconfig.md).

#### <span id="customize"></span>Com personalitzar la llista

Des d'aquesta pàgina, podeu **editar el nombre de fitxers relatius a la llista**, d'entre aquests:

-   missatges típics que s'envien als subscriptors en ocasions concretes:
    -   **missatge de benvinguda**: aquest missatge és la notificació que s'envia a la gent que s'acaba de subscriure. Heu d'escriure unes normes de funcionament per a la llistam i afegir-la en el missatge de benvinguda. Podeu crear un missatge estructurat amb MIME (reservat per a experts de format en MIME);
    -   **missatge de donada de baixa**: aquest missatge s'envia a la gent que es dóna de baixa de la llista;
    -   **missatge d'eliminació**: aquest missatge s'envia a la gent que doneu de baixa de la llista (ordre DEL), sobretot perquè l'adreça causa rebots;
    -   **missatge de recordatori**: aquest missatge s'envia als subscriptors com a recordatori personalitzat quan s'utilitza l'ordre RECORDATORI. Aquesta ordre és bàsica per a la bona gestió de la llista ja que molts dels rebots es deuen al fet que alguns subscriptors tenen una adreça que no és l'adreça amb què es van subscriure o que, fins i tot, s'han oblidat que estan subscrits a la llista;
    -   **missatge d'invitacióp a subscriure's**: aquest missatge s'envia a la gent que inviteu a subscriure's a la llista emprant l'ordre INVITE;
    -   **notificació de missatge rebutjat pel moderador**: aquest missatge s'envia al remitent del missatge que ha rebutjat el moderador;
    -   **avís de missatge rebutjat per un virus**: aquest missatge s'envia al remitent del missatge en què s'ha trobat el virus.
-   fitxers diversos:
    -   **descripció de la llista**: la descripció de la llista s'envia per correu com a resposta a l'ordre INFO. Per defecte, també s'inclou en el misstage de benvinguda (notificació de subscripció). Aquesta descripció no és la mateixa que es veu en l'interfície web de la llista de correu;
    -   **pàgina d'inici de la llista**: aquesta descripció està disponible en la pàgina d'informació de la llista. Pot estar en format HTML. Tot i que empreu aquest format, empreu `<br />` etiquetes per indicar els salts de línia;
    -   **capçalera dels missatges**: quan està disponible, s'afegeix com a MIME al començament de cada missatge distribuit a la llista;
    -   **peu de pàgina del missatge**: quan està disponible, s'afegeix com a MIME al final del missatge distribuit a la llista.

Per defecte, Sympa empra fitxers predeterminats; en aquest cas, els fitxers específics que es corresponen amb la llista estan buits. **Per a editar una arxiu, elegiu de la llista deplegable l'opció «Edita»**. Tindreu la opció de canviar el **camp «De»** (remitent), el **camp «Assumpte»** (línia d'assumpte) i el **cos del missatge**.

| Note |
|------|
| Aneu amb compte: els valors entre claudàtors poden variar. No els canvieu, si no sabeu que esteu fent... |

#### <span id="manage_shared"></span>Gestionar l'espai web per a compartir documents

Per defecte, les llistes no tenen un espai web per a compartir documents. Així, doncs, heu de crear un. Per a fer-ho, aneu al **mòdul d'administració de la llista** i feu clic en l'enllaç de «**Creació compartida**».

Per a permetre que els subscriptors publiquen documents en l'espai web per a compartir documents, necessiteu **canviar els permisos predeterminats**: en el mòdul d'administració de la llista feu clic en «**Editar configuració de la llista**» i després en «**Privilegis**». En el botó de la pàgina, hi ha una llista desplegable amb el nom «[**Qui pot editar**](listconfig#docsrights.md)»; elegiu l'opció «**Restringit per als subscriptors (privat)**».

| Note |
|------|
| Aneu amb compte: si creeu carpetes abans de cambiar els permisos, ja que aquestes carpetes continuaran sense poder-se modificar. Si voleu que es puguen modificar, haureu de [canviar els permisos d'accés](shared#acces.md) per a cada carpeta. |

També podeu voler [establir unes **cuotes**](listconfig#docsrights.md) per a l'espai web per a compartir documents en la pàgina de «Privilegis», la secció d'«Editar la configuració de la llista».

Per a **saber tot sobre la gestiò de l'espai web per a compartir documents** (com organitzar-ho, canviar els permisos d'accés, nom de documents, etc.), aneu a la Guia de l'Usuari, secció «[Com emprar l'espai web per a compartir documents](shared.md)».

Per a **denegar l'acess a l'espai web per a compartir documents**, en el menú d'«Adminisrtar»feu clic en «**Elimina espai compartit**». Aleshores, encara tindreu la possibilitat de **reobrir-lo** fent clic en «**Restaurar espai compartit**». Tot i que elimineu o restaureul'espai web per a compartir documents, això **no afectarà els documents que conté**.

#### <span id="manage_members"></span>Com gestionar els subscriptors

Aquesta secció us permet navegar per la **la llista de tots els subscriptors de la llista**. La informació següent, està disponible per a cada subscriptor:

-   **adreça electrònica**;
-   **domini** de la adreça electrònica (*@cru.fr*, *@sympa.org*, *@fai.com*, etc.);
-   **imatge** (si es va activar aquesta funció per a la llista);
-   **nom** (segons el mètode d'inscripció, no sempre es pot veure);
-   [**modalitat d'entrega del missatge**](#deliverymode);
-   **font de dades** s'indica l'origen en cas que el subscriptor estiga inclos en la llista, però no subscrit directament;
-   **data d'inscripció** en la llista;
-   **darrera actualització** de les opcions del subscriptor.

| Note |
|------|
| Per defecte, cada pàgina mostra 25 subscriptors. Podeu navegar per les pàgines emprant les fletxes de navegació o mitjançant l'opció de mostrar més subscriptors per pàgina. També podeu reordenar la llista de subscriptors segons diferents criteris fent clic en la capçalera de la columna corresponent. |

Per a **cercar un subscriptor**, introduïu tot o part de l'adreça electrònica o el nom del subscriptor en el camp d'entrada i feu clic en el botó de «**Cerca**».

Podeu **subscriure altres persones a la llista** des d'aqueste pàgina:

-   Per a afegir **només a una persona**, introduiu l'adreça d'aquesta en el camp d'entrada i feu clic en el botó de «**Afegeix**».
-   Per a afegir **més d'una persona**, fue clic en el botó «**Afegeix més d'un**». En el camp d'entrada que es veu, introduiu les adreces electròniques i els noms de les persones que voleu subscriure a la llista i feu clic en «**Afegeix subscriptors**».

| Note |
|------|
| Si voleu subscriure algú sense fer-s'ho saber amb una notificació, elegiu la casella de «Silenciós». Tot i així, és millor avisar la gent què els has subscrit! |

Encara que podeu subscriure persones a les vostres llistes de correu, sempre és **molt millor que facin els passos necessaris per a subscriure-s'hi per ells mateixos**. També podeu **invitar gent perquè es subscriguin a la llista** a través de l'ordre INVITE: envieu un correu a {{conf.email}}@{{conf.host}} i escriviu l'ordre següent en el cos del missatge: **convidar nomedelallista adreçalectrònica** (exemple: *convida llista\_exemple john.doe(@)fai.com*).

Per a **aceptar o rebutjar les sol·licituds de subscripció a la llista**, feu clic en «**Subcripcions pendents**». Es mostrarà la llista de tota la gent que a sol·licitat subcriure-s'hi. Per a acptar o rebutjar una sol·licitud, marqueu la casella que hi és davant el nom d'una persona o feu clic en el botó que volgueu.

Per a **enviar un recordatori de subscripció a tots els subscriptors**, feu clic en el botó «**Recorda a tots**». El missatge recordatori de subcripció conté:

-   el **nom de la llista** en què el subscriptor està subscrit;
-   l'**adreça electrònica** amb què es va subscriure;
-   la **contrasenya de la llista** del subscriptor;
-   un **enllaç a la pàgina d'informació** de la llista;
-   una **adreça per a donar-se de baixa de la llista fent clic al damunt**.

| Note |
|------|
| També podeu configurar un recordatori de subscripció automàtica, per fer això, aneu a la secció «Edita la configuració de la llista» i elegiu la pàgina «[Miscel·lània](listconfig#other.md)». |

Per a **donar de baixa un subscriptor** des d'aquesta pàgina, seleccioneu-los marcant les caselles que hi ha davant dels noms i feu clic en el botó «**Elimina les adreces electròniques selesccionades**».

| Note |
|------|
| Si no voleu que els subscriptors reben un avís, feu marqueu la casella «Silenciós». Tot i així, no es reconomana aquesta opció excepte en casos de subscriptors inaccesibles. |

| Note |
|------|
| Consell: per seleccionar tots els subscriptors d'una vegada, primer us heu d'assegurar que es veuen tots en una pàgina, i fer clic en el botó «Commuta la selecció»: tots els subscriptors es seleccionaran amb un clic! |

Per a **canviar les opcions de subscripció d'un subscriptor**, feu clic en l'adreça electrònica d'aquest.

Des d'aquesta pàgina, podeu **canviar el nom, l'adreça electrònica i la modalitat d'entrega del subscriptor**. També podeu **donar-lo de baixa**.

Si el subscriptor està [retornant missatges](#manage_bounces), es veura un altre formulari en el formulari de «Informació del subscriptor»:

La informació que es mostra inclou:

-   el tipus d'error (en Anglès);
-   el nombre d'errors;
-   el període de temps en què van haver errors.

Podeu **verificar l'últim error** o **reiniciar els errors**. Si reiniceu els errors, la [puntuació](listconfig#bouncers.md) del subscriptor es posarà a cero.

Per a gestionar amb més facilitat les adreces que generen missatges retornats, aneu al mòdul d'administració i elegiu la pàgina de «[Retornats](#manage_bounces)».

#### <span id="manage_bounces"></span>Com gestionar retornats

Quan hi ha un **problema amb les adreces electròniques dels subscriptors** (adreces electròniques obsoletes, adreces que estaben temporalment no disponibles quan es van enviar els missatges, que s'ha excedit la quota de la bústia d'entrada, etc.), el percentatge d'adreces que generen missatges retornats es pot veure en el menú de l'esquerra amb el nom de «**Freqüència d'error**». Per a verificar les adreces amb retornats, aneu al mòdul d'administració, la pàgina de «**Retornats**».

El programari de Sympa gestiona automàticament els subscriptors amb retornats: segons el nombre d'errors i el trànsit de la llista, també es notifica, dona de baixa o se'ls posa la puntuació a cero quan l'adreça deixa de fer retornats als subcriptors inaccesibles.

Per **fer que les adreces deixen de fer retornats**, seleccioneu-los marcant les caselles i fent clic en el botó «**Reiniciar errors per als usuaris seleccionats**». Si l'error continua, les adreces es llistaran com a retornats una altra vegada, tan prompte com s'envie un missatge a la llista.

També podeu **donar de baixa subscriptors les adreces dels quals continuen fent retornats**: si hi ha moltes adreces que fan retornats el servidor de la llista de correu es carrega bastant. Per a donar de baixa subscriptors, seleccioneu-los marcant les caselles de davant els noms i feu clic en el botó «**Elimina les adreces electròniques seleccionades**».

| Note |
|------|
| Consell: per seleccionar tots els subscriptors d'una vegada, primer us heu d'assegurar que es veuen tots en una pàgina, i fer clic en el botó «Commuta la selecció»: tots els subscriptors es seleccionaran amb un clic! |

#### <span id="moderate"></span>Com moderar els missatges que s'envien a la llista

Quan es modera una llista, **tots els missatges han de ser aprovats per un dels moderadors abans que no es distribueixen a la llista**. Després d'enviar un missatge a la llista, es notifica automàticament als subscriptors que es revisarà el seu missatge. Qant als moderadors, també reben una notificació de Sympa, que inclou el missatge que s'ha de revisar.

Podeu **realitzar tasques de moderació** ja siga **pel correu electrònic**, responent els missatges del Sympa, o **a través de la interfície web de la llista de correu**. Per a fer-ho, aneu al submenú «Modera» i feu clic en l'enllaç «**Missatge**»: que us envia a una pàgina que mostra tots els missatges que s'han de moderar (els missatges més recents estan al començament de la pàigna). **Per a llegir un missatge feu clic en l'assumpte**.

Teniu **dos opcions**:

-   **autoritzar la distribució del missatge** a la llista;
-   **rebutjar el missatge i notificar-s'ho al remitent**: quan rebutjeu un missatge, és millor notificar-s'ho al remitent...

Tots els moderadors poden decidir si distribuir un missatge o no. No obstant això, **el primer moderador que processe el missatge serà qui decidisca**. Sympa us enviarà una notificació si intenteu processar un missatge que ja ha estat revisat. Quan hi ha diversos moderadors, és **més fàcil moderar els missatges des de l'interfície web de la llista de correu**: ja que mostra els missatges que falta revisar.

| Note |
|------|
| **Sense importar la data i el moment de la revisió, la data i el moment d'enviament del missatge no canvia**. De manera que si la distribució del missatge s'aprova amb molt d'endarreriment, és pot rebre un missatge del dia 1 de gener el dia 31 de desembre! |

En el cas que el missatge s'haja rebutjat amb una notificació, el subscriptor que ha enviat el missatge rebre una notificació per correu electrònic. Podeu [personalitzar el missatge que reba](#customize).

Si s'activa la casella de «**Rebutja sense notificació**» l'autor del missatge no rebrà una notificació.

Si activeu la casella de «**Afegir a la llista negra**» omet la notificació i afegeix l'autor a la llista negra de la llista. Podeu gestionar la llista negra si anau a la part inferior de la pàgina i feu clic en el botó «**editar llista negra**».

Si voleu personalitzar el missatge de rebutjament que s'envia a l'autor, podeu fer-ho a través del botó «**Gestiona els missatges de rebutjament**». La pàgina de gestió dels missatges permet definir un conjunt de missatges de rebutjament i definir-ne un per defecte.

**Recordatori**: podeu [afegir o eliminar moderadors](listconfig#description.md) a través del mòdul d'administració de la llista. Per a fer-ho, heu d'anar a la pàgina d'informació i entrar en «**Edita configuració de llista**», després en «**Definició de la llista**» i per últim en «**Administra**».

També es possible **processar missatges després que s'hagen distribuit en la llista**; fet que podria ser útil quan una llista no està moderada. Si voleu **eliminar un missatge**, [cerqueu-ho en l'arxiu de missatges en línia](arc#arcsearch.md) aneu a la part superior dreta del missatge i feu clic en el botó «**Etiqueta aquest correu per a eliminar**». Es mostrarà un missatge de confirmació; feu clic en «OK». Després de uns pocs segons s'eliminarà el missatge . **Aneu en compte: aquesta acció és irreversible! Si elimineu un missatge, no podreu recuperar-lo.**

#### <span id="manage_archives"></span>Gestionar l'arxiu de missatges

El robot de gestió de llistes de correu de Sympa pot generar **arxius válids per a baixar-se(en format .ZIP) dels missatges que s'envien a la llista**. Per a baixar-se aquests arxius, **seleccioneu els mesos** que us interesen de la llista i feu clic en el botó «**Baixar fitxer Zip** ».

| Note |
|------|
| Nota: per a seleccionar tots els mesos en què s'han enviat missatges, aneu a la llista «Sel·lecció d'arxiu» i feu clic en el primer mes, mantingueu premut el botó de SHIFT i feu clic en l'últim botó de la llista. |

Rebreu un fitxer del tipus «**nomdelallista\_arxiu.zip**» que contindrà **carpetes amb els noms de «nomdelallista\_any-mes»** (exemple: *llista\_exemple\_2005-06*) per cada mes. Dins de cada carpeta, **els noms dels fitxers són números** que representen la posició cronològica del missatge enviat (exemple: el fitxer amb el nom «1» inclou el primer missatge que s'ha enviat del mes). Els fitxers dels missatges **no tenen una extensió**; però podeu obrir-los amb l'editor de text que elegiu (Notepad, WordPad, Vim, etc.). **Cada fitxer representa un missatge sencer (amb totes les capçaleres)**.

Des de la pàgina «Gestionar arxius», també es pot **eliminar missatges** (s'eliminen mes per mes i no missatge a missatge). Per a fer això, s'ha de **seleccionar els mesos** que interesen de la llista i fer clic en el botó «**Elimina els mesos seleccionats**».

| Note |
|------|
| **Atenció: aquesta acció és irreversible! Quan feu clic en «Elimina els mesos seleccionats», recordeu que no sols esteu eliminant un fitxer d'un arxiu, sinó tot l'arxiu complet del missatge del mes seleccionar!** |

#### <span id="renamelist"></span>Com renombrar una llista

En el **mòdul d'aministració de la llista**, feu clic en «**Renombra la llista**». Escriviu el nom que elegiu i feu clic en el botó de «Renombra aquesta llista». Apareoxerà un missatge de confirmació; feu clic en «D'acord».

| Note |
|------|
| Si canvieu de parer, sols haureu de refer l'acció inversa per a recuperar el nom anterior de la llista. |

**Atenció: quan renombreu la llista, s'ho has de dir als adminisrtador, sinó, el canvi no serà efectiu**.

Alguns consell per posar nom a una llista:

-   **No empreu espais, accents o caràcters especials** en el nom de la llista: aquests caràcters poden causar problemes.
-   Elegiu **un nom explicit però curt**: penseu en els subscriptors que han d'escriure el nom cada vegada que envien un missatge a la llista!
-   Si gestioneu un conjunt de llistes, podeu **emprar un prefix comú per als noms de totes les llistes**; així, es mostraran juntes en els llistats i es podran reconèixer fàcilment (exemple: *xx-users@{{conf.host}}, xx-hotline@{{conf.host}}.fr*, etc.).

#### <span id="supprlist"></span>Com eliminar una llista

En el **mòdul d'adminstració de la llista**, feu clic en «**Elimina la llista**». Apareixerà un missatge de confirmació; feu clic en «D'acord».

| Note |
|------|
| **Atenció: si elimineu la llista, no podreu tornar a obrir-la vosaltres mateixos! Si es voleu reobrir la llista, s'ho haureu de demanar als administradors.** |

En realitat, quines són les **conseqüències** d'eliminar una llista?

-   **Tots els subscriptors es donen de baixa de la llista immediatament** de manera automàtica (fins i tot els propietaris i els moderadors).
-   **Es desa l'arxiu dels missatges** però ningú no pot tornar a accedir.
-   **Es guarden els documents que es publiquen en l'espai compartit de documents del web** però ningú no pot tornar a accedir.
-   **Només els administradors poden reobrir una llista**; si ho fan, els antics subscriptors de la llista es tornen a subscriure automàticament.

| Note |
|------|
| Atenció: a causa d'una petita latència, es pot accedir a les llistes un temps després que s'hagen tancat si es sap la direcció. Després seran completament inaccesibles. |

**Si vols que la llista i tots els fitxers associats s'eliminen de permanentment**, s'ho haureu de demanar als administradors.

### <span id="rulesadmin"></span>Bones pràctiques

Per a aconseguir llistes dinàmiques, **heu de participar activament** en els intercanvis: si una llista no està controlada o animada pels propietaris, els missatges poden perdre qualitat i pot acabar per desaparèixer...

**La utilització del correu electrònic en general i de les llistes de correu té una serie de normes precises i necessàries per a intercanviar comunicacions satisfactòries: la «Netiqueta»**. Com a propietari o moderador, teniu la responsabilitat fer que els subscriptors les respecten. Trobareu els principis generals de la Netiqueta, així com molts altres enllaços en la [pàgina de Wikipedia dedicada a la Netiqueta](http://en.wikipedia.org/wiki/Netiquette).

<span id="charter"></span>Heu d'**escriure unes normes de funcionament per a la vostra llista** per a definir totes les normes que s'aplicaran durant la utilització d'aquesta:

-   temes permesos, tolerats i prohibits;
-   escriure normes (per exemple per especificar els llenguatges en que poden publicar els subscriptors, per prohibir la utilització de llenguatge «SMS», etc.);
-   les normes que s'han d'aplicar quan s'envien missatges (freqüència, fitxers adjunts, etc.);
-   responsanilitats dels subscriptors respecte de la netiqueta;
-   drets i responsabilitats dels subscriptors;
-   informació sobre la retenció dels missatges enviats a la llista;
-   informació legal i polítiques de privacitat;
-   les sancions per qui no respecte les normes de funcionament de la llista;
-   etcetera.

| Note |
|------|
| Per què tots els subscriptors llegeixen les normes de funcionament, heu d'incloure-la en el missatge de benvinguda que reben després que s'hagen subscrit. Per fer-ho, heu d'anar al mòdul d'administració, a la pàgina de «Personalitzar», apartat de [personalitzar el missatge](#customize). |

~~When available, the 'Owner and moderator charter' provides list owners and moderators with all the necessary information to carry out their roles. This Charter involves all the rights and responsibilities of owners and moderators.~~

------------------------------------------------------------------------
