Listas de correo - Introducción General
---------------------------------------

### ¿Qué es una lista de correo?

Una lista de correo es una **lista de distribución que permite a un grupo de suscriptores recibir automáticamente todos los mensajes enviados a ella**: todo mensaje enviado a la lista por un suscriptor es recibido por el resto de suscriptores. Cuando te suscribes a una lista de correo, puedes enviar mensajes, responderlos o simplemente leerlos sin participar.

**Casos especiales:**

-   A veces es posible enviar mensajes a una lista de correo sin estar suscrito a ella. Sin embargo, necesitas estar suscrito a una lista para poder recibir sus mensajes.
-   A veces es imposible enviar mensajes a una lista aún cuando estés suscrito a ella: éste es el caso de las listas de anuncios, las cuales son usadas para enviar información desde un único remitente a un gran número de receptores.

### Utilidad de las listas de correo

Las personas que se suscriben a una lista de correo (algunas veces abreviada como ML) para **informarse sobre un tema determinado** y para **ser partícipe de los intercambios al respecto**. Ejemplos de esto son:

-   listas de correo para todos los empleados de una compañía;
-   una lista de correo reservada a los participantes de un proyecto;
-   una lista de correo dedicada a los estudiantes de una clase;
-   una lista de correo sobre las últimas noticias sobre seguridad en ordenadores;
-   una lista de correo para la ayuda mutua entre reparadores;
-   una lista de correo restringida a los miembros de una familia y dedicada a la orgnización de grandes reuniones familiares;
-   ¡Y así sucesivamente!

### Tipos de listas de correo

Hay **miles de listas de correo** de todos los tipos en Internet: públicas y privadas, gratis y de pago, con la suscripción condicionada a ciertas reglas y no, etc. Estas listas pueden tener desde una docena a varios miles de miembros.

De acuerdo a como funcionan, podemos distinguir entre **dos tipos de listas**:

-   **Las Listas de anuncios**, permiten a los suscriptores solo recibir mensajes. De hecho, estos mensajes se conocen como boletines de noticia: revistas electrónicas, servicios diarios (horóscopo del día, el tiempo atmosférico del día, alertas de seguridad del día, etc.), notificaciones de actualización de un sitio web, etc. Con este tipo de lista de correo, la información va desde un único remitente a un gran número de receptores.
-   **Listas de discusión**, que permiten a todos los suscriptores tomar parte de los envíos. Estas listas pueden ser moderadas o no:
    -   En una **lista de discusión moderada**, los mensajes son transmitidos a todos los suscriptores una vez que han sido aprobados por uno de los moderadores de la lista. La moderación es una de las cualidades de la lista. Por ejemplo, asegura que los suscriptores no recibirán mensajes fuera del tema de la lista o mensajes comerciales no solicitados (spams) o mensajes que contienen archivos adjuntos de gran tamaño, etc.
    -   Es una **lista de discusión no moderada**, los mensajes son transmitidos tan pronto como el robot de administración de la lista los recibe.

### <span id="features"></span>Funciones

Una vez suscrito a una lista de correo, puedes:

