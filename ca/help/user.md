Llistes de correu - Guia de l'usuari
------------------------------------

### <span id="howitworks"></span>Com funciona el servei de llistes de correu

El servei de llistes de correu es gestiona amb un **programari de llistes de correu: Sympa**. Aquest programari inclou un **entorn web de llistes de correu**.

**Per fer accions relacionades amb les llistes de correur** (subscriure's, canviar les opcions, etc.), n'hi ha dues opcions:

-   **iniciar la sessió en l'entorn web**;
-   **enviar ordres per mail** al gestor de la llista de correu de Sympa**{{conf.email}}@{{conf.host}}**.

**Per enviar ordres a Sympa**, s'han de seguir les passes següents:

-   **Si només s'envia una ordre**, escriviu-la en l'assumpte del correu i deixeu el cos en blanc.
-   **Si s'envien diverses ordres**, deixeu l'assumpte en blanc i escriviu totes les ordres en el cos del correu. **Atenció**: Sympa no processarà el missatge si no es respecten les nomes següents:
    -   Escriviu cada ordre en una línia nova.
    -   Envieu el missatge en text net, no en HTML (sense format).
    -   El missatge no pot contenir res més que ordres de Sympa (no ha de portar un bloc de signatura).

Podeu trobar una descripció de totes les ordres que es poden enviar a Sympa en [file:///help/mail\_commands](mail_commands.md).

### <span id="subscribe"></span>Com subscriure's a una llista de correu

Subscriure's a una llista de correu es molt fàcil:

1.  **Elegiu l'adreça** amb què us voleu subscriure a la llista.

    | Note |
    |------|
    | Heu d'elegir una adreça electrònica que reviseu amb freqüència i que tinga una gran capacitat d'emmagatzematge: algunes llistes distribueixen molts missatges, que de vegades inclouen documents adjunts grans. |

    | Note |
    |------|
    | No cal dir que us podeu subcriure a una mateixa llista amb diferents adreces. Aleshores, haureu de refer tot el procés amb totes les adreces. |

2.  Envieu un **missatge a {{conf.email}}@{{conf.host}}** des de l'adreça amb què us voleu subscriure a la llista.

    | Note |
    |------|
    | Sympa no és una persona, sinó un robot de gestió de llistes de correu. De manera que és inútil enviar-li paraules afectuoses! ;-) |

3.  En l'assumpte del missatge, escriviu: **subscriure's nomdelallista Nom Cognoms** (canvia «nomdelallista» pel nom de la llista al què us voleu subscriure i indiqueu el nom i els cognoms).
4.  **Deixeu el cos del missatge en blanc**.

    | Note |
    |------|
    | Per estalviar temps, també podeu enviar diverses ordres en un únic missatge. Per fer-ho, seguiu les instruccions de la secció [Com funciona el servei de llistes de correu](#howitworks). |

**Després d'això, rebreu un missatge que us comunicarà si s'ha acceptat o no la sol·licitud**: si la subscripció a la llista està subjecta a qualsevol mena d'aprovació, el propietari de la llista pot optar per no subscriure-us. Si passa això, no envieu més sol·licituts: és inútil ja que el resultat serà el mateix. Podeu enviar un missatge directament al propietari de la llista (nomdelallista-request@{{conf.host}}), per explicar-li per què voleu de veritat subscriure-us a la llista...

| Note |
|------|
| Nota: de vegades us demanaran que confirmeu la sol·licitut de subscripció abans que es pugui processar. Si és així, seguiu les instruccions que inclou el missatge que heu rebut. |

Segons el tipus de llista (si la subscripció està sotmesa o no a unes condicions) y de la disponibilitat del propietari de la llista, **és possible que no rebeu l'avís de seguida**. És inútil enviar més sol·licituts.

**Si s'accepta la sol·licitud, el missatge que rebreu confirmarà la subscripció a la llista. Aquest missatge** (les normes de funcionament) **conté informació bàsica:**

-   la **contrasenya de la llista**. Aquesta contrasenya és la mateixa per a totes les llistes a què us subscriviu amb la mateixa adreça electrònica. Podeu [canviar-la en línia](#global_pref "Com canviar la contrasenya") després d'iniciar la sessió en l'entorn de la llista de correu;
-   **informació detallada sobre la llista**: propòsits, adreça d'Internet en què està disponible l'arxiu del missatge, etc.
-   **normes sobre la llista i els membres**: temes permesos i prohibits, etiqueta web, informaciò legal, política de privadesa, etc.

**Heu de guardar la notificació de subscripció**: és possible que més tard necessiteu recordar la contrasenya o enviar una ordre precisa a Sympa (per exemple: l'ordre de desactivar). En general, **us recomanem que guardeu totes les notificacions de subscripció a llistes de correu**.

**També podeu subscriure-us a una llista des de la interfície de la llista de correu**. Per ha fer-ho, heu de seguir els passos següents:

1.  Aneu a l'entorn de la llista **[pàgina inicial](%7B%7Bpath_cgi%7D%7D/home)** i **inicieu sessió**.
2.  **Aneu a la pàgina d'informació de la llista** a què us voleu subscriure.
3.  En el menú de l'esquerra, **feu clic en l'enllaç de «Subscriure's»**.

### <span id="sympa_auth"></span>Inicieu sessió en l'entorn de la llista de correu

Per a iniciar sessió en l'entorn de la llista de correu, empreu el formulari d'autenticació que es veu al damunt de la columna de l'esquerra de la interfície web. Quan hageu iniciat la sessió, hi veureu la vostra adreça del correu electrònic i el perfil d'usuari (subscriptor, moderador o propietari).

El procés d'autentificació canviar segons la situació personal:

-   **Si l'organització que ofereix el servei de llistes de correu empra tecnologia d'activació única** (un únic compte i una única autenticació, per exemple el sistema SAC), és millor que entreu amb el compte únic. Per a fer-ho, feu clic en el botó de «Vés» que està al costat del text «**Autenticació \[nom del sistema emprat\]**». Aleshores, escriviu el nom d'usuari i la contrasenya per a iniciar sessió en el servidor d'autenticació.

    | Note |
    |------|
    | Si ja heu iniciat sessió en un altre servidor emprant el sistema d'autenticació únic, l'autenticació és automàtica. Actualitzeu la pàgina si és necessari. |

-   ~~**If the unique authentication process does not apply to you, you can use your list password.** In this case, log on through the classic method: enter the **email address with which you subscribed to the list** as a login and your **list password** in the 'Password' field.~~

    | Note |
    |------|
    | ~~If you do not remember your list password, click on 'Lost password?'. After you've provided your email address, a mail with a validation URL will be sent at that address.~~ |

-   ~~**If the unique authentication process does not apply to you and you do no have a list password yet**, click on '**First login?**' and type in your email address. A confirmation URL will be sent at that address. Then you will be able to choose your password.~~

| Note |
|------|
| Recorda: la contrasenya de la llista és una contrasenya especial que només emprareu per al servei de llistes de correu. |

### Com comprovar les subscripcions

Per a veure totes les llistes en què us heu subscrit, primer de tot, necessiteu [iniciar sessió](#sympa_auth). Aleshores, en l'opció «Les vostres llistes» de la columna de l'esquerra, apareixerà una llista amb totes les llistes en què us heu subscrit, amb una petita descripció de cadascuna.

**Per a mirar en la pàgina d'informació d'una llista , feu clic en el nom**. La pàgina d'informació inclou una descripció de la llista (objectiu, normes per enviar missatges, etc.), que té una grandària diferent segons la llista.

Des d'aquesta pàgina d'informació, podreu:

-   canviar les [opcions de subscripció](#options);
-   llegir els [arxius de la llista](arc.md);
-   [cercar en l'arxiu dels missatges](arc#arcsearch.md);
-   [enviar nous missatges](sendmsg.md);
-   [baixar-se documents](shared#shared_read.md) de l'espai web per a compartir documents;
-   [carregar documents](shared#shared_upload.md) en l'espai compartit de documents del web;
-   [veure els membres](#subscribers) de la llista (si l'opció està disponible);
-   ~~[suspend or resume](suspend.md) your subscription of each list;~~
-   [donar-se de baixa](#unsubscribe) de la llista.

<span id="subscribers"></span>El **nombre de subscriptors** de la llista es pot veure sempre en el **menú de l'esquerra**. **Per veure la llista de membres, aneu al menú de l'esquerra i feu clic en l'enllaç «Veure membres»** (si el propietari de la llista ha decidit denegar l'accés a la llista de membre, l'enllaç no estarà disponible). La llista de subscriptors mostra l'**adreça electrònica** i el **nom** de cada subscriptor (la manera com aparèixen els noms dependrà del métode de subscripció).

| Note |
|------|
| Cada pàgina mostra per defecte 25 subscriptors. Es pot navegar per les pàgines emprant les fletxes de navegació o l'opció de mostrar més subscriptors per pàgina. També es poden ordenar els subscriptors per l'adreça electrònica, el domini o el nom fent clic en la capçalera de la columna corresponent. |

**Els noms dels propietaris de la llista i dels moderadors es poden veure en el menú de l'esquerra**. No heu d'escriure mai directamenta als propietaris o moderadors de la llista. Si voleu fer una pregunta o un comentari, heu d'emprar l'adreça següent: **nomdelallista-sol·licitud@{{conf.host}}** (canvia «nomdelallista» pel nom de la llista a què fa referència el missatge).

Per saber **quan us vau subscriure a la llista** i **l'última vegada que vau actualitzar les opcions de subscripció**, heu d'anar al menú de l'esquerra i **fer clic en l'enllaç d'«Opcions de subscripció»**.

### <span id="pref"></span>Com gestionar les preferències

Per a poder **emprar les llistes amb facilitat**, **heu de definir una sèrie de preferències personals**. Hi ha dos classes de preferències que podeu canviar:

-   les **opcions de subscripció**, que poden canviar segons la llista;
-   les **preferències generals**, que afecten tot l'entorn de les llistes de correu de Sympa.

#### <span id="options"></span>Com canviar les opcions de subscripció

**Les opcions de subscripció poden canviar d'una llista a una altra**. Per canviar-les, segueix els passos següents:

1.  Aneu a l'entorn de la llista **[pàgina inicial](%7B%7Bpath_cgi%7D%7D/home)** i **inicieu sessió**.
2.  **Aneu a la pàgina d'informació de la llista** en què voleu canviar les opocions de subscripció.
3.  En el menú de l'esquerra, **feu clic en l'enllaç «Opcions de subscripció»**.
4.  <span id="deliverymode"></span>**Elegiu una modalitat d'entrega dels missatges** (aquestes opcions són excloents, és a dir, no es pot elegir més d'una):
    -   **recopilatori en format MIME**: en comptes de rebre els missatges de manera habitual, rebreu un recopilatori d'aquests regularment. Aquest recopilatori compila un grup de missatges de la llista, mitjançant el format multipart/digest MIME. La freqüència dels recopilatoris, l'estableix el propietari de la llista.
    -   **format de text net del recopilatori**: en comptes de rebre els missatges de la llista de manera habitual, rebreu un recopilatori d'aquests regularment. Aquest recopilatori compila un grup de missatges de la llista en format de text net. La freqüencia dels recopilatoris, l'estableix el propietari de la llista.
    -   **modalitat resum**: en comptes de rebre els missatges de la llista de manera habitual, rebreu una llista d'aquests regularment. Per a llegir els missatges, haureu d'anar a l'arxiu en línia de la llista.
    -   **modalitat notícies**: amb aquesta modalitat, rebreu tots els missatges amb el cos en blanc: d'aquesta manera estareu informat de tots els missatges enviats a la llista en temps real, sense el risc què s'inunde la safata d'entrada.
    -   **no vull rebre correus (útil per a les vacances)**: aquesta modalitat fa que no rebeu missatges de la llista. És útil, sobretot, quan no podeu accedir al correu electrònic durant un temps prolongat i, tot i això, voleu seguir subscrits a la llista.
    -   **només en text**: aquesta modalitat permet rebre només la versió en text (text net) dels missatges que s'envien en els dos formats (text net i HTML).
    -   **només en format HTML** : aquesta modalitat permet que només rebeu la versió en HTML (text en html) dels missatges que s'envien en els dos formats.
    -   **modalitat URL**: aquesta modalitat permet no rebre documents adjunts. Tot i això, aquests documents estan disponibles en l'arxiu de la llista i en podeu accedir a través d'una URL que apareixerà en el missatge.
    -   **no vull rebre els meus missatges**: aquesta modalitat permet no rebre una còpia dels missatges que hageu enviat.
    -   **estàndard (recepció directa)**: aquesta és la modalitat d'entrega per defecte; això cancel·la qualsevol altra modalitat.
    -   ~~**suspended**: this mode allows you to suspend your subscription to one or more lists for a specified period or not. Unlike unsubscription, you can keep track of your subscription and reactivate it at any time by visiting the "Manage your subscription" section.~~
5.  **Com elegir una opció de visibilitat**:
    -   **aparèixer en la pàgina de revisió de llista**: apareixerà el vostre nom i adreça electrònica en la llista de membres (si el propietari de la llista permet que els subscriptors revisen la llista de membres).
    -   **ocult**: no apareixerà el vostre nom ni l'adreça electrònica en la llista de membres. Tot i això, sí que apareixeran en l'arxiu de la llista si envieu missatges.
6.  **Feu clic en el botó «Actualitzar»**.

#### <span id="global_pref"></span>Com canviar les preferències generals

Les preferències generals afecten a totes les subscripcions i la manera en què es veu l'interfície web de les llistes de correu de Sympa. Per canviar-les, seguiu els passos següents:

1.  Aneu a l'entorn de la llista **[pàgina inicial](%7B%7Bpath_cgi%7D%7D/home)** i **inicieu sessió**.
2.  En la capçalera de la columna esquerra es veu un formulari, **feu clic en l'enllaç «Preferències»**.
3.  **Com canviar les preferències**.
4.  **Feu clic en «Trametre» per a totes les opcions** que canvieu.

Podeu canviar:

-   el **nom**; si us subscriviu a una llista des de la interfície web del servidor de llistes de correu, el camp «Nom» s'omplirà automàticament en la llista de membres;
-   la **llengua en què es mostra la interfície web de Sympa** (podeu canviar la llengua en totes les pàgines de la interfície web; la opció elegida es mantindrà tret que canvies la llengua de la interfície en la pàgina de «Preferències»;
-   el **temps de vida de les galetes que instal·la Sympa a l'ordinador** («Període de venciment de la connexió»). Per defecte, la sessió s'acaba quan es tanca el navegador, si empreu sovint el servei de llistes de correu, us recomanem que elegiu una duració més llarga;

    | Note |
    |------|
    | Una galeta es un arxiu petit que acumula un servidor web en el disc dur, en general de manera temporal, per què us indetifiqueu com a usuaris del servei. Conté unes poques dades d'informació personal: nom, adreça electrònica, la data de l'última vegada que vau iniciar sessió, etc. |

-   l'**adreça electrònica amb què us heu subscrit** a les llistes (si heu subscrit amb més d'una adreça electrònica, l'adreça que es pot canviar és amb la qual hageu iniciat la sessió);

    | Note |
    |------|
    | Aneu amb compte: aquesta acció canviarà les subscripcions de totes les llistes. Si només voleu canviar l'adreça per a una llista de correu, és millor que us doneu de baixa de la llista i us torneu a subscriure amb la nova adreça electrònica. |

-   la **contrasenya de la llista**.

La secció «**D'altres adreces electròniques**» funciona com un canvi de adreça electrònica.

### Cercar una llista de correu

Podeu necessitar cercar una llista de correu. Per fer-ho, teniu tres opcions:

-   **navegueu per les diferents seccions** que apareixen en [l'entorn de la pàgina principal de la llista](%7B%7Bpath_cgi%7D%7D/home);
-   cerque la llista a través del **quadre de cerca**: la cadena de cerca mostrarà totes les llistes el nom o la descripció de les quals coïncida amb els criteris que heu escrit (la descripció d'una llista normalment és una frase curta);
-   al començament de la pàgina, feu clic en la pestanya «[Llista de listes](%7B%7Bpath_cgi%7D%7D/lists)» per a **veure totes les llistes disponible**.

| Note |
|------|
| Segons el domini de l'adreça electrònica (per exemple: *cru.fr*, *fai.com*, etc.) i el lloc des què inicieu sessió, no tindreu accés a les mateixes llistes. Tot i això, us podeu subscriure a una llista que no aparega si en sabeu el nom. Per fer això, [empreu el vostre client de correu](#subscribe). |

### <span id="archives"></span>Com llegirun arxiu de la llista en línia

Aneu a [**documents de l'arxiu**](arc.md).

### <span id="sendmsg"></span>Com enviar un missatge

Aneu a [**documents sobre com enviar missatges**](sendmsg.md).

### <span id="shared"></span>Com emprar l'espai web per a compartir documents

Aneu a [**documents sobre l'espai web per a compartir documents**](shared.md).

### <span id="suspend"></span>~~Suspending or resuming your subscription of each list~~

~~Please refer to the [**subscription management documentation**](suspend.md).~~

### <span id="unsubscribe"></span>Com donar-se de baixa de les llistes

Per a donar-se de baixa d'una llista, seguie el passos següents:

1.  Des de l'adreça amb què us vau subscriure a llista, envieu un **missatge a {{conf.email}}@{{conf.host}}**.
2.  En l'assumpte del correu electrònica poseu: **donar-se de baixa nomdelallista** (canvieu «nomdelallista» per el nom de la llista de la qual us voleu donar de baixa).
3.  **Deixeu el cos del missatge en blanc**.

    | Note |
    |------|
    | Per estalviar temps, també podeu enviar diverses ordres en un únic missatge. Per fer-ho, seguiu les instruccions de la secció [Com funciona el servei de llistes de correu](#howitworks). |

També us podeu donar de baixa a través de la interfície web de la llista de correu (hauràs de repetir el mateix procés amb totes les llistes de les quals us voleu donar de baixa):

1.  Aneu a l'entorn de la llista **[pàgina inicial](%7B%7Bpath_cgi%7D%7D/home)** i **inicieu sessió**.
2.  **Aneu a la pàgina d'informació de la llista** de la qual us voleu donar de baixa.
3.  **En el menú de l'esquerra, feu clic en l'enllaç «Donar-se de baixa»**.

------------------------------------------------------------------------
