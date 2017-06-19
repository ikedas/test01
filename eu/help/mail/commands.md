Sympako eposta interfazeko komandoen zerrenda
---------------------------------------------

Komando guztiak {{conf.email}}@{{conf.host}} helbidera bidali behar dira.

Mezu bakar batean komando anitz bidali ahal dira. Komandoak mezuaren gorputzean joan behar dute (komando bat lerro bakoitzeko).

### Erabiltzaileentzako komandoak

`HELP`: eskuragarri dauden komandoen zerrenda jaso

`LISTS`: zerbitzariak kudeatzen dituen zerrenda guztien zerrenda jaso

`WHICH`: harpidetuta zauden zerrenda guztien zerrenda jaso

`CONFIRM gakoa`: mezuaren bidalketa baieztatu (zerrenda konfiguratutako moduarekin bat)

`QUIT`: komandoen bukaera adierazten du (sinadurak baztertzeko erabilita)

`INFO zerrenda`: zerrendari buruzko informazioa jaso

`REVIEW zerrenda`: zerrendako kide guztien zerrenda jaso

`SUBSCRIBE zerrenda izena`: zerrendara harpidetza (edo harpidetzaren baieztapena)

`INVITE zerrenda eposta`: baten bat zerrendara harpidetzeko gonbidatu

`UNSUBSCRIBE zerrenda eposta`: zerrendatik ez-harpidetu. Eposta helbidea ez-harpidetzaren eposta mezua bidaltzeko erabili duzun helbidearen ezberdina denean bakarri behar da.

`UNSUBSCRIBE * eposta`: harpidetuta zauden zerrenda guztietatik ez-harpidetu

`SET zerrenda NOMAIL`: zerrendako mezuak jasotzeari utzi

`SET zerrenda DIGEST`: zerrendako mezuak bilduma moduan jaso

`SET zerrenda DIGESTPLAIN`: zerrendako mezuak bilduma moduan jaso (testu hutsa)

`SET zerrenda SUMMARY`: mezuen zerrenda jaso bakarrik

`SET zerrenda NOTICE`: mezuen gaia jaso bakarrik

`SET zerrenda MAIL`: mezuen bidalketa normala

`SET zerrenda CONCEAL`: zerrendetatik ezkutatu (ezkutatutako harpidedun helbidea)

`SET zerrenda NOCONCEAL`: harpidedunaren eposta helbidea ikusgai jarri

`INDEX zerrenda`: artxiboko fitxategien zerrenda jaso

`GET zerrenda fitxategia`: zerrendako artxibotik fitxategia jaso

`LAST zerrenda`: zerrendako mezu berriena jaso

### Zerrenda jabeentzako komandoak

`ADD zerrenda eposta izena`: zerrendara kide bat gehitu

`DEL zerrenda eposta`: zerrendatik harpidedun bat kendu

`STATS zerrenda`: zerrendako estatistikak jaso

`REMIND zerrenda`: harpidedun guztiei pertsonalizatutako oroigarria bidali zerrendara harpidetzeko erabili zuten eposta helbidearekin

### Zerrenda moderatzaileentzako komandoak

`DISTRIBUTE zerrenda gakoa`: mezua onartu

`REJECT zerrenda gakoa`: moderatzeke dagoen mezua baztertu

`MODINDEX zerrenda`: moderatzeke dauden mezuen zerrenda jaso
