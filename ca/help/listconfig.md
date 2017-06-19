<span id="listconfig"></span>Com configurar la llista
-----------------------------------------------------

Com la configuració de la llista és un poc complicada, es divideix en diferents parts amb una pàgina diferent per cada part:

-   [Definició de la llista](#description);
-   [Enviaments/rebuts](#sending);
-   [Privilegis](#command);
-   [Arxiu](#archives);
-   [Retornats](#bounces);
-   [Miscel·lània](#other).

Recomanem que **feu els canvis de configuració de forma progressiva**: de maenra que si el resultat no és el que esperaveu, serà més fàcil desfer els canvis.

El mòdul d'administració de la llista us ofereix **moltes opcions per a configurar la llista**. No obstant això, aquestes opcions poden no adaptar-se perfectament a les vostres necessitats. Per a sol·lucionar aquest problema, podeu **preguntar els administradors de la llista per crear opcions noves** (per suposat, dins dels límits de tot el que poden fer): l'accés o els drets estan limitats segons les categories dels usuaris depenent del lloc des d'on inicien sessió, el domini o l'adreça de correu, el grup d'usuaris al qual pertanyen, etc.

### <span id="description"></span>Definició de la llista

En el camp de «**Assumpte de la llista**», podeu canviar l'assumpte que vau elegir quan vau crear la llista. Aquest assumpte es mostra com a capçalera de totes les pàgines de la llista, també es pot veure en l'índex de pàgines de la llista (llista de llistes, llista de les subscripcions, etc.) i en la barra de títols del navegador.

També podeu canviar «**Visibilitat de la llista**». Les opcions disponibles són les següents:

-   ocult excepte per als subscriptors (conceal) - *opció predeterminada*;
-   accés instantani (intranet);
-   sense ocultar (nonconceal);
-   ocult fins i tot per als subscriptors (secret);

| Note |
|------|
| Si voleu limitar la visibilitat de la llista segons altres criteris, heu de preguntar els adminisrtadors de la llista: poden crear una opció nova per què coincideixi amb les vostres necessitas (exemple: la llista és visible sols per als membres d'un grup d'usuaris, d'un domini d'Internet, etc.). |

En les àrees de «Propietaris» i «Moderadors», podeu **afegir propietaris i moderadors** a la llista o **canviar la informació personal d'aquests**:

-   Per a cada propietari/moderador, heu d'indicar una **adreça de correu** i un **nom**.
-   També podeu afegir informació una opció «**Informació privada**» safata d'entrada (número de teléfon, funció, etc.); aquesta informació només serà accesble per als adminsirtadors amb perfil «Privilegiat».
-   Podeu canviar **la modalitat d'entrega** (les úniques opcions disponibles en aquesta pàgina són «mail» i «nomail»).
-   El paràmetre «Perfil» no es pot canviar: el **Perfil «privilegiat»** es reserva al creador de la llista (altres propietaris tenen el perfil «Normal»).

| Note |
|------|
| Atenció: ser propietari o moderador de la llista no significa que esteu automàticament subscrits a la llista. De maner que els propietaris i moderadors es tenen que subscriure a la llista. |

Per **eliminar propietaris/moderadors**, neteja el contingut de les safates d'entrada de la persona que vulgueu eliminar i feu clic en el botó «Actualitzar».

També podeu canviar **el tema de la llista** així com la **llengua**. Si canvieu la llengua de la llista, tots els missatges predeterminats s'enviaran en la llengua elegida (aneu amb compte: aquesta opció depèn de si està traduït).

No podeu canvier el **domini d'Internet** de la llista: només els administradors poden canviar aquest paràmetre.

**Atenció: no oblideu fer clic en el botó «Actualitzar»** que apareix en la part de sota de la pàgina per a desar els canvis.

### <span id="sending"></span>Enviaments i rebuts

Des d'aquesta pàgina, podeu **decidir qui podrà publicar missatges en la llista**.

En l'àrea de «**Freqüència de recopilació**», es pot definir la freqüència amb que s'envien els missatges compilats (modalitats d'entrega Digest i Summary): en la llista, seleccioneu tots els **dies** dels quals voleu que s'envie un recopilatori. Després elegiu una **data d'entrega** per als recopilatoris (eviteu elegir una hora enrte les 11 i les 12 de la nit).

En la llista d'«**Opcions de subscripció disponibles**», seleccioneu totes les opcions de subscripció que voleu oferir als subscriptors. Per defecte, estan seleccionades totes les opcions.

L'àrea d'«**Adreça de resposta**» permet definir els destinataris predeterminats de qualsevol resposta que s'envie a un missatge de la llista:

-   Amb el valor «**Tots**», la resposta s'envia al **remitent del missatge** i a la **llista**.
-   Amb el valor «**Llist**», la resposta s'envia a la **llista**.

    | Note |
    |------|
    | Atenció: aneu amb compte amb aquesta opció. La experiència demosrta que els subscriptors no comproven sempre l'adreça a que van enviar la resposta. De manera que, poden enviar missatges privats a tota la llista quan intenten respondre a una persona... |

-   Amb el valor «**Other\_email**», la resposta s'envia a una **adreça predetermiada**. Si elegiu aquesta opció, haureu d'**indicar una adreça de correu en la casella de «Altra adreça de correu»**.
-   Amb el valor «**Remitent**», la resposta s'envia al **remitent del missatge**. És possible que elegiu aquesta opció.

El desplegable «**Respecta la capçalera que hi ha**» permet elegir com es processarà la capçalera «Reply-To» SMTP dels missatges que s'envien a la llista. L'opció de «**Respecta**» manté el valor de la casella mentre l'opció «**Força**» permet sobreescriure-la.

Per últim, l'opció «**Etiquetació de l'assumpte**» permet elegir el **text que s'inclou abans de s'assumpte de tots els missatges** que s'envien a la llista: això permet als subscriptors ordenar els missatges fàcilment, emprar filtres per a processar missatges automàticament, etc. Per defecte, aquest text consisteix en el **nom de la llista entre claudàtors** (els sistema afegeix automàticament els claudàtors, de manera que no cal que els escriviu).

**Atenció: no oblideu fer clic en el botó «Actualitzar»** que apareix en la part de sota de la pàgina per a desar els canvis.

### <span id="command"></span>Privilegis

Des d'aquesta pàgina, podeu decidir:

-   **qui pot veure la informació de la llista**. Les opcions disponibles són:
    -   per a qualsevol (open) - *opció predeterminada*;
    -   restringida als subscriptros (private).
-   **qui pot subscriure's a la llista**. Les opcions disponibles són:
    -   petició de subscripció confirmada (auth);
    -   necessita autentificació (s'envia una notificació als propietaris) (auth\_notify);
    -   necessita autentificació i l'aprovació del propietari (auth\_owner);
    -   subscriure-s'hi és impossible (closed);
    -   restringida als usuaris del domini local (intranet);
    -   aprovació dels usuaris del domini local o dle propietari (intranetorowner);
    -   per a qualsevol sense autenticació (open) - *opció predeterminada*;
    -   qualsevol, s'envia una notificació al propietari de la llista (open\_notify);
    -   qualsevol, sense missatge de benvinguda (open\_quiet);
    -   aprovació del propietari (owner);
    -   cal que estiga signat en S/MIME (smime);
    -   cal que estiga signat en S/MIME o l'aprovació del propietari (smimeowner).

        | Note |
        |------|
        | Heu d'elegir sempre una opció que incloga el paràmetre «auth»; d'aquesta manera, el sistema demana una confirmació per correu al futur subscriptors abans que s'el subscriga a la llista. Això evita subscripcions amb adreces de correu invàlides i garanteix que ningú pot ser subscrit a la llista sense saber-ho. |

-   **qui pot donar-se de baixa de la llista**. Les opcions disponibles són:
    -   necessita autentificació (auth);
    -   cal una petició d'autentificació, s'envia un avís al propietari (auth\_notify);
    -   impossible (tancada);
    -   oberta (open) - *opció predeterminada*;
    -   oberta amb un correu de confirmació, s'avisa el propietari (open\_notify);
    -   aprovació del propietari (owner).

        | Note |
        |------|
        | Heu d'elegir sempre una opció que incloga el paràmetre «auth»; d'aquesta manera, el sistema demana una confirmació per correu al futur subscriptors abans que s'el subscriga a la llista. Això evita que gent malintencionada done de baixa a algú sense que aquest ho sàpiga. |

-   **qui pot invitar gent a què es subscriga a la llista**. Les opcions disponibles són:
    -   tancat (closed);
    -   propietari de la llista, sense autentificació (owner);
    -   restringida als subscriptors (private) - *opció predeterminada*;
    -   públic (public).
-   **qui pot veure els subscriptors**. Les opcions disponibles són:
    -   ningú no pot veure'ls (closed);
    -   restringit als subscriptors o als usuaris del domini local (intranet);
    -   només els administradors (listmaster);
    -   només el propietari (i els administradors) (owner) - *opció predeterminada*;
    -   restringit als subscriptors (private);
    -   tothom pot veure'ls! (public).

        | Note |
        |------|
        | No haurieu de deixar mai que tothom puga veure la llista de membres. L'opció «restringit als subscriptors» és la opció més interessant per què els subscriptors es puguen comunicar sense que hagen de publicar missatges en la llista. No obstant això, aquesta opció no és l'adequada en cas d'una llista d'avisos que incloga subscriptors que no tinguen cap mena de relació. |

<span id="docsrights"></span>Des d'aquesta pàgina, també podeu **definir els drets d'accés que s'apliquen a l'espai compartit de documents del web** (la secció de «Documents compartits» de la llista és accessible a través de l'enllaç del menú de l'esquerra). Podeu definir tant els drets de lectura com d'escriptura dels documents:

-   El desplegable «**Qui pot veure**» té les opcions següents:
    -   restringit als subscriptors o als usuaris del domini local (intranet);
    -   restringit als propietaris (owner);
    -   restringida als subscriptors (private) - *opció predeterminada*;
    -   documents públics (public).
-   El desplegable «**Qui pot editar**» té les opcions següents:
    -   restringit als propietaris (owner) - *opció predeterminada*;
    -   moderat pels subscriptors (editor);
    -   restringit als subscriptors (private);
    -   documents públics (public).

La casella «**Quota**» permet definir un **tamany màxim que no es podrà superar per a l'espai compartit de documents del web**. Aquest tamany no representa el tamany màxim d'*un* document publicat en l'espai compartit de documents web, sinó el tamany màxim per a tots els documents publicats en la llista. S'expressa en kilobytes. Quan un subscriptor intenta publicar un document massa gran per a l'espai que queda, rep un missatge d'error.

Per a saber **més sobre la gestió i compartició de l'espai compartit de documents del web** (com organitzar-lo, canviar els drets d'accés, anomenar els documents, etc.), aneu a la secció de la Guia de l'usuari, «[Com utilitzar l'espai compartit de documents del web](shared.md)».

**Atenció: no oblideu fer clic en el botó «Actualitzar»** que apareix en la part de sota de la pàgina per a desar els canvis.

### <span id="archives"></span>Arxiu

Des d'aquesta pàgina, podeu **decidir qui pot accedir a l'arxiu de la llista en línia** (missatges legibles en la interfície web de la llista de correu). Les opcions disponibles són:

-   tancat (closed);
-   restringida als usuaris del domini local (intranet);
-   administrador (listmaster);
-   propietari (owner);
-   moderador (moderator);
-   només els subscriptors (private);
-   públic (public).

La casella «**Quota**» permet definir un **tamany màxim que no es podrà superar per a l'arxiu de missatges**. Aquest tamany s'expressa en kilobytes. Els propietaris de la llista reben un avís quan l'arxiu arriba a un 95 % del tamany permès. Quan s'arriba al tamany màxim, no es reben més missatges.

| Note |
|------|
| Encara que els missatges no s'arxiven, naturalment, es pot continuar enviant missatges a la llista. |

També es pot **accedir a l'arxiu de la llista per correu**, enviant **{{conf.email}}@{{conf.host}}** l'ordre següent: <span class="commande">**GET nomdelallista year-month**</span> (exemple: *GET list\_example 2016-07*). Aleshores, rebreu una compilació de tots els missatges enviats durant el mes que hageu elegit. Aquesta compilació s'envia en text net i conté etiquetes HTML en comptes del format original; també inclou capçaleres completes per a cada missatge. El paràmetre «**Arxius de text**» permet definir:

-   **qui pot** rebre l'arxiu de missatges de la llista per correu;
-   **amb quina freqüència es crearan aquests fitxers de l'arxiu**. Per exemple, si la freqüència s'estableix en «mes», tots els missatges que es distribueixen durant un mes en la llista s'arreplegaran en un únic fitxer de l'arxiu.

Si no s'especifica aquest paràmetre, la llista no tindrà un arxiu accessible per correu. Atenció: **només els adminisrtadors poden canviar aquest paràmetre.**

Es poden enviar **missatges encriptats en S/MIME** a la llista. L'opció «**Arxivar correus encriptats com a text net**» permet elegir com es volen arxivar els missatges:

-   L'opció «**Desencriptar**» arxiva el missatge desprès de llevar l'encriptament.
-   L'opció «**Original**» arxiva el missatge amb la seva forma encriptada original.

Aquesta opció s'aplica per al text de l'arxiu i per a l'arxiu en línia, així com per a les compilacions que s'envien a qui va elegir la modalitat d'entrega «Recopilatori».

**Atenció: no oblideu fer clic en el botó «Actualitzar»** al final de la pàgina per a desar tots els canvis.

### <span id="bounces"></span>Retornats

Els «**retornats**» representen els **subscriptors les adreces dels quals tenen errors**, per ex. els subscriptors que no poden rebre els missatges enviats a la llista. Això pot tenir moltes raons: una adreça de correu obsoleta, adreces inaccessibles temporalment quan es van enviar els missatges, s'ha passat el màxim de la quota de la safata d'entrada, etc.

La secció «**Gestió de retornats**» defineix dos ràtios:

-   La **ràtio d'avís** indica la ràtio d'adreces de correu amb retornats de les quals el propietari rebrà un **avís amb el nom «Ràtio de retornats massa alta»** per què elimini els subscriptors amb retornats de la llista.
-   La **ràtio d'aturada** indica la ràtio d'adreces de correu amb retornats a les quals **s'aturarà la distribució de missatges automàticament** fins que es resolga el problema (en general fins que s'eliminen els subscriptors amb retornats).

<span id="bouncers"></span>Les seccions «**1r nivell de gestió de retornats**» i «**2n nivell de gestió de retornats**» permeten fer tasques automàtiques per a controlar els retornats dels subscriptors. Podeu definir:

-   els **rangs de puntuació que defineixen el nivell 1 i el nivell 2 de retornats**. Per defecte, els retornats de nivell 1 tenen una puntuació entre 45 i 74 i els de nivell 2 tenen una entre 75 i 100;

    | Note |
    |------|
    | La puntuació depèn del nombre, tipus i freqüència dels errors. Si el temps de retornats és molt curt o si no ha tingut molts errors, no es puntua al subscriptor amb retornats. |

-   les **mesures que es prenen amb els subscriptors involucrats** són: no hi ha mesures, avís, eliminació de la llista;
-   **persona que rep l'avís** quan es pren la mesura: ningú, els propietaris de la llista, els administradors. L'avís que s'envia quan es pren una mesura inclou els noms de tots els subscriptors implicats així com informació precisa sobre les mesures.

**Per a gestionar els retornats** (posar a cero els errors d'alguns subscriptors, donar de baixa els subscriptors inaccesibles, demana un recordatori de subscripció, etc.), **aneu a la pàgina «[Retornats](admin.md#manage_bounces)»** del mòdul d'administració de la llista.

**Atenció: no oblideu fer clic en el botó «Actualitzar»** al final de la pàgina per a desar tots els canvis.

### <span id="other"></span>Miscel·lània

L'opció «**Tasca periòdica de venciment periòdica de la subscripció**» permet definir **una data límit de venciment de les subscripcions** per a la llista: de manera regular (exemple: una vegada a l'any), els subscriptors rebran un missatge que els demanarà que renoven la subscripció. Si no ho fan, se'ls donarà de baixa automàticament. Aquest procediment garanteix que tots els subscrits a la llista es preocupen i s'interessen per la llista.

L'opció «**Tasca periòdica de recordatoris de subscripció**» permet **enviar recordatoris de subscripció** a la llista de manera regular.

L'opció «**mètode de protecció d'adreces de correu**» garanteix que els robots generadors de correu brossa no puguen arreplegar les adreces dels subscriptors. Aquesta opció s'aplica a totes les pàgines de la llista.

En aquesta pàgina, també podeu veure **informació sobre l'última actualització de la llista** (qui la va fer i quan), així com el **nombre de canvis de configuració** des què es va crea la llista.

**Atenció: no oblideu fer clic en el botó «Actualitzar»** que apareix en la part de sota de la pàgina per a desar els canvis.
