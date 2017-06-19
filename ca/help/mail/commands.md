Llista d'ordres de la interfície de correu de Sympa
---------------------------------------------------

S'han d'enviar totes les ordres a {{conf.email}}@{{conf.host}}.

Es pot enviar més d'una ordre en un missatge. Les ordres han d'anar en el cos del missatge (una ordre per línia).

### Ordres per als usuaris

`HELP`: es rep una llista amb totes les ordres disponibles

`LISTS`: es rep una llista de totes les llistes que es gestionen en el servidor

`WHICH`: es rep una llista de totes les llistes en què esteu subscrits

`CONFIRM clau`: confirma l'enviament d'un missatge (segons la configuració de la llista)

`QUIT`: indica el final de les ordres (s'empra per a ignorar la signatura)

`INFO llista`: es rep informació de la llista

`REVIEW llista`: es rep una llista de tots els membres de la llista

`SUBSCRIBE nom llista`: subscripció (o confirmació de la subscripció) a la llista

`INVITE correu llista`: s'invita algú a subscriure's a la llista

`UNSUBSCRIBE correu llista`: es dona de baixa de la llista. Només es necessita l'adreça si voleu donar-vos de baixa des d'una adreça diferent de què esteu subscrits

`UNSUBSCRIBE * correu`: donar-se de baixa totes les llistes a què esteu subscrits

`SET llista NOMAIL`: se suspèn la recepció de missatges de la llista

`SET llista DIGEST`: es reben missatges en la modalitat recopilatori

`SET llista DIGESTPLAIN`: es reben missatges en la modalitat recopilatori (text net)

`SET llista SUMMARY`: només es rep la llista de missatges

`SET llista NOTICE`: només es reben els assumptes dels missatges

`SET llista MAIL`: modalitat d'entrega de missatges normal

`SET llista CONCEAL`: deixar d'aparèixer en la llista (oculta l'adreça del subscriptor)

`SET llista NOCONCEAL`: es pot veure l'adreça del subscriptor a través de REview

`INDEX llista`: es rep la llista dels fitxers de l'arxiu

`GET fitxer llista`: es un fitxer de l'arxiu de la llista

`LAST llista`: es reben els últims missatges de la llista

### Ordres per a propietaris

`ADD nom del correu de la llista`: s'afig un membre a la llista

`DEL correu llista`: s'elimina un subscriptor de la llista

`STATS llista`: es comproven les estadístiques de la llista

`REMIND llista`: s'envia a tots els subscriptors un recordatori personalitzat amb l'adreça amb què està subscrit a la llista

### Ordres per a moderadors

`DISTRIBUTE clau llista`: s'aprova un missatge

`REJECT clau llista`: es rebutja un missatge moderat

`MODINDEX llista`: es comprova la llista de missatges per moderar
