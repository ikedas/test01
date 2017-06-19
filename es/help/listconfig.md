<span id="listconfig"></span>Configurar la lista
------------------------------------------------

Como la configuración de la lista es un poco compleja, esta está dividida en varias partes con una página para cada parte:

-   [Definición de la lista](#description);
-   [Envío/Recepción](#sending);
-   [Privilegios](#command);
-   [Archivo](#archives);
-   [Rebotes](#bounces);
-   [Miscelánea](#other).

Te aconsejamos que **hagas cambios progresivamente**: así, si el resultado no coincide con lo que esperabas, será fácil retroceder.

El módulo de administración de la lista te ofrece **muchas opciones para configurar tu lista**. Sin embargo, estas opciones pueden no coincidir exactamente con tus necesidades. Para solucionar este problema, puedes **preguntar a los listmaster para crear nuevas opciones** (dentro de los límites en los que ellos puedan, naturalmente...): accesos o permisos limitados a algunas categorías de personas de acuerdo al lugar desde el que acceden, el dominio de sus direcciones de correo, el grupo de usuarios al que pertenecen, etc.

### <span id="description"></span>Definición de la lista

En el área de '**Asunto de la lista**', puedes cambiar el asunto que elegiste cuando creaste la lista. El asunto se muestra como cabecera de todas las páginas de lista, y también es visible en el índice de páginas de la lista (lista de listas, lista de tus suscripciones, etc.) y en la barra de títulos del navegador.

También puedes cambiar la '**Visibilidad de la lista**'. Las opciones disponibles son las siguientes:

-   Oculto salvo para los suscriptores (conceal) - *opción por defecto*;
-   acceso intranet (intranet);
-   sin ocultar (noconceal);
-   oculto incluos a los suscriptores (secret);

| Note |
|------|
| Si quieres limitar la visibilidad de la lista según otro criterio, debes preguntar a los listmasters: ellos pueden ser capaces de crear una nueva opción que coincida con tus necesidades (por ejemplo: lista visible solo por miembros de un grupo de usuarios, de un dominio de Internet, etc.). |

En las áreas de 'Dueños' y 'Moderadores', puedes **añadir dueños y moderadores** a la lista o **cambiar su información personal**:

-   Para cada dueño/moderador, tienes que indicar una **dirección de correo electrónico** y un **nombre**.
-   También puedes añadir la información que elijas en la casilla '**Información privada**' (número de teléfono, función, etc.); esta información solo será accesible para listmasters y los dueños de la lista con un perfil 'Privilegiado'.
-   Puedes cambiar el **modo de entrega de mensajes** (la únicas opciones disponibles en esta página son 'mail' y 'nomail').
-   El parámetro 'Perfil' no puede cambiarse: el **perfil 'Privilegiado'** está reservado para el creador de la lista (el resto de dueños tienen un perfil 'Normal').

| Note |
|------|
| Ten cuidado: convertirse en dueño o moderador de una lista no significa que automáticamente estés suscrito a la misma. De este modo los moderadores y dueños deben suscribirse ellos mismos a la lista. |

Para **borrar dueños/moderadores**, deja vacío las casillas correspondientes a las personas que quieres borrar y haz clic en el botón 'Actualizar'.

También puedes cambiar el **tema de la lista** así como su **lenguaje**. Si cambias el lenguaje de la lista, todo los mensajes predefinidos se enviarán en el idioma elegido (ten cuidado: ¡sujeto a la disponibilidad de una traducción!).

No puedes cambiar el **dominio de Internet** de la lista: solo los listmasters pueden cambiar este parámetro.

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** de la parte inferior de la página para aplicar todos tus cambios.

### <span id="sending"></span>Envío/Recepción

Desde esta página, puedes **decidir quien tendrá permiso para enviar mensajes a la lista**.

En el área '**Periodicidad de la recopilación**', puedes definir cada cuánto se envían los mensajes agrupados (modos de entrega Recopilación y Resumen): en la lista, selecciona todos los **días** en los que quieres que se envíen recopilaciones. Luego elige la **hora de entrega** de las recopilaciones (por favor, intenta evitar seleccionar una hora entre las 11 p.m. y la media noche).

En la lista '**Opciones de suscripción disponibles**', selecciona todas las opciones de suscripción que quieres ofrecer a tus usuarios. Por defecto, todas las opciones están seleccionadas.

El área '**Dirección de respuesta**' te permite definir los destinatarios por defecto de cualquier respuesta a un mensaje enviado a la lista.

-   Con el valor '**Todos**', la respuesta es envaida al **remitente del mensaje** Y a la **lista**.
-   Con el valor '**Lista**', la respuesta se envía a la **lista**.

    | Note |
    |------|
    | Ten cuidado: ¡utiliza esta opción cuidadosamente!. La experiencia dice que los suscriptores no siempre comprueban la dirección a la que envían su respuesta. Es decir, puede que envíen mensajes privados a la lista completa cuando intentan responder a una determinada persona... |

-   Con el valor '**Other\_email**', la respuesta se envía a una **dirección predefinida**. Si eliges esta opción, debes **indicar una dirección de correo en la casilla 'Otra dirección de correo'**.
-   Con el valor '**Remitente**', la respuesta se envía al **remitente del mensaje**. Esta es la opción que probablemente deberías elegir.

El desplegable '**Respetar una cabecera existente**' te permite elegir cómo la cabecera SMTP 'Reply-To' se procesará en los mensajes enviados a la lista. La opción '**Respetar**' mantiene el valor de dicha casilla mientras que la opción '**Forzar**' permite sobre escribirla.

Por último, la opción '**Etiqueta del Tema**' te permite elegir el **texto incluido antes del asunto todos los mensajes** enviados a la lista: esto permite a los suscriptores ordenar sus mensajes fácilmente, utilizar filtros de mensaje en ellos para procesar los mensajes automáticamente, etc. Por defecto, el texto consiste en el **nombre de la lista rodeado de corchetes** (los corchetes los añade automáticamente el sistema, así que no es necesario que los especifique usted mismo).

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** de la parte inferior de la página para aplicar todos tus cambios.

### <span id="command"></span>Privilegios

Desde esta página, puedes decidir:

-   **Quién puede ver información de la lista**. Las siguientes opciones están disponibles:
    -   para cualquiera (abierta) - *opción por defecto*;
    -   restringida a suscriptores (privada).
-   **quién puede suscribrse a la lista** . Están disponibles las siguientes opciones:
    -   solicitud de subscripción confirmada (auth);
    -   necesita autenticación (una notificación es enviada a los dueños) (auth\_notify);
    -   necesita autenticación y luego autorización del dueño (auth\_owner);
    -   suscribirse es imposible (closed);
    -   restringido al dominio local de usuarios (intranet);
    -   usuarios del dominio local o con autorización del dueño (intranetorowner);
    -   para cualquier sin autentificación (open) - *opción por defecto*;
    -   cualquiera, se envía notificación al dueño de la lista (open\_notify);
    -   cualquiera, sin mensaje de bienvenida (open\_quiet);
    -   aprobación del dueño (owner);
    -   requiere ser firmado en S/MIME (smime);
    -   necesita firma S/MIME o autorización del dueño (smimeorowner).

        | Note |
        |------|
        | Siempre debes elegir una opción que incluya el parámetro 'auth': de esta forma, el sistema solicita confirmación a los futuros suscriptores por email antes de suscribirlos a la lista. Esto evita suscripciones con direcciones de correo inválidas y garantiza que nadie puede ser suscrito a la lista sin su conocimiento. |

-   **quién puede suscribirse a la lista**. Están disponibles las siguientes opciones:
    -   necesita autentificación (auth);
    -   autentificación solicitada, notificación enviada al dueño (auth\_notify);
    -   imposible (closed);
    -   abierta (open) - *opción por defecto*;
    -   abierta con confirmación de mail, notificación al dueño (open\_notify);
    -   autorización del dueño (owner).

        | Note |
        |------|
        | Deberías elegir siempre alguna opción con el parámetro 'auth': de esta forma, el sistema requiere la confirmación del suscriptor por correo electrónico antes de darlo de baja de la lista. Esto previene que gente mal intencionada de de baja a otros usuarios sin su conocimiento. |

-   **quién puede invitar gente a suscribirse a la lista**. Están disponibles las siguientes opciones:
    -   cerrado (closed);
    -   dueño de la lista, sin autenticación (owner)
    -   restringido a suscriptores (private) - *opción por defecto*;
    -   público (public).
-   **quién puede revisar los suscriptores**. Están disponibles las siguientes opciones:
    -   nadie puede revisar (closed);
    -   reservado a suscriptores o usuarios del dominio local (intranet);
    -   sólo listmaster (listmaster);
    -   solo el dueño (y listmaster) (owner) - *opción por defecto*;
    -   restringido a subscriptores (private);
    -   cualquiera puede hacerlo (public).

        | Note |
        |------|
        | No deberías hacer que la lista de miembros fuese accesible a cualquiera. La opción 'Restringido a suscriptores' puede ser interesante para permitir a los suscriptores comunicarse entre ellos sin necesidad de publicar mensajes a la lista. Sin embargo, no es apropiado en el caso de una lista de notificaciones que incluya a suscriptores que no tenga una relación particular entre ellos. |

<span id="docsrights"></span>Desde esta página, también puedes **definir los permisos de acceso que se aplicarán al espacio web compartido de documentos** (La sección 'Documentos compartidos' de la lista, accesible a través del enlace situado en el menú lateral izquierdo). Puedes definir tanto permisos de escritura como de lectura sobre los documentos:

-   Las siguientes opciones están disponbiles en el desplegable '**Quién puede ver**'
    -   reservado a suscriptores o usuarios del dominio local (intranet);
    -   reservado a los dueños de la lista (owner);
    -   restringido a suscriptores (private) - *opción por defecto*;
    -   documentos públicos (public).
-   Las siguientes opciones están disponibles en el desplegable '**Quién puede editar**':
    -   reservado a los dueños de la lista (owner) - *opción por defecto*;
    -   moderado para los suscriptores (editor);
    -   restringido a subscriptores (private);
    -   documentos públicos (public).

La casilla de entrada '**Cuota**' te permite definir un **tamaño máximo que no podrá excederse en el espacio de documentos compartidos**. Este tamaño no representa el tamaño máximo de *un* documento publicado en el espacio de documentos compartidos, sino el tamaño máximo de todos los documentos publicados en la lista. Está expresado en kilobytes. Cuando un suscriptor intenta publicar un documento muy grande superando este espacio, obtiene un mensaje de error.

Para conocer **más sobre la gestión del espacio de documentos compartidos** (cómo organizarlo, cambiar sus reglas de acceso, nombrar documentos, etc.) por favor, revise la sección '[Usar el espacio de documentos compartidos](shared.md)' de la Guía de usuario.

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** de la parte inferior de la página para aplicar todos tus cambios.

### <span id="archives"></span>Archivo

Desde esta página, puedes **decidir quién puede acceder al archivo web de la lista** (mensajes legibles en la interfaz web de la lista de correo). Están disponibles las siguientes opciones:

-   cerrado (closed);
-   restringido al dominio local de usuarios (intranet);
-   ~~listmaster (listmaster);~~
-   dueño (owner);
-   moderador (moderator);
-   sólo para suscriptores (private);
-   público (public).

La casilla '**Cuota**' te permite definir un **tamaño máximo para el archivo de los mensajes**. Este tamaño está expresado en kilobytes. Se notifica a los dueños de la lista cuando el tamaño del archivo supera el 95 % del tamaño permitido. Cuando se alcanza el tamaño máximo, los mensajes enviados posteriormente no se archivan.

| Note |
|------|
| Aunque se pare el archivado, naturalmente sigue siendo posible enviar mensajes a la lista. |

También es posible **acceder al archivo de la lista por correo electrónico**, enviando a **{{conf.email}}@{{conf.host}}** el siguiente comando: <span class="commande">**GET nombredelalista año-mes**</span> (example: *GET list\_example 2016-07*). Entonces recibirás una recopilación de todos los mensajes enviados durante el mes elegido. Esta recopilación se envía en texto sin formato y contiene etiquetas HTML en vez del formato original; también incluye todas las cabeceras de cada mensaje. Los parámetros de '**archivos de texto**' te permiten definir:

-   **quien está autorizado** para recibir mensajes de la lista por email;
-   **con qué periodicidad se crearán los ficheros de archivo**. Por ejemplo, si la periodicidad se establece a 'mensual', todos los mensajes distribuidos a la lista en un mes se agruparán en un único fichero de archivo.

Si este parámetro no está definido, la lista no tendrá accesibles los archivos por email. Ten cuidado: **solo los listmasters tienen el poder de cambiar este parámetro.**

Es posible enviar **mensajes encriptados en S/MIME** a la lista. La opción '**Archivar mensajes encriptados como texto claro**' te permite definir cómo se archivarán dichos mensajes:

-   La opción '**Descifrado**' archiva el mensaje tras quitar la encriptación.
-   La opción'**Original**' archiva el mensaje conservando la encriptación original.

Esta opción se aplica tanto al archivo de texto como al archivo web, así como en las recopilaciones que se envían a los usuarios que tengan activado el modo de entrega 'Recopilación'.

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** al final de la página para guardar todos los cambios.

### <span id="bounces"></span>Rebotes

"**Rebotes**" representa a aquellos **suscriptores con dirección de corre errónea**, es decir suscritores que no reciben los mensajes enviados a la lista. Esta situación puede estar causada por varias razones: direcciones de correo obsoletas, cuentas temporalmente no disponibles cuando se enviaron los mensajes, cuota de carpeta de entrada excedida, etc.

La sección de '**Gestión de rebotes**' define dos ratios:

-   La **tasa de aviso** indica la tasa de direcciones de correo electrónicos rebotadas (con errores) por el cual el dueño de la lista recibirá un **aviso titulado 'Tasa de rebotes demasiado alta'** invitandándole a borrar dichos suscriptores de la lista.
-   El **ratio de stop** indica el ratio de direcciones de correo con correos rebotados por el cual **la distribución de mensajes se parará automáticamente** hasta la resolución del problema (generalmente borrando a los suscriptores implicados).

<span id="bouncers"></span>Las secciones '**Gestión de rebotes, 1er nivel**' y '**Gestión de rebotes, 2º nivel**' te permiten realizar tareas automáticas para controlar los rebotes de los suscriptores. Puedes definir:

-   los **rangos de tasas que definen el nivel 1 y el nivel 2 de rebotes**. Por defecto, el nivel 1 de rebotes tiene una tasa comprendida entre 45 y 75, y el nivel 2 tiene una tasa comprendida entre 75 y 100;

    | Note |
    |------|
    | La tasa depende del número, tipo y frecuencia de los errores. Si el tiempo entre rebotes es demasiado corto o si han habido muchos errores, no se asigna una tasa al rebote. |

-   la **tarea a realizar sobre los suscriptores involucrados**: sin tarea, notificación, borrado de la lista;
-   la **persona a notificar** cuando una tarea se lleva a cabo: nadie, los dueños, el listmaster. La notificación enviada cuando una tarea se lleva a cabo incluye los nombres de todos los suscriptores involucrados así como información precisa sobre la tarea.

**Para gestionar rebotes** (reiniciar el contador para determinados usuarios, dar de baja suscriptores con errores, solicitar un recordatorio de suscripción, etc.) **ve a la página de [Rebotes](admin#manage_bounces.md)** del módulo de administración de la lista.

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** al final de la página para guardar todos los cambios.

### <span id="other"></span>Miscelánea

La opción '**Tarea periódica de expiración de suscripción**' te permite definir un **tiempo límite para la expiración automática de las suscripciones** a la lista: por defecto (ejemplo: una vez al año), los suscriptores recibirán un mensaje preguntándoles si quieren renovar su suscripción a la lista. Si no la renuevan, serán dados de baja automáticamente. Este procedimiento asegura que toda persona suscrita a la lista está realmente enterada de su existencia e interesada en la misma.

La opción '**Tarea periódica de recordatorios de suscripción** te permite **enviar recordatorios de suscripción** a los miembros de la lista.

La opción '**método de protección de las direcciones de correo**' asegura que las direcciones de correo de los suscriptores no podrán ser recolectadas por robots de spam. Esta opción se aplicará a todas las páginas de la lista.

En esta página, también puedes ver **información sobre la última actualización de la lista** (quién la hizo y cuando), así como el **número de cambio de la configuración** desde que la lista fue creada.

**TEN CUIDADO: no olvides pinchar en el botón 'Update'** de la parte inferior de la página para aplicar todos tus cambios.
