<span id="docadmin"></span>Listas de correo - Guía para el dueño y el moderador
-------------------------------------------------------------------------------

### Introducción: ¿quién es el encargado de gestionar las listas de correo?

Recuerda: un servicio de listas de correo involucra a cuatro tipos de roles:

-   **~~listmaster;~~**
-   **dueño;**
-   **moderador;**
-   **suscriptor;**

Revisa la [descripción de cada rol](introduction.md#roles) para saber más sobre esto.

### <span id="create_list"></span>Solicitar la creación de una lista de correo

La **solicitud de creación de una lista** puede estar **sujeta a condiciones**. Incluso si cumples esas condiciones, **la creación de la lista** estará **sujeta a la aprobación por parte de los listmasters**

Para solicitar la creación de una lista de correo, haz lo siguiente:

1.  Ve a la **[página principal del entorno web](%7B%7Bpath_cgi%7D%7D/home)** y [**accede**](user.md#sympa_auth).
2.  En el menú superior, **pincha en el enlace 'Crear lista'**.

    | Note |
    |------|
    | Si no se muestra el enlace, significa que no tienes privilegios suficientes para crear una lista. |

3.  Dale un **nombre** a la lista (sólo introduce el nombre, sin '@' ni el dominio; ejemplo: *languages\_spanish* y no *languages\_spanish@{{conf.host}}*).

    | Note |
    |------|
    | No utilices ningún espacio, acnetos o caracteres especiales para los nombres de listas: esos caracteres pueden causar problemas. |

    | Note |
    |------|
    | Elige un nombre corto y explícito: ¡piensa en los suscritpores que tienen que escribir ese nombre cada vez que quieran mandar un mensajes a la lista!. Si gestionas un conjunto de listas, puedes poner un prefijo común a los nombres de las listas; así estarán juntas cuando se ordenen y serán fácilmente reconocibles (ejemplo: *xx-usuarios@{{conf.host}}, xx-lineadirecta@{{conf.host}}*, etc.). |

4.  Elige un **tipo de lista** dentro de los tipos predefinidos (los tipos predefinidos son solo ejemplos de configuraciones típicas que pueden cambiarse por los dueños de la lista después de la creación; es incluso posible configurar la lista bajo las opciones ofrecidas en el módulo de administración de la lista, preguntando a los listmasters).
5.  Elige un **asunto** para tu lista. El asunto se mostrará como cabecera de todas las páginas de la lista, y tambíen será visible en las páginas de índice de listas (lista de listas, lista de tus suscripciones, etc.) y en la barra de título del navegador.
6.  Elige un **tema** en el desplegable de 'Temas'.

    | Note |
    |------|
    | Si ningún tema encaja en tus necesidades, puedes solicitar la creación de un nuevo tema solicitándoselo a los listmasters. |

7.  Introduce una **descripción** para tu lista. La descripcíon se mostrará en la página de información de la lista y en la 'Carta de bienvenida para Suscriptores' enviada por correo a cada nuevo suscriptor, bajo la cabecera 'Asunto de la lista'. Esta descripción puede contener información sobre los siguientes aspectos:

    -   motivo de la lista y objetivos;
    -   temas discutidos;
    -   funcionamiento de la lista (responsabilidades, estado de la lista, etc.);
    -   reglas aplicables;
    -   descripción de los suscriptores típicos (sus ocupaciones, los proyectos que gestionan, sus nacionalidades, etc.).

    | Note |
    |------|
    | Puedes dar formato a la descripción de la lista con etiquetas HTML. Ten cuidado: si tu descripción es larga, utiliza finales de línea manuales (tecla ENTER de tu teclado); si no lo haces, es posible que no se vea por completo en la ventana del navegador. |

8.  Pincha en el botón '**Enviar la solicitud de creación de lista**'.

Se muestra un mensaje para informarte que la solicitud de creación de la lista ha sido enviada a los listmasters y desde ese momento, puedes modificar la lista pulsando el botón 'Admin'. Sin embargo, el mensaje advierte que la lista se instalará y será visible en el servidor solamente tras la aprobación por parte del listmaster.

Tras esto, debes **esperar a la parobación de la lista por parte de uno de los listmasters**. Entonces recibirás un mensaje de notificación titulado '**Creación de la lista nombredelalista**', informádote que tu lista ha sido creada.

**Por último, suscríbete a tu lista**: crear una lista o ser su dueño o moderador no significa que automáticamente estés suscrito a ella.

### Gestionar una lista

Para gestionar una lista de la que eres dueño, haz lo siguiente:

1.  Ve a la **página de inicio de la lista** y **[accede](user.md#sympa_auth)**.

    | Note |
    |------|
    | Si estás suscrito a la lista con distintas direcciones, utiliza la dirección con la que solicitaste la creación de la lista. |

2.  **Ve a la página de información de la lista** que quieres gestionar.
3.  En el menú lateral izquierdo, **haz clic en el enlace 'Administración'**.

Para mostrar las secciones del módulo de administración, haz clic en los enlaces situados bajo el enlace 'Administración', en el menú lateral izquierdo.

Las distintas secciones te permiten:

-   [configurar la lista](listconfig.md);
-   [personalizar los archivos relacionados con la lista](#customize);
-   [gestionar suscriptores](#manage_members);
-   [gestionar los archivos de mensajes de la lista](#manage_archives);
-   [gestionar mensajes rebotados](#manage_bounces);
-   [crear, borrar o restaurar el espacio web de los documentos compartidos](#manage_shared);
-   [renombrar la lista](#renamelist);
-   [borrar la lista](#supprlist).

Las opciones disponibles en el submenú 'Moderar' te permitirá:

-   [moderar mensajes](#moderate)enviados a la lista;
-   [moderar documentos](shared.md) disponibles en el espacio web compartido de documentos;
-   [moderar suscripciones pendientes](#manage_members).

#### <span id="edit_list"></span>Configurar la lista

Para aprender a configurar la lista, por favor revisa la [**documentación sobre la configuración de listas**](listconfig.md).

#### <span id="customize"></span>Personalizar la lista

Desde esta página, puedes **editar una serie de archivos relacionados con la lista**, entre ellos:

-   mensajes típicos enviados a los suscriptores en ocasiones particulares:
    -   **mensaje de bienvenida**: este mensaje corresponde a la notificación enviad a la gente que se acaba de suscribir. Debes escribir una carta de bienvenida a tu lista y añadirla a este mensaje de bienvenida. Puedes crear un mensaje MIMEestructurado (reservado para los expertos en formateo MIME);
    -   **mensaje para dar de baja**: este mensaje se envía a la gente que se da de baja de la lista;
    -   **mensaje de borrado**: este mensaje se envía a la gente que se da de baja de la lista (comando DEL), especialmente porque su dirección produce rebotes;
    -   **mensaje recordatorio**: este mensaje se envía a los suscriptores como un recordatorio personalizdo cuando se utiliza el comando REMING. Este comando es esencial para el buen funcionamiento de tu lista ya que muchos rebotes son provocados por gente cuya actual dirección de correo ya no es la dirección suscrita, o incluso quien ha olvidado que están suscritos a la lista;
    -   **mensajes de invitación a la suscripción**: este mensaje se envia a gente para invitarles a suscribirse a la lista utilizando el comando INVITE;
    -   **notificación de mensaje rechazado por el moderador**: este mensaje se envía al remitente de un mensaje rechazado por el moderador;
    -   **notificación de mensaje rechazado por un virus**: este mensaje se envía al remitente de un mensaje en el cual se han encontrado virus.
-   archivos varios:
    -   **descripción de la lista**: la descripción de la lista se envía por correo como resultado del comando INFO. Por defecto, también se incluye en el mensaje de bienvenida (notificación de suscripción). Esta descripción no es la misma que la mostrada en la página de presetnación de la interfaz web de la lista.
    -   **página principal de la lista**: esta descripción está disponible en la página de información de la lista. Puede estar en formato HTML. Incluso si no utilizas este formato, utiliza la etiqueta `<br />` para introducir saltos de línea.
    -   **cabecera del mensaje**: cuando está disponible, se añade como un adjunto MIME al principio de cada mensaje distribuido a la lista;
    -   **pie de página del mensaje**: cuando está disponible, se añade como un adjunto MIME al final de cada mensaje distribuido a la lista;

Por defecto, Sympa utiliza archivos predefinidos; en este caso, los archivos específicos correspondientes a tu lista están vacíos. **Para editar un archivo, elígelo desde la lista desplegable y pincha en el botón 'Editar'**. Tendrás la posibilidad de cambiar el **campo 'From'** (remitente), el **campo 'Subject'** (asunto) y el **cuerpo del mensaje**.

| Note |
|------|
| Ten cuidado: los valores entre corchetes son variables. No las cambies, a no ser que sepas lo que realmente estás haciendo... |

#### <span id="manage_shared"></span>Gestionar el espacio web compartido de documentos

Por defecto, las listas no tiene espacio web compartido de documentos. Así que tienes que crearlo. Para hacerlo, ve al **módulo de administración** y pincha en el enlace '**Create shared**'.

Para permitir que los suscriptores publiquen documentos en el espacio web compartido, necesitas **cambiar los permisos por defecto**: en el módulo de administración de la lista, pincha en '**Editar configuración de la lista**' y luego en ''. Al principio de la página, existe un desplegable titulado '[**Quién puede editar**](listconfig.md#docsrights)'; elige la opción '**Restringido a suscriptores**'

| Note |
|------|
| Ten cuidado: si creaste carpetas antes de cambiar estos permisos, las carpetas seguirán sin poder escribirse en ellas. Si quieres que tengan permisos de escritura, tendrás que [cambiar los permisos de acceso](shared.md#acces) para cada carpeta. |

Puede que también quieras [establecer **cuotas**](listconfig.md#docsrights) para el espacio web compartido de docuemtnso en la página 'Privilegios' de la sección 'Editar configuración de la lista'.

Para **conocer todo lo necesario para la gestión del espacio web compartido de documentos**(cómo organizarlo, cambiar permisos de acceso, nombres de documentos, etc.), revisa la sección '[Utilizar el espacio web compartido de documentos](shared.md)' de la Guía de usuario.

Para **prohibir el acceso al espacio web de documentos compartidos**, haga clic en '**Eliminar documentos compartidos**' en el submenú 'Admin'. Todavía podrás **restaurarlo** haciendo clic en '**Restaurar documentos compartidos**'. La eliminación o restauración del espacio web de documentos compartidos **no tiene impacto en los documentos que éste contiene**.

#### <span id="manage_members"></span>Gestionar suscriptores

Esta sección te permite mostrar el **listado de suscriptores de la lista**. Cada suscriptor dispondŕa de la siguiente información:

-   **dirección de correo**
-   **dominio** de la dirección de correo (*@cru.fr*, *@sympa.org*, *@fai.com*, etc.);
-   **foto** (en caso de haberse activado esta funcionalidad para la lista);
-   **nombre** (según se haya realizado la suscripción, esta información podría no estar disponible);
-   [**modo de envío de mensajes**](#deliverymode);
-   **fuente de datos** indicando el origen en caso de que el suscriptor esté incluido o suscrito diréctamente;
-   **fecha de la suscripción** a la lista;
-   **última actualización** de las opciones del suscriptor.

| Note |
|------|
| Por defecto, cada página muestra 25 suscriptores. Puedes navegar a través de las páginas utilizando las flechas de navegación o mostrando más suscriptores en cada página. Puedes también reordenar la lista de suscriptores según diferentes criterios pinchando en la correspondiente cabecera de cada columna. |

Para **buscar a un suscriptor**, introduce todo o parte de su dirección de correo o de su nombre en la casilla y pincha en el botón '**Buscar**'.

Puedes **suscribir otra gente a la lista** desde esta página:

-   Parsa añadir **una única persona**, introduce su dirección de correo en la casilla y pincha en el botón '**Añadir**'.
-   Para añadir **varias personas**, pincha en el botón '**Añadir varios**'. En la casilla que se muestra, introduce una dirección dec orreo y el nombre de cada persona que quieras suscribir en la lista y pincha '**Añadir suscriptores**'.

| Note |
|------|
| Si quieres suscribir a gente sin que sea avisada de ello, activa la casilla 'Silencioso'. Sin embargo, ¡es mejor avisar a la gente que la estás suscribiendo a la lista! |

A pesar de que tienes la posibilidad de que la gente se suscriba a tu lista de correo, siempre **es mucho mejor que la gente realice los pasos necesarios para suscribirse ellos mismos** a la lista. También puedes **invitar a gente a que se suscriba a la lista** a través del comando INVITE: envia un email a {{conf.email}}@{{conf.host}} y escribe el siguiente comando en el cuerpo del mensaje:**invite nombredelalista direcciondecorreo**(ejemplo:*invite list\_example john.doe(@)fai.com*).

Para **aceptar o rechazar una solicitud de suscripción a la lista**, pincha en '**suscripciones pendientes**'. Se mostrará un listado con toda la gente que ha solicitado la suscripción a la lista. Para acetar o rechazar una solicitud, activa la caja situada al lado del nombre de la persona y pincha en el botón de tu elección.

Para **enviar un recordatorio de suscripción a todos los suscriptores**, pincha en el botón '**Recordar a todos**'. El mensaje recordatorio de suscripción contiene:

-   el **nombre de la lista** a la que pertenece el suscriptor;
-   la **dirección de correo** con la que se ha suscrito el suscriptor.
-   la **contraseña de lista** del suscriptor;
-   un **enlace a la página de información** de la lista;
-   una **dirección con un enlace para que los suscriptores puedan darse de baja** de la lista.

| Note |
|------|
| También puedes configurar un recordatorio de suscripción automático a travéz de la página '[Miscelánea](listconfig.md#other)' de la sección 'Editar configuración de la lista'. |

Para **dar de baja suscriptores** desde esta página, selecciónalos activando la caja situada al lado de sus nombre y haz clic en el botón '**Borrar las direcciones de correo seleccionadas**'.

| Note |
|------|
| Si no quieres notificar a los suscriptores, activa la caja 'Silecioso'. Sin embargo, esto no es recomendable a excepción del caso de suscriptores con mensajes rebotados. |

| Note |
|------|
| Truco: para seleccionar todos los suscriptores a la vez, primero asegúrate que se muestran todos en la página, y luego pincha en el botón 'Invertir selección':¡todos los suscriptores se seleccionarán en un único click! |

Para **cambiar las opciones del suscriptor**, pincha en su dirección de correo.

Desde esta página, puedes **cambiar el nombre, la dirección de correo y el modo de entrega de mensajes del suscriptor**. También puedes **darlo de baja**.

si el suscriptor está [rebotando mensajes](#manage_bounces), se muestra otro formulario bajo el formulario 'Información del Suscriptor':

La información mostrada incluye:

-   el tipo de error (en Inglés);
-   el número de errores;
-   el periodo en el que ocurrieron los errores.

Puedes **comprobar el último error** o **reiniciar los errores**. Si reinicias los errores, el [contador](listconfig.md#bouncers) del suscriptor se establecerá a cero.

Para gestionar más fácilmente las direcciones que generan rebotes, ve a la página '[Rebotes](#manage_bounces)' del módulo de administración de la lista.

#### <span id="manage_bounces"></span>Gestionar rebotes

Cuando hay un **problema con las direcciones de correo electrónico de los suscriptores** (direcciones de correo electrónico obsoletas, direcciones temporalmente indisponibles cuando se enviaron los mensajes, cuota del buzón de entrada superada, etc.), el porcentaje de direcciones con rebotes se muestra en el menú lateral izquierdo bajo el nombre de '**Porcentaje de errores**'. Para comprobar las direcciones con rebotes, ve a la página '**Rebotes** del módulo de administración de la lista.

Sympa gestiona automáticamente a los suscriptores con rebotes: según el número de errores y el tráfico de la lista, los suscriptores con rebotes son notificados, desuscritos, o su contador se reinicia a cero cuando sus direcciones paran de rebotar mensajes.

Para **hacer que las direcciones de correo paren de rebotar mensajes**, selecciónalas activando sus casillas y pinchando en el botón '**Reiniciar errores para los usuarios seleccionados**'. Si los errores persisten, las direcciones volverán a informarse como direcciones con rebotes tan pronto como un mensaje se mande a la lista.

También puedes **dar de baja suscriptores cuyas direcciones de correo siguen rebotando**: demasiadas direcciones con rebotes provocan una carga considerable en los servidores de listas de correo. Para dar de baja suscriptores, selecciónalos activando las casillas delante de sus nombres y haz clic en el botón '**Borrar direcciones de correo seleccionadas**'.

| Note |
|------|
| Truco: para seleccionar todos los suscriptores a la vez, primero asegúrate que se muestran todos en la página, y luego pincha en el botón 'Invertir selección':¡todos los suscriptores se seleccionarán en un único click! |

#### <span id="moderate"></span>Moderar mensajes enviados a la lista

Cuando una lista es moderada, **todos los mensajes deben ser aprobados por uno de los moderadores antes de ser distribuidos a la lista**· Después de enviar un mensaje a la lista, se notifica automáticamente a los los suscriptores por correo indicando que su mensaje será moderado. Para los moderadores, también reciben una notificación de Sympa, la cual incluye el mensaje a moderar.

Puedes **realizar operaciones de moderación** tanto **por email**, respondiendo el mensaje recibido de sympa, o **a través de la interfaz web del servidor de listas**. Para hacer eso, pincha en el enlace '**Mensaje**' del submenú 'Moderar': se te dirigirá a una página que muestra todos los mensajes que necesitan moderación (los mensajes más recientes están al principio de la página). **Para leer un mensaje, pincha en el asunto** .

Tienes **dos opciones**:

-   **autorizar la distribución del mensaje** a la lista;
-   **rechazar el mensaje y notificar al remitente**: cuando rechazas un mensaje, es mejor notificárselo al remitente...

Todos los moderadores pueden decidir si distribuir un mensaje o no. Sin embargo, **el primer moderador que procese el mensaje será el que tome la decisión**. Sympa te avisará si intentas procesar un mensaje que ya ha sido moderado. Cuando hay varios moderadores, es mejor **modrar los mensajes desde la interfaz web del servidor de listas de correo**: así,podrás ver los mensajes que quedan realmente por moderar.

| Note |
|------|
| **Independientemente de la fecha y hora de la moderación, la fecha y hora del envío del mensaje no varía**. Así, si la distribución del mensaje se aprueba con mucho retraso, ¡es posible recibir un mensaje datado el 1 de Enero el 31 de diciembre! |

En caso de que el mensaje se rechace con una notificación, el suscriptor que lo ha enviado es notificado por correo electrónico. Puedes [personalizar el mensaje que éste recibe](#customize).

Activando el casilla '**Rechazar sin notificación**' te permitirá prevenir que se notifique al autor del mensaje.

Activando la casilla '**Añadir a la lista negra**' añade al autor del mensaje a la lista negra de esa lista de correo y además omitir la notificación de rechazo. Puedes gestionar la lista negra a través del botón '**editar la lista negra**' en la parte inferior de la página.

Si deseas personalizra el mensaje de rechazo que se envía al autor del mensaje a moderar, puedes hacerlo a través del botón '**Gestionar mensajes de rechazo**. La página de gestión de mensajes permite definir un conjunto de mensajes de rechazo así como definir uno por defecto.

**Recuerda**: puedes [añadir o quitar moderadores](listconfig.md#description) a través del módulo de administración de la lista. Para hacer eso, desde la página de información de la lista, pincha en '**Admin**', en '**Editar configuración de la lista**', y luego en '**Definición de la lista**'.

También es posible **procesar mensajes tras su distribución a la lista**; esto puede ser útil cuando una lista no está moderada. Si quieres **borrar un mensaje**,[búscalo en el archivo we de mensajes](arc.md#arcsearch) y pincha en el botón '**Marcer este mail para borrado**' en la esquina superior derecha del mensaje. Se mostrará un mensaje de confirmación; pincha en 'OK'. El mensaje se borrará tras unos segundos.**Ten cuidado: ¡¡¡esta operación es irreversible!!!. Si borras un mensaje, no podrás recuperarlo.**

#### <span id="manage_archives"></span>Gestionar el archivo de mensajes

El gestor de listas de correo Sympa puede generar **archivos comprimidos descargables (formato .ZIP) de los mensajes enviados a la lista**. Para descargar esos archivos, **selecciona el mes** que te interesa en la lista y pincha en el botón '**Descargar archivo ZIP**'.

| Note |
|------|
| Nota: en la lista 'Selección de archivo', para seleccionar todos los meses durante los que se han enviado mensajes, pincha en el primer mes, mantén pulsada la tecla SHIFT y pincha en el último mes de la lista. |

Recibirás un archivo del tipo '**nombredelalista\_archive.zip**' que contiene **una carpeta llamada nombredelalista\_año-mes**(ejemplo: *lista\_ejemplo\_2005-06*por cada mes. Dentro de cada carpeta, **el nombre de los archivos son números** correspondiendo a la posición del mensaje según posición cronológica de fecha de envió (ejemplo: el archivo con nombre '1' contiene el primer mensaje enviado del mes). Los archivos de mensaje **no tienen extensión**; utiliza un editor de textos de tu elección (Bloc de Notas, WordPad, Vim, etc.) para abrirlo. **Cada archivo representa un mensaje completo (con todas las cabeceras)**.

Desde la página "Gestionar archivo", puedes también **borrar mensajes**(borrado mes a mes y no mensaje a mensaje). Para hacer esto, **selecciona los meses** que te interesan en la lista y pincha en el botón '**Borrar meses seleccionados**'.

| Note |
|------|
| **Ten cuidado: ¡¡¡esta operación es irreversible!!!. Cuando pinchas en 'Borrar meses seleccionados', ten en cuenta que no solo estas borrando un archivo, ¡¡¡sino también el archivo de mensajes del mes seleccionado!!!** |

#### <span id="renamelist"></span>Renombrar la lista

En el **módulo de administración de la lista**, pincha en '**Renombrar lista**'. Introduce el nombre que elijas y pincha en el botón 'Renombrar esta lista'. Se mostrará un mensaje de confirmación; pincha en 'OK'.

| Note |
|------|
| Si cambias de parecer, solo tendrás que realizar la operación inversa para volver al nombre anterior. |

**Ten cuidado: cuando renombras una lista, tienes que notificárselo a los listmasters; en caso contrario, el cambio no será efectivo**.

Algunos consejos para nombrar tus listas:

-   **No uses ningún espacio, acentos o caracteres especiales** en los nombres de lista: dichos caracteres pueden causar problemas.
-   Elige un **nombre explícito y corto**: piensa en los suscriptores que tendrán que escribir el nombre cada vez que quieran mandar un mensajes a la lista.
-   Si gestionas un conjunto de listas, puedes **utilizar un prefijo común para todas tus listas**; de esa forma se mostrarán juntas en los listados y serán fácilmente reconocibles (ejemplo: *xx-usuarios@{{conf.host}}, xx-lineadirecta@{{conf.host}}.es*, etc.).

#### <span id="supprlist"></span>Borrar la lista

En el **módulo de administración de la lista**, pincha en '**Borrar lista**'. Se mostrará un mensaje de confirmación; pincha en 'OK'.

| Note |
|------|
| **Ten cuidado: si borras la lista, ¡¡¡no podrás abrirla tu mismo!!!. Si quieres reabrir la lista, tendrás que consultar con los listmasters.** |

En términos reales, ¿cuales son las **consecuencias** de borrar una lista?

-   **Todos los suscriptores son automáticamente dados de baja** (incluyendo dueños y moderadores).
-   **El archivo de mensajes se mantiene** pero ya nadie puede acceder a él.
-   **Los documentos publicados en el espacio web compartido de documentos se mantienen** pero ya nadie puede acceder a ellos.
-   **Solo los listamsters tienen el poder de reabrir la lista**; si lo hacen, los suscriptores que anteriormente estaban suscritos a la lista serán automáticamente suscritos de nuevo.

| Note |
|------|
| Ten cuidado: debido a una pequeña latencia, las páginas de listas pueden permanecer accesibles por un tiempo si conoces sus direcciones. Después, serán completamente inaccesibles. |

**Si quieres que todos los archivos asociados se borren permanentemente**, debes preguntar a los listmasters.

### <span id="rulesadmin"></span>Buenas prácticas

Con la intención de hacer las listas dinámicas, **debes involucrarte activamente** en sus intercambios: si una lista no está controlada ni animada por sus dueños, puede ocasionar una pérdida de calidad en los mensajes e incluso sus suscriptores acaben fugándose...

**El uso del correo electrónico en general y para las listas de correo implica un conjunto de reglas precisas y necesarias para compartir comunicaciones agradables: la "Netiqueta"**. Como moderador o dueño de una lista, tu rol consiste en que los suscriptores las respeten. Encontrarás los principios generales de la Netiqueta, así como muchos enlaces en la [página de la Wikipedia dedicada a la Netiqueta](https://es.wikipedia.org/wiki/Netiqueta).

<span id="charter"></span>Debes **escribir unas condiciones de uso de tu lista** para definir todas las reglas que se aplicarán en su uso:

-   temas permitidos, tolerados y prohibidos;
-   escribir reglas (por ejemplo para especificar el lenguaje en que los suscriptores deben publicar, para banear "lenguaje SMS", etc.);
-   reglas que se aplican al enviar mensajes (periodicidad, adjuntos, etc.);
-   responsabilidades de suscriptores con respecto a la netiquette;
-   derechos y obligaciones de los suscriptores;
-   información sobre la retención de los mensajes enviados a la lista;
-   información legal y política de privacidad;
-   sanciones aplicables a aquellos que no respetaran las reglas de la lista;
-   ~~etc.~~

| Note |
|------|
| Con la intención de que todos lean las condiciones de uso de la lista, debes incluirla en el mensaje de bienvenida que se les envía después de suscribirse. Para hacer eso, necesitas [personalizar dicho mensaje](#customize) a través de la página 'Personalizar' del módulo de administración de la lista. |

Cuando esté disponible, la 'Carta a dueño y moderador' proporciona la información necesaria para que dueños y moderadores puedan desempeñar sus roles. Estas condiciones de uso indican todos los derechos y obligaciones de moderadores y dueños.

------------------------------------------------------------------------
