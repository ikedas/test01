Eposta zerrendak - Erabiltzaile gida
------------------------------------

### <span id="howitworks"></span>Nola dabil eposta zerrenden zerbitzua

Eposta zerrendaren zerbitzua **Sympa eposta zerrenda softwareak** kudeatzen du. Software hau **eposta zerrenden web ingurunearekin** dator.

**Eposta zerrendekin erlazionatutako ekintzak burutzeko** (harpidetu, zure aukerak aldatu, etab.) bi aukera dituzu:

-   **web ingurunean izena eman**;
-   Sympa eposta zerrenden kudeatzaileari **komandoak epostaz bidali** **{{conf.email}}@{{conf.host}}** helbidean.

**Sympari komando bat bidaltzeko** ondokoa egin:

-   **Komando bakarra bidaltzen baduzu**, idatzi komandoa zure epostaren gaian eta utzi edukia hutsik.
-   **Komando sorta bidaltzen badituzu**, utzi zure epostaren gaia hutsik eta idatzi komandoak epostaren gorputzean. **Kontuz**: Sympak ez du zure eposta prozesatuko ondoko erregelak betetzen ez badituzu:
    -   Idatzi komando bakoitza lerro batean.
    -   Mezua testu hutsean bidali, ez HTML formatuan.
    -   Mezuak komandoak baino ez ditu eduki behar (sinadurarik ez).

Sympari bidali ahal dizkiozun komando guztien deskribapena [file:///help/mail\_commands](mail_commands.md) helbidean dago.

### <span id="subscribe"></span>Eposta zerrendetara harpidetzen

Eposta zerrendara harpidetzea oso sinplea da:

1.  **Hautatu helbide bat**, zerrenda harpidetzeko erabiliko duzuna.

    | Note |
    |------|
    | Askotan begiratu ahal duzun helbide bat izan beharko luke, eta epostak gordetzeko leku handia duena: zerrenda batzuk mezu asko bidaltzen dituzte, hauetako batzuk eranskin handiekin. |

    | Note |
    |------|
    | Eposta zerrenda batera helbide bat baino gehiagorekin harpidetu zaitezke, noski. Helbide bakoitzeko prozesu osoa berregin beharko duzu orduan. |

2.  Zerrendara harpidetu nahi duzun helbidetik bidali **mezua {{conf.email}}@{{conf.host}} helbidera**.

    | Note |
    |------|
    | Sympa ez da pertsona bat, eposta zerrenden kudeaketa robot bat baizik. Ez ditu hitz maitagarririk behar! ;-) |

