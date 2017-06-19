<span id="docadmin"></span>Eposta zerrendak - Jabe eta moderatzaileen gida
--------------------------------------------------------------------------

### Sarrera: zeinek du eposta zerrendak kudeatzeko ardura?

Oroigarria: eposta zerrendetan lau rol mota dago:

-   **zerrenda kudeatzailea;**
-   **jabea;**
-   **moderatzailea;**
-   **harpideduna.**

Begiratu [rol bakoitzeko deskribapena](introduction#roles.md) honi buruz gehiago jakiteko.

### <span id="create_list"></span>Eposta zerrenda bat sortzeko eskatzen

**Zerrenda sortzeko eskaera** bat **baldintzatua izan daiteke**. Baldintza horiek bete arren **zerrendaren sorrera** beti **zerrenda kudeatzaileek onartua** izan behar du.

Eposta zerrendaren sorrera eskatzeko ondokoa egin:

1.  Joan **[hasiera orrira](%7B%7Bpath_cgi%7D%7D/home)** eta [**izena eman**](user#sympa_auth.md).
2.  Goiko menuan **'Zerrenda sortu' esteka sakatu**.

    | Note |
    |------|
    | Esteka hori ez bada agertzen, zerrendak sortzeko baimenik ez duzula esan nahi du |

3.  Jarri **izena** zure zerrendari (izena bakarrik, '@' eta domeinurik gabe; adibidez: *hizkuntzak\_euskara* eta ez *hizkuntzak\_euskara@{{conf.host}}*).

    | Note |
    |------|
    | Ez erabili azentu, hutsune edo karaktere berezirik zerrenda izenetan, arazoak sortu ditzakete |

    | Note |
    |------|
    | Aukeratu esanguratsua eta motza den izena: pentsa zerrendara mezu bat bidali nahi duten bakoitzean harpidedunek izen hau idatzi beharko dutela! Zerrenda multzo bat kudeatzen badituzu aurrizki berdina jarri ahal diezu guztiei; horrela elkarrekin ordenatuko dira eta errazago antzemango dira (adibidez: *xx-erabiltzaileak@{{conf.host}}, xx-garatzaileak@{{conf.host}}*, etab.). |

4.  Aurredefinitutakoen artean **zerrenda mota** bat aukeratu (aurredefinitutako motak ohizko konfigurazioen adibideak baino ez dira, zerrenda sortu eta gero aldatu daitezkeenak; zerrenda kudeaketa moduluak eskaintzen dituen aukerez kanpo ere konfiguratu daiteke, zerrenda kudeatzaileei galdetuta).
5.  Zure zerrendaren **gaia** adierazi. Gai hau zerrendaren horri guztien goiburuan agertuko da eta ikusgai egongo da zerrenden indizeetan (zerrenden zerrendak, zuk harpidetutako zerrendak, etab.) eta nabigatzailearen izenburu barran.
6.  **Mintzagaiak** menuko **mintzagai** bat hautatu

    | Note |
    |------|
    | Mintzagai bat ere balio ez badizu, zerrenda kudeatzaileei mintzagai berrien sorrera eskatu ahal diezu. |

7.  Zure zerrendaren **deskribapena** adierazi. Deskribapen hau zerrendaren informazio orrian agertuko da, eta baina harpidedun berriei bidaliko zaien 'Harpidedunen Arautegia' epostan, 'Zerrendaren gaia' goiburuan. Deskribapen honek ondoko atalak landu ditzake:

    -   zerrendaren zergatia eta helburuak;
    -   landutako gaiak;
    -   zerrendaren funtzionamendua (ardurak, zerrendaren egoera, etab.);
    -   dauden erregelak;
    -   harpidedun arruntaren deskribapena (beraien lana, kudeatzen dituzten proiektuak, nazionalitateak, etab.).

    | Note |
    |------|
    | Zure deskribapenean HTML etiketak erabili ahal dituzu. Kontuz: zure deskribapena luzeegia bada hasi lerro berriak noizbehinka (teklatuko ENTER tekla sakatuta); bestela baliteke nabigatzailean osorik ez ikustea |

8.  Sakatu '**Sorrera eskaera bidali**' botoian.

Mezu bat agertuko da sorrera eskaera zerrenda kudeatzaileei bidali zaiela esateko eta hemendik aurrera zerrenda moldatu dezakezula bere 'Kudeaketa' botoian sakatuta. Hala ere mezuak ohartaraziko zaitu zerrenda ez dela benetan instalatuko eta ikusgai jarriko zerrenda kudeatzaile batek onartu arte.

Honen ondoren **zerrenda kudeatzaileek eskaera onartu harte** itxaron beharko duzu. Orduan **zerrendaizena zerrendaren sorrera** izenburudun mezu bat jasoko duzu, zerrenda dagoeneko sortuta dagoela esateko.

**Azkenik, harpidetu zure zerrendara**: zerrenda bat sortzeak edo bere jabe edo moderatzaile bihurtzeak ez du automatikoki harpidetuko zarenik esan nahi!

### Zerrenda kudeatzen

Zure zerrenda bat kudeatzeko ondokoa egin:

1.  Joan **hasiera orrira** eta **[saioa hasi](user#sympa_auth.md)**.

    | Note |
    |------|
    | Eposta bat baino gehiagorekin harpidetuta bazaude, erabili eporta sorrera eskaerarako erabili zenuena. |

2.  **Joan kudeatu nahi duzun zerrendaren informazio orrira joan**.
3.  Ezkerreko menuko **'Administrazioa' esteka sakatu**.

Administrazio moduluko atalak nabigatzeko sakatu 'Administrazioa' estekaren azpiko esteketan, ezkerreko menuan.

Atal ezbedin hauek ahalbidetzen dute:

-   [zerrenda konfiguratzea](listconfig.md);
-   [zerrendarekin erlazionatutako fitxategiak aldatzea](#customize);
-   [harpidedunak kudeatzea](#manage_members);
-   [zerrendako mezuen artxiboa kudeatzea](#manage_archives);
-   [erreboteak kudeatzea](#manage_bounces);
-   [partekatutako dokumentuen atala sortu, ezabatu edo kudeatzea](#manage_shared);
-   [zerrenda berrizendatzea](#renamelist);
-   [zerrenda ezabatzea](#supprlist).

'Moderatu' azpimenuko aukera ahalbidetzen dute:

-   zerrendara bidalitako [mezuak moderatzea](#moderate);
-   partekatutako dokumentuen web atalean atzigarri dauden [dokumentuak moderatzea](shared.md);
-   [egiteke dauden harpidetzak moderatzea](#manage_members).

#### <span id="edit_list"></span>Zerrenda konfiguratzen

Zerrenda nola konfiguratu ikasteko [**zerrenda konfigurazioari buruzko dokumentazioan**](listconfig.md) begiratu mesedez.

#### <span id="customize"></span>Zerrenda moldatzen

Orri honetan zure **zerrendarein erlazionatutako fitxategiak aldatu** ahal dituzu, besteen artean:

-   harpidedunei momentu jakinetan bidaltzen zaizkien mezuak:
    -   **harrera mezua**: mezu hau harpidetu berri direnei bidaltzen zaien oharra da. Zure zerrendaren arautegi bat idatzi beharko zenuke harrera mezu honetan. MIME egitura duen mezua sortu ahal duzu (MIME formatuan adituentzat);
    -   **ez-harpidetze mezua**: mezu hau zerrendatik ez-harpidetzen direnei bidaltzen zaie.
    -   **ezabatze mezua**: mezu hau zerrendatik ez-harpidetezen dituzunei (DEL komandoa) bidaltzen zaie, beraien helbideak erreboteak sortzen dituztenean bereziki;
    -   **mezu oroigarria**: mezu hau harpidedunei bidaltzen zaie REMIND komandoa erabiltzen denean. Komando hau zerrendaren kudeaketa egokirako ezinbestekoa da errebote asko erabiltzaileen oraingo helbidea harpidetzeko erabili zutena ez izateagatik, edo harpidetuta daudela ahazteagatik sorten direlako.
    -   **harpidetza gonbite mezua**: mezu hau INVITE komandoaren bidez harpidetzeko gonbidatu dituzunei bidaltzen zaie;
    -   **moderatzaileak mezua atzera botatzeko mezua**: mezu hau atzera botatako mezuaren bidaltzaileari bidaltzen zaio;
    -   **Birus-a izateagatik atzera botatakoan oharra**: mezu hau birusa topatu zaion mezuaren bidaltzaileari bidaltzen zaio.
-   bestelako fitxategiak:
    -   **zerrendaren deskribapena**: epostaz bidaltzen da INFO komandoaren erantzun moduan. Defektuz ongietorri mezuan (harpidetza oharran) ere txertatzen da. Ez da zerrendaren web interfazeko aurkezpen orrian agertzen denaren berdina
    -   **zerrendaren hasiera orria**: deskribapen hau zerrendaren informazio orrian ikus daiteke. HTML formatuan egon daiteke. Formatu hau erabiltzen ez baduzu ere, sartu `%lt;br />` etiketa lerro berriak hasteko;
    -   **mezuaren goiburua**: ahal denean MIME eranskin bezala txertatuko da zerrendara bidalitako mezuetan.
    -   **mezuaren oina:**: ahal denean MIME eranskin bezala txertatuko da zerrendara bidalitako mezuetan.

Sympak defektuzko fitxategiak erabiltzen ditu; hala bada zure zerrendako fitxategiak hutsik egongo dira. **Fitxategiren bat editatzeko, zerrendatik hautatu eta sakatu 'Editatu' botoian**. **'Nork'** eta **'Gaia** eremuak eta **mezuaren gorputza** aldatu ahalko dituzu.

| Note |
|------|
| Kontuz: Kortxete artean dauden balioak aldagaiak dira. Ez aldatu, egiten zaudenaz ziur ez bazaude. |

#### <span id="manage_shared"></span>Web-ean partekatutako dokumentuak kudeatzen

Defektuz, zerrendek ez dut partekatutako dokumentuentzako tokirik. Sortu beharko duzu, beraz. Horretarako **zerrendaren kudeaketa modulura** joan eta klikatu **Partekatua sortu** estekan.

Harpidedunak partekatutako dokumentuen web atalean argitaratu ahal izateko **defektuzko baimenak aldatu** behar dituzu: zerrenaren kudeaketa moduluan, klikatu '**Editatu zerrenda konfigurazioa**'n eta gero '**Baimenak**en. Orriaren behealdean '[**Zeinek edita dezake**](listconfig#docsrights.md) menu bat dago; hautatu '**harpidedunentzat mugatuta** aukera.

| Note |
|------|
| Kontuz, baimen hauek aldatu baino lehen karpeta batzuk sortzen badituzu idaztezin jarraituko dute. Bertan idaztea ahalbidetzeko karpeta bakoitzaren [change access rights](shared#acces.md) |

Agian kuotak esleitu nahiko dituzu partekatutako web atalentzako 'Baimenak' atalean 'Zerrendako konfigurazioa editatu' sekzioan

**Partekatutako web atalari buruz dena jakin nahi izanez gero** (nola antolatu, sarbide baimenak aldatu, dokumentuak izendatuetab.) Erabiltzaile liburuko 'Partekatutako web atala' kontsulta dezakezu

**Partekatutako web atalerako sarbidea ukatzeko**'Admin' azpimenuko **Partekatutakoa ezabatu** sakatu. Berriro **irekitzeko** **Partekatutakoa berrezarri**erabil dezakezu. Partekatutako web atalak borratu eta berrezartzeko ez du eraginik barnean dituzten dokkumentuetan.

#### <span id="manage_members"></span>Harpidedunak kudeatu

Atal honek **harpidedun guztien zerrenda** erakusten du.Harpidedun bakoitzeko, honako informazio dago eskuragarri:

-   **eposta helbidea**
-   Eposta helbidearen **domeinua** (*@cru.fr*, *@sympa.org*, *@fai.com*, etab.);
-   **irudia** (zerrendarako gaituta badago);
-   **izena** (harpidetza moduaren arabera batzutan ez da erakusten);
-   [**mezu bidalketa modua**](#deliverymode);
-   **datu iturria**, harpideduna zerrendara nondik txertatu den adierazteko, zuzenean harpidetu ez bada;
-   zerrendara **harpidetze data**;
-   harpidedunaren aukeren **azken eguneraketa**.

| Note |
|------|
| Defektuz, orri bakoitzak 25 harpidedun erakusten ditu. Orrien artean nabigatzeko geziak erabili ahal dituzu edo orri bakoitzean harpidedun gehiago erakutsi. Harpidedunak irizpide ezberdinen arabera ordenatu ahal dituzu baita ere, dagokion zutabearen goiburuan sakatuz. |

**Harpidedun bat bilatzeko**, bilaketa eremuan bere eposta edo izen osoa edo zati bat sartu, eta sakatu **Bilatu** botoia.

Orri honetatik **jendea zerrendara harpidetu** ahal duzu:

-   **Pertsona bakar bat** gehitzeko, sartu bere eposta helbidea sarrera eremuan eta **Gehitu** botoian sakatu.
-   **Pertsona batzuk** gehitzeko sakatu '**Asko gehitu**' botoian. Agertzen den sarrera eremuan sartu harpidetu nahi dituzunen eposta eta izenak eta sakatu **Harpidedunak gehitu**n.

| Note |
|------|
| Jendea ohartarazi gabe harpidetu nahi baduzu, sakatu 'Isila' botoia. Hala ere, askoz hobea da jendea harpidetu duzula adieraztea! |

Jendea zure eposta zerrendara harpidetu ahal duzun arren, **askoz hobea da jendeak harpidetzeko beharrezko pausuak ematen baditu bere kabuz**. INVITE komandoa erabiliz **jendea zerrendara harpidetzeko gonbidatu** ahal duzu ere bai: bidali eposta bat {{conf.email}}@{{conf.host}} helbidera eta mezuaren gorputzean ondokoa idatzi: **invite zerrendarenizena epostahelbidea** (adibidez: *invite adibideko\_zerrenda john.doe(@)fai.com*).

**zerrendarako harpidetza eskaera onartu edo atzera botatzeko** klikatu '**harpidetzak onartzeke**'. Zerrendarako harpidetza eskaera egin duten guztien zerrenda agertuko da. Eskaera bat onartu edo atzera botatzeko, gaitu pertsonaren izenaren ondoko kutxa eta klikatu dagokion botoian.

**Harpidedun guztiei harpidetzaren oroigarria bidaltzeko**, klikatu '****' botoia. Harpidetzaren mezu oroigarriak honakoa du:

-   harpidetzaren **zerrendaren izena**;
-   harpidetza honetarako erabili den **eposta helbidea**;
-   harpidedunaren **zerrendako pasahitza**;
-   zerrendaren **informazio orrirako esteka**;
-   zerrendatik **ez-harpidetzeko helbide klikagarria**.

| Note |
|------|
| 'Zerrendaren konfigurazioa aldatu' ataleko '[Denetarik](listconfig#other.md)' atalean harpidetzaren oroigarri automatikoak konfiguratu ahal dituzu baita ere. |

Orri honetatik **harpidedunak ez-harpidetzeko**, beraien izenen ondoan dagoen kutxa gaitu eta klikatu '**Hautatutako eposta helbideak ezabatu**' botoia.

| Note |
|------|
| Ez badituzu harpidedunak ohartarazi nahi, gaitu 'Isila' kutxa. Hala ere ez da gomendagarria, errebotatzen duten harpidedunak ez badira. |

| Note |
|------|
| Iradokizuna: harpidedun guztiak batera hautatzeko, egiaztatu guztiak agertzen direla orrian eta klikatu 'Hautapena alderantzizkatu' botoian: harpidedun guztiak klik batekin hautatuko dira! |

**Harpidedun baten harpidetza aukerak aldatzeko**, sakatu bere eposta helbidean.

Orri honetatik, **harpidedunaren izena, eposta helbidea eta mezuen bidalketa modua aldatu** ditzakezu. **Bera ez-harpidetu** ahal duzu baita ere.

Harpideduna [errebotatzen badabil](#manage_bounces), beste formulario bat agertuko da 'Harpidedunaren informazioa' formularioaren azpian:

Agertzen den informazioa:

-   errore mota (Ingelesez);
-   errore kopurua;
-   erroreak egon diren tartea.

**Azken errorea aztertu** edo **erroreak berrezarri** ahal duzu. Erroreak berrezartzen badituzu, harpidedunaren [puntuazioa](listconfig#bouncers.md) zeron jarriko da.

Errebotatzen duten helbideak errazago kudeatzeko, kudeaketa moduluko '[Erreboteak](#manage_bounces)' orrira joan.

#### <span id="manage_bounces"></span>Erreboteak kudeatzen

**Harpidedunen eposta helbidearekin arazo bat** dagoenean (eposta helbide zaharkituak, mezuak bidaltzean atzigarri ez zeuden helbideak, kuota gaindituak, etab.), erreboteen ehunekoa ezkerreko menuan agertzen da '**Errore tasa**' izenarekin. Errebotatzen duten helbideak aztertzeko joan kudeaketa moduluko '**Erreboteak**' orrira.

Sympa softwareak automatikoki kudeatzen ditu errebotatzen duten harpidedunak: errore kopurua eta zerrendako trafikoaren arabera, errebotatzen duten harpidedunak ohartu edo ez-harpidetzen dira. Bere puntuazioa zeron jartzen da berriz helbidea errebotatzeari uzten dionean.

**Helbideen erreboteak gelditzeko**, gaitu bere kutxa eta klikatu '**Hautatutako erabiltzailearen erroreak berrezarri**' botoian. Erroreak jarraitzen badu helbidea berriro errebotatzen markatuko da zerrendara mezu bat bidali bezain laster.

**Errebotatzen dauden harpidedunak ez-harpidetu** ahal dituzu baita ere: errebotatzen duten helbide gehiegi daudenean eposta zerrenden zerbitzariaren karga asko handitzen da. Ez-harpidetzeko, gaitu beraien izenen ondoan dauden kutxaj eta klikatu '**Hautatutako eposta helbideak ezabatu**' botoian.&gt;

| Note |
|------|
| Iradokizuna: harpidedun guztiak batera hautatzeko, egiaztatu guztiak agertzen direla orrian eta klikatu 'Hautapena alderantzizkatu' botoian: harpidedun guztiak klik batekin hautatuko dira! |

#### <span id="moderate"></span>Zerrendara bidaltzen diren mezuak moderatzen

Zerrenda bat moderatuta dagoenean **mezu guztiak moderatzaileren batengatik onartuak izan behar dira zerrendara bidali baino lehen**. Zerrendara mezua bidali ostean harpidedunari eposta bat bidaltzen zaio bere mezua moderazio zain dagoela ohartarazteko. Moderatzaileek ere eposta bat jasotzen dute ohar batekin, moderatzeke dagoen mezuarekin.

**Moderazio lanak** ere **epostaz** egin ditzakezu, Sympa-tik jasotako mezuari erantzunez, edo **eposta zerrendako web interfazetik**. Horretarako, klikatu 'Moderatu' azpimenuko '**Mezua**' esteka: moderatzeke dauden mezuen zerrenda agertuko zaizu (mezu berrienak goialdean). **Mezu bat irakurtzeko bere gaian sakatu**.

**Bi aukera** dituzu:

-   zerrendara **mezu bidalketa baimendu**;
-   **mezua gaitzetsi eta bidaltzailea ohartarazi**: mezu bat gaitzesten duzunean hobeto bidaltzailea ohartzen baduzu...

Edozein moderatzaile erabaki ahal du mezu bat bidali edo ez. Hala ere, **mezua prozesatzen duen lehen moderatzailea izango da erabakia hartuko duena**. Sympak ohartaraziko zaitu dagoeneko moderatuta dagoen mezu bat prozesatzen saiatzen bazara. Moderatzaile asko daudenean **errazagoa da mezuak zerrendako web interfazetik moderatzea**: horrela, moderatzeko zain gelditzen diren mezu guztiak ikusiko dituzu.

| Note |
|------|
| **Moderazioaren data edozein dela ere, mezuaren bidalketa data ez da aldatuko**. Horrela, mezua onartzeko denbora asko pasa bada gerta liteke Urtarrilak 1ean bidalitako mezu bat Abenduak 31an jasotzea! |

Mezua ohar batekin gaitzetsi bada, bidali duen harpidedunak eposta bat jasoko du. [Jasotzen duen mezua pertsonalizatu](#customize) dezakezu.

'**Ohartarazi gabe gaitzetsi**' kutxa gaitzean mezuaren egileak ez du oharrik jasoko.

'**Zerrenda beltzera gehitu**' kutxa gaituz gero ez da gaitzespen mezurik bidaliko eta mezuaren egilea zerrenda honen zerrenda beltzera gehituko da. Orriaren behealdean dagoen '**zerrenda beltza editatu**' botoia erabiliz zerrenda beltza kudeatu dezakezu.

Mezuaren egileari bidaltzen zaion gaitzespen oharra pertsonalizatu nahi baduzu, '**Gaitzespen mezuak kudeatu**' botoiarekin egin ahal duzu. Mezuen kudeaketa orrian gaitzespen mezuen multzo bat definitu ahalko duzu eta lehenetsia zein den adierazi.

**Oroigarria**: zerrendaren kudeaketa moduluan [moderatzaileak gehitu edo kendu](listconfig#description.md) ahal dituzu. Horretarako, zerrendaren informazio orritik, sakatu '**Administrazioa**'-n, gero '**Zerrendaren konfigurazioa aldatu**'-an, eta azkenik '**Zerrendaren definizioa**-n.

**Zerrendara heldu ondoren mezuak prozesatu** daitezke; erabilgarria izan daiteke zerrenda moderaturik ez dagoenean. **Mezu bat ezabatu** nahi baduzu, [bilatu webeko mezuen artxiboan](arc#arcsearch.md) eta klikatu mezuaren goi eskuinaldean dagoen **markatu eposta hau ezabatzeko** botoian. Baieztapen mezu bat agertuko da; sakatu 'Ados'. Mezua segundo gutxi barru ezabatuko da. **Kontuz ibili: ekintza hau ezin da desegin!!! Mezu bat ezabatzen baduzu ezingo duzu berreskuratu.**

#### <span id="manage_archives"></span>Mezuen artxiboa kudeatzen

Sympak, posta zerrenden kudeaketa robotak, **zerrendara bidalitako mezuen artxibo konprimitua (.ZIP formatuan)** sor dezake. Artxibo hauek deskargatzeko, interesatzen zaizkizun **hilabeteak hautatu** eta klikatu '**Deskargatu Zip fitxategia**' botoian.

| Note |
|------|
| Iradokizuna: 'Artxibo hautaketa' zerrendan, mezuak izan dituzten hilabete guztiak hautatzeko, klikatu lehen hilabeteak, SHIFT tekla sakatuta mantendu eta klikatu zerrendako azken hilabetean. |

'**zerrendaizena\_artxiboa.zip**' izeneko fitxategi bat eskuratuko duzu, barruan hilabete bakoitzerako **'zerredaizena\_urtea-hilabetea' izeneko karpetak** dituena. (adibidea: *list\_example\_2005-06*). Karpeta bakoitzaren barruan **fitxategi izenak zenbakiak dira** mezuen kokapen kronologikoa adierazten dutena (adibidea; '1' izeneko fitxategia hilabeteko lehenbiziko eposta da). Mezu fitxategiak **ez dute luzapenik**; erabili zure gustuko testu editorea (Notepad, WordPad, Vim, etab.) irekitzeko. **Fitxategi bakoitzak mezu oso bat du barruan (goiburu guztiak)**.

'Artxiboa kudeatu' orritik **mezuak ezabatu** ahal dituzu (hilabeteka ezabatuz, mezuz mezu ezabatu ordez). Hori egiteko interesatzen zaizkizun **hilabeteak hautatu** eta klikatu '**Hautatutako hilabetea(k) ezabatu**' botoian.

| Note |
|------|
| **Kontuz ibili: eragiketa hau ezin da desegin!!! 'Hautatutako hilabeteak(k) ezabatu' klikatzen duzunean kontuan eduki ez zaudela artxibo fitxategia ezabatzen bakarrik, hautatutako hilabetetako mezu artxibo osoa baita ere!!!** |

#### <span id="renamelist"></span>Zerrenda berrizendatzen

Zerrendaren kudeaketa moduluan, klikatu '**Zerrenda berrizendatu**'-n. Sartu nahi duzun izena eta sakatu 'Zerrenda hau berrizendatu' botoian. Baieztapen mezu bat agertzen da; klikatu 'Ados'.

| Note |
|------|
| Ideiaz aldatu baduzu eragiketa alderantziz berregin beharko duzu zerrendaren aurreko izena berreskuratzeko. |

**Kontuz: zerrenda berrizendatzen duzunean, zerrenda kudeatzaileei ohartarazi beharko diezu, bestela aldaketa ez da efektiboa izango**.

Zure zerrenda izendatzeko iradokizun batzuk:

-   **Ez erabili hutsunerik, azenturik edo karaktere berezirik** zerrendaren izenean, arazoak zor ditzakete.
-   Aukeratu **esanguratsua eta motza den izena**: pentsa zerrendara mezu bat bidali nahi duten bakoitzean harpidedunek izen hau idatzi beharko dutela!
-   Zerrenda multzo bat kudeatzen badituzu **aurrizki berdina jarri ahal diezu guztiei**; horrela elkarrekin ordenatuko dira eta errazago antzemango dira (adibidez: *xx-erabiltzaileak@, xx-garatzaileak@*, etab.).

#### <span id="supprlist"></span>Zerrenda ezabatzen

**Zerrendaren kudeaketa moduluan** sakatu '**Zerrendaezabatu**'-n. Baieztapen mezu bat agertuko da, sakatu 'Ados'.

| Note |
|------|
| **Kontuz: zerrenda ezabatzen baduzu ezingo duzu zuk bakarrik berriroireki!!! Zerrenda berriro ireki nahi baduzu zerrenda kudeatzaileei eskatu beharko diezu.** |

Benetan, zeintzuk dira zerrenda ezabatzearen **ondorioak**?

-   **Harpidedun guztiak ez-harpidetzen dira** automatikoki (baita zerrendaren jabe eta moderatzaileak).
-   **Mezuen artxiboa mantentzen da** baina inork ezin du atzitu.
-   **Partekatutako dokumentuen web atalean argitaratutako dokumentuak mantentzen dira** baina inork ezin ditu atzitu.
-   **Zerrenda kudeatzaileek bakarrik ireki ahal dute zerrenda berriz**; egiten badute, aurreko harpidedunak berriro harpidetuko dira.

| Note |
|------|
| Kontuz: latentzia apur bat dela eta, zerrendako orriak eskuragarri egongo dira tarte baterako, beraien helbidea badakizu. Erabat atziezin egongo dira. |

**Zerrenda eta erlazionatutako fitxategi guztiak betirako ezabatu nahi badituzu**, zerrenda kudeatzaileei eskatu beharko diezu.

### <span id="rulesadmin"></span>Ohitura onak

Zerrenda dinamikoak izateko, bertako mezu trukeetan **sakon inplikatuta egon behar duzu**: zerrenda bat ez badu bere jabeak kontrolatzen ez girotzen, bere mezuen kalitate galera egon daiteke eta azkenean desagertu liteke...

**Epostaren erabilera orokorrean eta eposta zerrendetan arau sorta zehatz batzuetara lotuta dago, mezu trukeak atseginak izateko: "Netiketa"**.Zerrenda jabe edo moderatzaile bezala, zure lana da harpidedunek hau betetzea.Netiketaren printzipio orokorrak eta esteka pila bat [Wikipediako Netiketaren orrian](http://eu.wikipedia.org/wiki/Netiketa).

<span id="charter"></span>**Zure zerrendaren arautegi bat** idatzi beharko zenuke bertan bete beharreko arau guztiekin:

-   baimendutako, onartutako eta debekatutako mintzagaiak;
-   idazteko gidalerroak (adibidez erabili beharreko hizkuntza, "SMS hizkuntza" debekatzeko, etab.);
-   mezuen bidalketarako erregelak (frekuentzia, eranskinak, etab.);
-   netiketarekin erlazionatutako ardurak;
-   harpidedunen eskubide eta betebeharrak;
-   mezura bidalitako mezuen eusteari buruzko informazioa;
-   informazio legala eta pribatutasun politika;
-   zerrendaren arautegian agertzen dena ez betetzeagatik egongo diren zigorrak;
-   etab.

| Note |
|------|
| Harpidedun guztiek arautegia irakurtzen dutela bermatzeko harpidetu eta gero bidaltzen zaien ongietorri mezuan txertatu beharko zenuke. Horretarako, [mezu hori pertsonalizatu](#customize) behar duzu, zerrendaren kudeaketa moduluan dagoen 'Pertsonalizatu' orrian. |

Eskuragarri dagoenean, 'Jabe eta moderatzaileen arautegia'k zerrendaren jabe eta moderatzaileek beraien lana egiteko behar duten informazioa guztia du. Arautegi honek jabe eta moderatzaileen eskubide eta betebehar guztiak lantzen ditu.

------------------------------------------------------------------------
