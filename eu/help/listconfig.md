<span id="listconfig"></span>Zerrenda konfiguratzen
---------------------------------------------------

Zerrendaren konfigurazioa nahiko konplexua denez, atal ezberdinetan banatuta dago, orri bat atal bakoitzeko:

-   [Zerrendaren definizioa](#description);
-   [Bidalketa/Jasotzea](#sending);
-   [Baimenak](#command);
-   [Artxiboa](#archives);
-   [Erreboteak](#bounces);
-   [Denetarik](#other).

**Konfigurazio aldaketak progresiboki egitea** gomendatzen dizugu: horrela, emaitzak ez bazaitu betetzen errazagoa izango da atzera botatzea.

Zerrendaren kudeaketa moduluak **zure zerrenda konfiguratzeko aukera asko** eskaintzen dizkizu. Hala ere, baliteke aukera hauek ez betetzea zure beharrak erabat. Hau konpontzeko, **zerrenda kudeatzaileei aukera berriak eskatu** ahal diezu (beraien eskura dagoen heinean, noski...): pertsona multzoak mugatu beraien izena emateko lekuaren arabera, beraien epostaren domeinuaren arabera, beraien taldea, eta abar.

### <span id="description"></span>Zerrendaren definizioa

'**Zerrendaren gaia**' eremuan zerrenda sortzean hautatu zenuen gaia aldatu dezakezu. Gai hau zerrendako horri guztietako orrien goiburuan agertzen da, zerrenden indize orrietan ere ikus daiteke (zerrenden zerrendak, zure harpidetzen zerrendak, etab.) eta nabigatzailearen izenburu barran agertzen da.

'**Zerrendaren ikusgaitasuna**' aldatu dezakezu baita ere. Aukerak ondokoak dira:

-   harpidedunak ez direnengandik ezkutatu (ezkutatu) - *defektuzko aukera*;
-   intraneteko atzipena (intranet);
-   ez ezkutatu (ez ezkutatu);
-   harpidedunengandik ere ezkutatu (sekretua);

| Note |
|------|
| Zerrendaren ikusgaitasuna beste irizpide batekin mugatu nahi baduzu zerrenda kudeatzaileei eskatu beharko zenieke: zure beharrak asetzen duen aukera sortzeko gai izan daitezke (adibidez: erabiltzaile talde batentzako bakarrik, internet domeinu bat, etab.). |

'Jabeak' eta 'Moderatzaileak' eremuetan zerrendara **jabeak eta moderatzaileak gehitu** ahal dituzu edo **beraien informazio pertsonala aldatu**:

-   Jabe/Moderatzaile bakoitzeko **eposta helbidea** eta **izena** zehaztu behar dituzu.
-   ~~You can also add the information of your choice in the '**Private information**' input box (phone number, function, etc.); this information will only be accessible by listmasters and list owners with a 'Privileged' profile.~~
-   **Mezu bidalketa modua** aldatu dezakezu (orri honetako aukera bakarrak 'eposta' eta 'epostarik ez' dira).
-   'Profila' parametroa ezin da aldatu: **'Berezia' profila** zerrendaren sortzailearentzat erreserbatuta dago (beste jabeek profil 'Normala' dute).

| Note |
|------|
| Kontuz: jabe edo moderatzaile bihurtzeak ez du automatikoki harpidetuko itxitazarenik ezan nahi. Jabe eta moderatzaileak bere kabuz harpidetu beharko dira beraz. |

**Jabe/moderatzaileak ezabatzeko**, kendu nahi duzun pertsonaren eremuetan dagoen edukia ezabatu eta klikatu 'Eguneratu' botoian.

**Zerrendaren mintzagaia** eta bere **hizkuntza** ere aldatu ditzakezu. Zerrendaren hizkuntza aldatzen baduzu aurredefinitutako mezu guztiak hautatutako hizkuntzan bidaliko dira (kontuz: itzulpenak eginda egon behar dute!).

Ezin duzu zerrendako **Interneteko domeinua** aldatu: parametro hau zerrenda kudeatzaileek bakarrik aldatu ahal dute.

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzea** egin dituzun aldaketak gordetzeko.

### <span id="sending"></span>Bidalketa/jasotzea

Orri honetan **zerrendara mezuak zeinek bidali ahal dituen erabaki** ahal duzu.

'**Bilduma maiztasuna**' arean konpilatutako mezuak (Bilduma eta laburpen modual) zein maiztasunarekin bidaltzen diren definitu ahal duzu: zerrendan, hautatu bilduma bidali nahi duzun **egun** guztiak. Gero bildumentzako **bidalketa ordua** hautatu (mesedez ez hautatu 23:00 eta gauerdi harteko ordurik).

'**Harpidetze aukerak**' zerrendan, hautatu harpidedunei eskaini nahi dizkiezun aukerak. Defektuz aukera guztiak hautatuta daude.

'**Erantzun helbidea** eremuak zerrendara bidalitako mezu bat erantzutean defektuz nori bidaliko zaion definitu ahal duzu:

-   '**Dena**' balioarekin, erantzuna **mezuaren bidaltzaileari** ETA **zerrendari** bidaltzen zaie.
-   '**Zerrenda**' balioarekin, erantzuna **zerrendara** bidaltzen da

    | Note |
    |------|
    | Kontuz ibili aukera honekin! Esperientziak esaten du harpidedunek ez dutela beti erantzuten dauden helbidea egiaztatzen. Beraz, mezu pribatu bat zerrendara bidali ahal dute pertsona bakar bati erantzun nahi diotenean... |

-   '**Beste eposta**' balioarekin, erantzuna **aurredefinitutako helbide** batera bidaltzen da. Hau aukeratzen baduzu, 'Beste eposta helbide bat' eremuan eposta helbide bat zehaztu beharko duzu.
-   '**Bidaltzailea**' balioarekin, erantzuna **mezua bidali duenari** bidaltzen zaio. Hau da ziur aski aukeratu behar duzuna.

'**Aurreko goiburua eremua mantendu** kutxak sartzen diren mezuen 'Reply-To' SMTP goiburuarekin zer egingo den aukeratzen uzten dizu. '**Mantendu**' aukerak eremu hori mantentzen du eta '**Derrigortutakoa**' aukerak gainidazten uzten du.

Azkenik, '**Gaiaren etiketatzea**' aukerak zerrendara bidalitako **mezu guztien gaiaren aurrean txertatuko den testua** hautatzen uzten dizu: honek harpidedunei mezuak errazago ordenatzea ahalbidetzen die, mezuak automatikoki prozesatzeko iragazkiak erabili, etab. Defektuz testu hau **zerrendaren izena kortxeteen artean** da (kortxeteak sistemak gehitzen ditu automatikoki, ez dituzu zuk bertan zehaztu behar).

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzea** egin dituzun aldaketak gordetzeko.

### <span id="command"></span>Baimenak

Orri honetan ondokoa erabaki ahal duzu:

-   **Informazioa zeinek ikusi ahal duen**. Aukera hauek daude:
    -   edozeinentzako (irekia) - *defektuzko aukera*
    -   harpidedunentzat bakarrik (pribatua).
-   **zein harpidetu daiteke**. Aukera hauek daude:
    -   harpidetza eskaera baieztatuta (auth);
    -   autentifikazioa behar du (jabeei ohartarazpena bidaltzen zaie) (auth\_notify);
    -   autentifikazioa eta jabearen baieztapena behar du (auth\_owner);
    -   ezin da harpidetu (itxita);
    -   domeinu lokalekoentzat bakarrik (intranet);
    -   domeinu lokalekoak edo jabearen oniritzia (intranetorowner);
    -   edonorentzat Autentifikazio gabe (irekia) - *defektuzko aukera*;
    -   edonor, jabeari ohartarazpena bidaltzen zaio (open\_notify);
    -   edonor, ongietorri mezurik ez (open\_quiet)
    -   jabearen oniritzia (owner);
    -   S/MIME zinadura behar du (smime);
    -   S/MIME zinadura edo jabearen oniritzia (smimeorowner).

        | Note |
        |------|
        | 'auth' parametroa duen aukeraren bat hautatu beharko zenuke: horrela sistemak harpidedunari baieztapena eskatzen dio harpidetu baino lehen. Honek eposta helbide okerrekin harpidetzea saihesten du, eta ohartu gabe inor ez dela harpidetu bermatzen du. |

-   **zein harpidetu daiteke**. Ondoko aukerak daude:
    -   Autentifikazioa behar du (auth);
    -   autentifikazioa eskatuta, jabeari ohartarazpena bidaltzen zaio (auth\_notify);
    -   ezinezkoa (closed);
    -   irekia (open) - *defektuzko aukera*
    -   irekia eposta baieztapenarekin, jabea ohartarazia (open\_notify);
    -   jabearen oniritzia (owner)

        | Note |
        |------|
        | 'auth' parametroa duen aukeraren bat hautatu beharko zenuke: horrela sistemak harpidedunari baieztapena eskatzen dio harpidetu baino lehen. Horrela inork ezingo du beste bat ez-harpidetu bera jakin gabe. |

-   **zerrendara harpidetzeko gonbidapenak zeinek bidali ahal ditu**. Aukera hauek daude:
    -   itxita (closed)
    -   zerrenda jabeak, autentifikaziorik ez (owner);
    -   harpidedunentzat mugatuta (private) - *defektuzko aukera*;
    -   publikoa (public).
-   **zeinek ikusi ditzake harpidedunak**. Ondoko aukerak daude:
    -   inor ezin ditu ikusi (close)
    -   harpidedun edo domeinu lokalekoak bakarrik (intranet);
    -   zerrenda kudeatzaileak bakarrik (listmaster);
    -   jabea bakarrik (eta zerrenda kudeatzailea) (owner) - *defektuzko aukera*;
    -   harpidedunentzat mugatuta (private);
    -   edonork egin ahal du! (public).

        | Note |
        |------|
        | Ez zenuke harpidedunen zerrenda edonorentzat atzigarri utzi beharko. 'Harpidedunentzat mugatuta' aukera interesgarria izan daiteke harpidedunak elkarren artean komunikatzeko zerrendatik pasa gabe. Hau ez da egokia harpidedunak elkarren artean erlaziorik ez duten iragarpen zerrendetan, ordea. |

<span id="docsrights"></span>Orri honetatik **partekatutako dokumentuen web atalera aplikatuko diren baimenak definitu** daitezke baita ere ('Partekatutako dokumentuak' atala, ezkerreko menuko menuan atzigarri). Dokumentuen irakurri eta idazteko baimenak definitu ahal dituzu:

-   Ondoko aukerak daude '**Zeinek ikus dezake**' kutxan:
    -   harpidedun edo domeinu lokalekoak bakarrik (intranet);
    -   zerrenda jabeei mugatuta (owner);
    -   harpidedunentzat mugatuta (private) - *defektuzko aukera*;
    -   dokumentu publikoak (public).
-   Ondoko aukerak daude '**Zeinek edita dezake**' kutxan:
    -   zerrenda jabeei mugatuta (owner) - *defektuzko aukera*;
    -   harpidedunentzat moderatuta (editor);
    -   harpidedunentzat mugatuta (private);
    -   dokumentu publikoak (public).

'**Kuota**' kutxan **partekatutako dokumentuen web atalaren tamaina maximoa** definitu dezakezu. Honek ez du partekatutako dokumentuen web atalean argitaratutako dokumentu *baten* tamaina zehazten, dokumentu guztien batura baizik. Kilobytetan adierazten da. Harpidedun batek geratzen den lekua baino handiagoa den dokumentu bat igotzen saiatzen denean errore mezu bat jasoko du.

**partekatutako dokumentuen web atalari buruz gehiago** jakiteko (nola antolatu, baimenak aldatu, dokumentuak izendatu, etab.), joan erabiltzaile gidaren '[Partekatutako dokumentuen web atala erabiltzen](shared.md)' atalera

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzea** egin dituzun aldaketak gordetzeko.

### <span id="archives"></span>Artxiboa

Orri honetatik **web artxiboa zeinek atzitu dezakeen erabaki** dezakezu (eposta zerrendaren web interfazea irakurgarri dauden mezuak). Ondoko aukerak daude:

-   itxita (closed)
-   domeinu lokalekoentzat bakarrik (intranet);
-   zerrenda kudeatzailea (listmaster);
-   jabea (owner);
-   moderatzailea (moderator);
-   harpidedunak bakarrik (pribatua);
-   publikoa (public).

'**Kuota**' kutxak **artxiboaren tamaina maximoa** definitzen uzten dizu. Tamaina kilobytetan adierazten da. Zerrenda jabeak oharra jasotzen dute artxiboaren tamaina era heltzea denean. Maximoa gainditzen denean mezuak ez dira gehiago artxibatzen.

| Note |
|------|
| Nahiz eta mezuak ez diren artxibatzen, posible da zerrendara mezuak bidaltzen jarraitzea. |

**Zerrendako artxiboa eposta bidez eskuratu** ahal da ere, **{{conf.email}}@{{conf.host}}** helbidera ondoko komandoa bidaliz: <span class="commande">**GET zerrendaizena urtehilbetea**</span> (adibidez: *GET zerrenda\_bat 2016-07*). Hautatutako hilabeteko mezu guztien bilduma jasoko duzu. Bilduma testu hutsean bidaltzen da eta HTML etiketak ditu berezkok formatuaren ordez; mezu bakoitzaren goiburu guztiak adierazten dira ere. '**Testu artxiboak**' parametroak ondokoa adieraz dezake:

-   **zeinek jaso ahal ditu** zerrendako mezuen artxiboa posta bidez;
-   **artxibo fitxategi hauek sortzeko maiztasuna**. Adibidez, maiztasuna 'hilabetea' bada, hilabete batean zerrendara bidalitako mezu guztiak fitxategi bakar batean elkartuko dira.

Parametro hau ezarrita ez badago, zerrendak ez du eposta bidez jasotzeko artxiborik edukiko. Kontuz: **zerrenda kudeatzaileek bakarrik aldatu dezakete parametro hau.**

Zerrendara mezuak **S/MIME** bidez zifratuta bidali ahal dira. '**Zifratutako mezuak testu hutsean gorde**' aukerak mezu hauek nola artxibatuko diren zehazten du:

-   '**Dezifratuta**' aukerak mezuak dezifratu ostean artxibatzen ditu.
-   '**Jatorrizkoa**' aukerak mezuak zuen zifratzea mantenduta artxibatzen da.

Aukera honek bai testu artxiboetara bai webeko artxiboetara eragiten die, baita 'Bilduma' bidalketa modua aukeratzen dutenentzako bidaltzen den bilketara.

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzen**, orriaren behealdean, zure aldaketa guztiak gordetzeko.

### <span id="bounces"></span>Erreboteak

"**Erreboteek**" **helbidean arazoa duten harpidedunak** adierazten dituzte, hau da, zerrendara bidalitako mezuak jaso ezin dituzten harpidedunak. Arrazoi ezberdinengatik izan daiteke: eposta helbide zaharkituak, mezua bidaltzean eskuragarri ez zegoen helbidea, kuota gaindituak, etab.

'**Erreboteen kudeaketa**' atalak bi tarte definitzen ditu:

-   ~~The **warn rate** indicates the bouncing email addresses rate from which the list owner will receive a **notice entitled 'Bounce rate too high'** inviting him/her to delete bouncing subscribers from the list.~~
-   ~~The **halt rate** indicates the bouncing email addresses rate from which **the message distribution will automatically be stopped** up to the resolution of the problem (generally through the deletion of bouncing subscribers).~~

<span id="bouncers"></span>'**Erreboteen kudeaketa, 1.go maila**' eta '**Erreboteen kudeaketa, 2. maila**' atalek errebotatzen duten harpidedunekin ataza automatikoak ahalbidetzen dituzte. Definitu dezakezu:

-   **1.go maila eta 2. mailako erreboteak definitzen dituzten tarteak**. Defektuz, 1.go mailako erreboteak 45 eta 74 arteko puntuazioa dute eta 2. mailakoak 75 eta 100 artekoa;

    | Note |
    |------|
    | Puntuazioa erroreen kopuru, mota eta maiztasunaren menpekoa da. Erreboteen arteko tartea oso txikia bada edo ez badira errore asko egon, erreboteak ez du puntuaziorik irabazten. |

-   **dagokion harpidedunarekin burutuko den ataza**: atazarik ez, oharra, zerrendatik ezabatu;
-   ataza burutzen denean **ohartaraziko den pertsona**: inor ez, zerrendako jabeak, zerrenda kudeatzaileak. Ataza burutzean bidaltzen den ohartarazpenak eragindako harpidedun guztien izenak eta atazari buruzko informazio zehatza dauka.

**Erreboteak kudeatzeko** (harpidedun baten erroreak berrezarri, errebotatzen duen harpideduna ez-harpidetu, harpidetzaren oroigarria eskatu, etab.), joan kudeaketa moduluko '[Erreboteak](admin.md#manage_bounces)' orrira.

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzen**, orriaren behealdean, zure aldaketa guztiak gordetzeko.

### <span id="other"></span>Denetarik

'**harpidetzaren iraungitze periodikoaren ataza**' aukerak zerrendako **harpidetzen iraungitze data automatikoak** definitzea ahalbidetzen dizu: periodikoki (adibidez: urtero), harpidedunek beren harpidetza berritzeko eskaera bat jasoko dut. Ez badute egiten automatikoki ez-harpidetuko dira. Prozesu honek zerrendara harpidetutako guztiek interesa mantentzen dutela ziurtatzen du.

'**Harpidetzaren oroitzapen periodikoaren ataza**' aukerak zerrendako harpidedunei harpidetzen oroigarriak periodikoki bidaltzen ahalbidetzen dizu.

'**Eposta helbidea babesteko modua**' aukerak spam-robotek harpidedunen eposta helbideak hartuko ez dituztela ziurtatzen du. Aukera hau orri guztietan aplikatzen da.

Orri honetan **zerrendaren azken eguneraketari buruzko informazioa** (zeinek eta noiz egin zuen), eta zerrenda sortu zenetik **konfigurazio aldaketen kopurua** ikus ditzakezu ere bai.

**KONTUZ: ez ahaztu 'Eguneratu' botoia sakatzea** egin dituzun aldaketak gordetzeko.