3.  Zure mezuaren gaian **subscribe zerrendarenizena LehenIzena Izena** idatzi (aldatu 'zerrendarenizena' harpidetu nahi duzun zerrendaren izenagatik eta adierazi zure izena eta lehen abizena).
4.  **Utzi mezuaren gorputza hutsik**.

    | Note |
    |------|
    | Denbora apur bat aurrezteko, komando multzoa bidali ahal duzu mezu bakarrean. Horretarako, jarraitu [Nola dabil eposta zerrenden zerbitzua](#howitworks) ataleko instrukzioak. |

**Honen ondoren mezu bat jasoko duzu zure eskaera onartua izan den edo ez esanez**: zerrendarako harpidetzak oniritzia behar badu, zerrendaren jabeak zu ez harpidetzea erabaki dezake. Honelakoetan ez bidali eskaera gehiago: ez du ezertarako balio erantzun berdina izango duelako. Zerrendaren jabearekin zuzenean kontaktuan jar zaitezke (zerrendarenizena-request@{{conf.host}}) zergatik harpidetu nahi zaren azaltzeko...

| Note |
|------|
| Oharra: batzutan zure harpidetza eskaeraren baieztapena eskatuko zaizu prozesatu baino lehen. Horrelakoetan jasotzen duzun mezuan esaten duena jarraitu. |

Zerrenda motaren arabera (harpidetzarako baldintzak dituzten zerredak eta ez dituztenak) eta zerrendaren jabearen eskuragarritasunaren arabera, **baliteke oharra berehala ez jasotzea**. Eskaera asko bidaltzeak ez du ezertarako balio.

**Zure eskaera onartzen bada, harpidetza konfirmatzen duen mezua jasoko duzu. Mezu hau** (zerrendaren arautegia) **ezinbesteko informazioa du:**

-   zure **zerrendako pasahitza**. Pasahitz hau eposta helbide berdinarekin harpidetu zaren zerrenda guztietan berdina izango da. [Web bidez aldatu](#global_pref "Nola aldatu zure pasahitza") dezakezu, eposta zerrenden ingurunean izena eman ondoren;
-   **zerrendaren inguruko informazio zehatza**: bere betekizuna, mezuen artxiboaren Interneteko helbidea, etab.
-   **zerrenda eta bere kideek bete beharreko arauak**: onartutako eta debekatutako mintzagaiak, netiketa, informazio legala, pribatutasun politika, etab.

**Zure harpidetzaren oharra gorde beharko zenuke**: baliteke geroago behar izatea zure pasahitza gogoratzeko edo Sympari komando jakin bat bidaltzeko (adibidez, ez-harpidetza komandoa). Orokorrago, **eposta zerrendetako harpidetzen ohar guztiak gordetzea gomendatzen dugu**.

**Zerrenda batera web bidez ere harpidetu zaitezke** ondoko pausuak jarraituz:

1.  Zerrenda ingurunearen **[hasiera orrira](%7B%7Bpath_cgi%7D%7D/home)** joan eta **izena eman**.
2.  Harpidetu nahi duzun **zerrendaren informazio orrira joan**.
3.  Ezkerreko menuak, **klikatu 'Harpidetu'** estekan.

### <span id="sympa_auth"></span>Eposta zerrenden ingurunean izena ematen

Eposta zerrenden ingurunean izena emateko, web interfazearen goi ezkerraldean agertzen den autentifikazio formularioa erabili. Izena emanda duzunean zure eposta helbidea eta erabiltzaile profila (harpidedun, moderatzaile edo jabea) ikusiko dira bertan.

Autentifikazio prozesua zure egoera pertsonalaren arabera aldatzen da:

-   **Eposta zerrenden zerbitzua eskaintzen duen erakundeak SSO teknologia erabiltzen badu** (kontu eta autentifikazio bakarra, CAS sistemarekin adibidez) zure kontu bakarrarekin izen ematea nahiagoko duzu. Horretarako, klikatu '**\[Erabilitako sistemaren izena\] autentifikazioa**' testuaren ondoko 'Joan' botoia. Ondoren idatzi zure erabiltzaile izen eta pasahitza autentifikazio zerbitzarian izena emateko.

    | Note |
    |------|
    | Zure autentifikazio sistema bakarra erabiliz beste zerbitzu batean izena eman baduzu zure autentifikazioa automatikoa da, Orria birkargatu beharrezkoa bada. |

-   **Autentifikazio bakarreko sistemak ez badizu eragiten, zure zerrendako pasahitza erabili dezakezu.** Kasu honetan betiko moduan izena eman: sartu **zerrendara harpidetzeko erabili zenuen eposta helbidea** erabiltzaile izen bezala eta **zerrendako pasahitza** 'Pasahitza' eremuan.

    | Note |
    |------|
    | Ez baduzu zure zerrendako pasahitza gogoratzen, klikatu 'Pasahitza galduta?'-n. Zure eposta helbidea eman ondoren mezu bat bidaliko zaizu helbide horretara baieztapen URL batekin. |

-   **Autentifikazio bakarreko sistemak ez badizu eragiten eta oraindik zerrendako pasahitza ez baduzu** sakatu '**Lehen izen ematea?**' eta idatzi zure eposta helbidea. Baieztapen URL bat bidaliko da helbide horretara. Orduan zure pasahitza aukeratu ahalko duzu.

| Note |
|------|
| Gogoratu: zerrendako pasahitza berezia da eta eposta zerrenden ingurunean bakarrik erabiliko duzu. |

### Zure harpidetzak egiaztatzen

Harpidetu zaren zerrenda guztiak ikusteko lehenbizi [izena eman](#sympa_auth) behar duzu. Ondoren ezkerreko zutabeko 'Zure zerrendak' formularioan zure zerrenda guztien zerrenda bistaratuko da, bakoitzaren deskribapen labur batekin.

**Zerrenda baten informazio orrira joateko klikatu bere izenean**. Informazio orrian zerrendaren deskribapena (izaera, mezuak bidaltzean bete beharreko arauak, etab.) dago, bere luzera zerrendaren araberakoa da.

Informazio orri honetan honakoak egin ahal dituzu:

-   zure [harpidetza aukerak](#options) aldatu;
-   [zerrendako artxiboa](arc.md) irakurri;
-   [zerrendako artxiboan bilatu](arc.md#arcsearch);
-   [mezu berriak bidali](sendmsg.md);
-   partekatutako dokumentuen web ataletik [dokumentuak deskargatu](shared.md#shared_read);
-   partekatutako dokumentuen atalera [dokumentuak igo](shared.md#shared_upload);
-   zerrendako [kideak aztertu](#subscribers) (eskuragarri badago);
-   zerrenda bakoitzeko harpidetza [baja edo alta eman](suspend.md);
-   zerrendatik [ez-harpidetu](#unsubscribe).

<span id="subscribers"></span>Zerrendara **harpidetutakoen kopurua** beti ikusgai dago **ezkerreko menuan**. **Kideen zerrenda aztertzeko klikatu 'Kideak aztertu' estekan**, ezkerreko menuan (zerrendaren jabeak kideen zerrendara atzipena ukatzen badu esteka hau ez da egongo). Kideen zerrendan harpidedun bakoitzaren **eposta helbidea** eta **izena** ikusten dira (izenaren adierazpena harpidedunek erabilitako harpidetza moduaren araberakoa da).

| Note |
|------|
| Defektuz, orri bakoitzak 25 harpidedun erakusten ditu. Orriak nabigatu ahal dituzu nabigatzeko geziak erabiliz edo orrian harpidedun gehiago erakuts ditzakezu. Harpidedunak eposta helbideagatik, domeinuagatik edo izenagatik ordenatu ahal dituzu dagokion zutabearen goiburuan klikatuz. |

**Ezkerreko menuan zerrendaren jabe eta moderatzaileen zerrenda ikusten da**. Ez zenuke inoiz zerrendako jabe edo moderatzaileei zuzenean idatzi behar. Galdera edo iruzkin bat egin nahi baduzu ondoko helbidea erabili beharko zenuke: **zerrendarenizena-request@{{conf.host}}** (aldatu 'zerrendarenizena' dagokion zerrendaren izenarekin).

**Zerrendara noiz harpidetu zinen** eta **zure harpidetzaren aukerak aldatu zenuen azkeneko aldia** zein den jakiteko, ezker menuko **'Harpidetza aukerak' klikatu**.

### <span id="pref"></span>Zure hobespenak kudeatzen

**Zerrenda erosoago erabiltzeko**, **hobespen pertsonal batzuk definitu ditzakezu**. Bi hobespen mota aldatu ditzakezu:

-   zure **harpidetza aukerak**, zerrenda bakoitzeko aldatu daitekeena;
-   zure **hobespen orokorrak**, Sympa eposta zerrenden ingurune osoari eragiten dietena.

#### <span id="options"></span>Zure harpidetza aukerak aldatzen

**Zure harpidetza aukerak zerrenda batetik bestera aldatu daitezke**. Aldatzeko ondokoa egin:

1.  Zerrenda ingurunearen **[hasiera orrira](%7B%7Bpath_cgi%7D%7D/home)** joan eta **izena eman**.
2.  Harpidetza aukerak aldatu nahi dizkiozun **zerrendaren informazio orrira joan**.
3.  Ezkerreko menuan, **klikatu 'Harpidetza aukerak' estekan**.
4.  <span id="deliverymode"></span>**Mezu bidalketa mota bat hautatu** (aukera hauetako bat bakarrik hautatu dezakezu):
    -   **MIME formatuko bilduma**: zerrendako mezuak normal jaso beharrean, periodikoki mezuen bildumak jasoko dituzu. Bilduma hauetan zerrendako mezu multzo bat dago, multipart/digest MIME formatuan. Bildumaren maiztasuna zerrendako jabeak ezartzen du.
    -   **testu soileko bilduma**: zerrendako mezuak normal jaso beharrean, periodikoki mezuan bildumak jasoko dituzu. Bilduma hauetan zerrendako multzo bat dago, test soilean. Bildumaren maiztasuna zerrendako jabeak ezartzen du.
    -   **laburpen modua**: zerrendako mezuak normal jaso beharrean, periodikoki mezuen zerrendak jasoko dituzu. Mezuak irakurtzeko web artxiboa nabigatu beharko duzu.
    -   **albiste modua**: modu honetan mezu guztien gorputzak hutsik jasoko dituzu: modu honetan bidaltzen diren mezu guztiak denbora errealean jarraitu ahalko dituzu posta kutxa beteko beldurrik gabe.
    -   **epostarik ez (oporretarako erabilgarria)**: modu honetan ez duzu zerrendako mezurik jasoko. Denbora luzean epostara sartu ezin zarenean erabilgarria batez ere, zerrendarako harpidetza mantenduz.
    -   **testua bakarrik modua**: modu honetan bi moduetan bidaltzen diren mezuen testu hutseko bertsioa jasoko duzu bakarrik (testu solia eta HTML).
    -   **HTML bakarrik modua**: modu honetan bi moduetan bidaltzen diren mezuen HTML bertsioa (text/html) jasoko duzu bakarrik.
    -   **url bihurtu modua**: modu honetan ez dituzu eranskinak jasoko. Dokumentu hauek zerrendako artxiboan daude eskuragarri eta mezuan eskaintzen diren URLen bidez atzitu ahalko dituzu.
    -   **ez jazo zure mezuak**: modu honetan ez duzu zuk bidalitako mezuen kopiarik jasoko.
    -   **estandarra (zuzenean jaso)**: hau da defektuzko bidalketa modua; beste edozein bidalketa modu ezeztatzen du.
    -   **bajan**: modu honetan zure harpidetza bajan eman ahal duzu denbora tarte jakin baterako edo ez. Ez-harpidetzearekin ez bezala zure harpidetzen jarraipena egin ahal duzu eta edozein momentutan alta eman ahal duzu "Zure harpidetzak kudeatu" atalean.
5.  **Ikusgaitasun aukera bat hautatu**:
    -   **berrikuspen zerrendan zerrendatu**: zure izena eta eposta helbidea kideen zerrendan agertuko da (zerrendaren jabeak harpidedunei kideen zerrenda ikusteko baimena ematen badie).
    -   **ezkutatuta**: zure izena eta eposta helbidea ez dira kideen zerrendan agertuko. Hala ere mezuak bidaltzen badituzu zerrendako artxiboan zure eposta helbidea ikusi ahalko da.
6.  **Klikatu 'Eguneratu' botoian**.

#### <span id="global_pref"></span>Zure hobespen orokorrak aldatzen

Hobespen orokorrak zure harpidetza guztietara aplikatzen zaie eta baita Sympa eposta zerrenden web interfazea nola bistaratuko modura. Zure hobespenak aldatzeko ondokoa egin:

1.  Zerrenda ingurunearen **[hasiera orrira](%7B%7Bpath_cgi%7D%7D/home)** joan eta **izena eman**.
2.  Goi ezkerraldean agertzen den formularioan **'Zure hobespenak' estekan klikatu**.
3.  **Zure hobespenak aldatu**.
4.  Aldatzen duzun **aukera bakoitzeko 'Bidali' klikatu**.

Aldatu ahal duzu:

-   zure **izena**; zerrenda batera eposta zerrenden zerbitzariko webetik harpidetzen zarenean 'Izena' eremua automatikoki beteko da kideen zerrendan;
-   **Symparen web interfazeak erabiltzen duen hizkuntza** (web interfazeko edozein orritan aldatu ahal duzu hizkuntza; zure aukera mantenduko da 'Hobespenak' ez den beste orriren batean hizkuntza aldatzen baduzu ere;
-   **Sumpak zure ordenagailuan jartzen duen cookie-aren biziraupena** ('Konexio irauntze tartea'). Defektuz, saioa nabigatzailea ixten duzunean bukatzen da; eposta zerrenden zerbitzua asko erabili behar baduzu tarte luzeagoa hautatzea gomendatzen dizugu;

    | Note |
    |------|
    | Cookie bat web zerbitzari batek zure disko gogorrean gordetzen duen fitxategi txiki bat da, gehienetan tenporala, zu zerbitzuaren erabiltzaile bezala identifikatzeko. Zuri buruzko informazio pertsonal apurrak ditu: izena, eposta helbidea, azken saio hasiera, etab. |

-   zerrendetara **harpidetzeko erabiltzen duzun eposta helbidea** (eposta helbide bat baino gehiagorekin harpidetu bazara, aldatuko den helbidea saioa hasteko erabili duzuna izango da);

    | Note |
    |------|
    | Kontuz: honek zure zerrenda guztietako harpidetzak aldatuko ditu. Zerrenda bakar baterako helbidea aldatu nahi baduzu, hobe zerrenda horretatik ez-harpidetu eta gero berriro eposta helbide egokiarekin harpidetzen bazara. |

-   zure **zerrendako pasahitza**.

'**Zure beste eposta helbideak**' atalak eposta helbideak aldatzen ditu.

### Eposta zerrenda bat bilatzen

Eposta zerrenda bat bilatu behar duzunean hiru aukera dituzu:

-   [zerrenda ingurunearen hasiera orriak](%7B%7Bpath_cgi%7D%7D/home) agertzen diren **atal ezberdinak nabigatu**;
-   **bilaketa kutxa** erabiliz zerrenda bat bilatu: bilatzen duzun testua izen edo deskribapenean duten zerrenda guztiak itzuliko ditu (deskribapenak normalean esaldi motzak izan ohi dira);
-   klikatu orriko goialdean dagoen '[Zerrenden zerrenda](%7B%7Bpath_cgi%7D%7D/lists)' **eskuragarri dauden zerrenda guztiak ikusteko**

| Note |
|------|
| Zure epostaren domeinuaren arabera (adibidez: *cru.fr*, *fai.com*, etab.) eta izena ematen duzun kokapenaren arabera ikusten duzun zerrenda ezberdina izango da. Agertzen ez den zerrenda batera harpidetu zaitezke bere izena badakizu. Horretarako [erabili zure posta bezeroa](#subscribe). |

### <span id="archives"></span>Zerrendako artxiboa webean irakurtzen

Irakurri [**artxiboaren dokumentazioa**](arc.md) mesedez.

### <span id="sendmsg"></span>Mezua bidaltzen

Irakurri [**mezuen bidalketarako dokumentazioa**](sendmsg.md) mesedez.

### <span id="shared"></span>Partekatutako dokumentuen web atala erabiltzen

Irakurri [**partekatutako dokumentuen web atalaren dokumentazioa**](shared.md) mesedez.

### <span id="suspend"></span>Zerrenda bakoitzaren harpidetza baja edo alta ematen

Irakurri [**harpidetzen kudeaketaren dokumentazioa**](suspend.md) mesedez.

### <span id="unsubscribe"></span>Zerrendatik ez-harpidetzen

Zerrenda batetik ez-harpidetzeko ondokoa egin:

1.  Harpidetzeko erabili zenuen helbidetik **mezua bidali {{conf.email}}@{{conf.host}}-era**.
2.  Mezuaren gaian idatzi: **unsubscribe zerrendaizena** (zerrendaizena ez-harpidetu nahi duzun zerrendaren izenaz aldatu).
3.  **Utzi mezuaren gorputza hutsik**.

    | Note |
    |------|
    | Denbora apur bat aurrezteko, komando multzoa bidali ahal duzu mezu bakarrean. Horretarako, jarraitu [Nola dabil eposta zerrenden zerbitzua](#howitworks) ataleko instrukzioak. |

Zerrendaren web interfazetik ere ez-harpidetu zaitezke (ez-harpidetu nahiduzun zerrenda bakoitzeko egin beharko duzu):

1.  Zerrenda ingurunearen **[hasiera orrira](%7B%7Bpath_cgi%7D%7D/home)** joan eta **izena eman**.
2.  Ez-harpidetu nahi duzun **zerrendaren informazio orrira joan.**
3.  **Ezkerreko menuan, sakatu 'Ez-harpidetu' estekan**.

------------------------------------------------------------------------