-   **buscar una lista de correo** según tus intereses principales o tu situación particular;
-   **gestionar tus suscripciones**:
    -   [suscribirte](user#subscribe.md) a listas,
    -   [darte de baja](user#unsubscribe.md) de listas a las que te encuentras suscrito,
    -   cambiar tus [opciones de suscripción](user#options.md) lista por lista,
    -   cambiar tus [preferencias generales](user#pref.md), las que se aplican todo el entorno de las listas de correo (nombre, contraseña, idioma de la interfaz web, etc.);
-   **usar las listas de correo**:
    -   leer el [archivo web de mensajes de las listas a las que no estás suscrito](arc.md), si ese archivo es público y si tus permisos personales te permiten acceder a esas listas,
    -   leer el [archivo de las listas a las cuales estás suscrito](arc.md),
    -   realizar [búsquedas en los archivos de la lista](arc#arcsearch.md),
    -   [enviar mensajes](sendmsg.md) a las listas a las que estás suscrito,
    -   [descargar documentos](shared#shared_read.md) desde el espacio de documentos compartidos,
    -   [subir documentos](shared#shared_upload.md) al espacio de documentos compartidos;
-   **gestionar listas de correo**:
    -   [crear nuevas listas](admin#create_list.md) (acceso restringido) - sujeto a la autorización,
    -   [configurar las listas](admin#edit_list.md) que te pertenecen,
    -   [administrar suscripciones](admin#manage_members.md),
    -   [administrar el espacio de documentos compartidos](admin#manage_shared.md),
    -   [moderar las listas](admin#moderate.md) de las cuales eres moderador.

### <span id="roles"></span>Cómo funciona el servicio de listas de correo: roles y responsabilidades

Un servicio de listas de correo involucra cuatro tipos de roles:

-   ~~**listmaster;**~~
-   **dueño;**
-   **moderador;**
-   **suscriptor.**

Es posible tener varios roles al mismo tiempo (por ejemplo, puedes ser el dueño y moderador de una lista y estar suscrito a varias otras).

#### ~~Listmasters~~

Los listmasters están a cargo de **la administración del servicio de listas de correo**. Sus tareas:

-   **administración del servidor de listas de correo** (implementación, mantención, etc.);
-   **definir las orientaciones generales del servicio de listas de correo**:
    -   a quién se le permitirá pedir la creación de una nueva lista,
    -   cuales opciones estarán disponibles en la gestión de la lista (definición del scenario),
    -   lo que contendrán por defecto los archivos (creación de modelos),
    -   cómo se verá la interfaz web de la lista de correo;
-   **indica la forma en que el servicio de listas de correo debe usarse** y **documenta esas reglas en los mensajes** enviados a suscritpores, moderadores y dueños;
-   **aprueba las slocitides de creación de lista de correo**
-   cuando sea necesario, **sustituye temporalmente a los dueños de la lista**; por otra parte, los listmasters no deberían realizar las funciones de los moderadores.

**Los dueños de la lista y los moderadores pueden notificar a los listmasters** cuando encuentren algún problema que no esté relacionado con la documentación o con algún comentario. Sin embargo, para no inundar a los listmasters con mensajes, se recomienda que los suscriptores se pongan en contacto con los dueños de la lista

#### Dueños

**El dueño de la lista suele ser su creador** o, en su defecto, la persona que ha solicitado la creación de la lista o quien se haga responsable de ella. **Su rol**:

-   **define la [forma en que se utilizará la lista](admin#edit_list.md)**;
-   **escribe una [carta de bienvenida](admin#charter.md)** orientada a los suscriptores;
-   **establece uno o varios <span>moderadores</span>**;
-   **gestiona las [suscripciones y desuscripciones](admin#manage_members.md)**;
-   **cuando es relevante poner un [documento compartido en el espacio web](admin#manage_shared.md)** a la disposición de los suscriptores;
-   **contesta preguntas de los suscriptores o potenciales suscritores sobre la lista;**
-   ~~etc.~~

Una lista puede tener varios dueños. Sin embargo, el **perfil 'Privilegiado'** se reserva al creador de la lista; el resto de dueños tienen el perfil 'Normal', el cual tiene menos privilegios.

#### Moderadores

**Los moderadores los nombra el dueño de la lista**. Ellos se encargan de [controlar la relevancia de los mensajes](admin#moderate.md) enviados a la lista: despues de leerlos, **eligen si los aceptan o los rechazan.**. El proceso de moderación ocurre antes de que el mensaje se envíe a los suscriptores. El rechazo de un mensaje posiblemente va asociado a una notificación para el remitente con la intención de explicar la razón del rechazo.

Una lista puede tener uno o varios moderadores; generalmente, el dueño de la lista es también un moderador.

Esto concierne solo a los moderadores de listas.

### <span id="policy"></span>Framework Regulador

El uso de un servicio de listas de correo significa respetar una serie de normas:

-   En la mayoría de los servicios de listas de correo, los suscriptores reciben una 'Carta de bienvenida' en la suscripción. Se encuentran entonces obligados a respetar todas las reglas contenidas en dicha carta.
-   Si está disponible, los dueños y moderadores de la lista tienen que estar de acuerdo con la 'Carta de dueño y moderador'.
-   El uso de listas de correo naturalmente implica respetar las normas de buenas prácticas referentes al correo electrónico.

Para conocer mas, diríjase a la sección dedicada a [las buenas prácticas para suscriptores](sendmsg#rulesuser.md) y a la sección sobre [buenas prácticas para dueños y moderadores](admin#rulesadmin.md).

------------------------------------------------------------------------
