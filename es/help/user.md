Listas de Correo - Guía de Usuario
----------------------------------

### <span id="howitworks"></span>Cómo funciona el servicio de listas de correo

El servicio de listas de correo está gestionado por un **sofware de listas de correo: Sympa**. El software viene con un **entorno web de listas de correo**.

**Para realizar acciones relacionadas con las listas de correo**(suscripción, chambiar tus opciones, etc.), tienes dos opciones:

-   **Entrar en el entorno web**;
-   **enviar comando por email** al gestor de listas de correo Sympa **{{conf.email}}@{{conf.host}}**

**Para enviar un comando a Sympa**, haz lo siguiente:

-   **Is mandas un solo comando**, escríbelo en el Asunto del mensaje y deja el cuerpo del mensaje en blanco.
-   **Si mandas varios comandos**, deja el Asunto del mensaje en blanco y escribe todos los comandos dentro del cuerpo del mensaje.**Ten cuidado**: Sympa no procesará tu mensaje si no respetas las siguientes reglas:
    -   Escribe cada comando en una nueva línea.
    -   Envía tu mensaje en texto plano (sin formato), no en HTML.
    -   Tu mensaje no puede contener otra cosa que no sean comandos Sympa (no se debe incluir ninguna firma).

Una descripción de todos los comandos que puedes enviar a Sympa está disponible en [file:///help/mail\_commands](mail_commands.md).

### <span id="subscribe"></span>Suscripción a listas de correo

La suscripción a una lista de correo es muy simple:

1.  **Elige la dirección** con la que quieres suscribirte a la lista.

    | Note |
    |------|
    | Debes escoger una dirección que compruebes frecuentemente a que ofrezca una buena capacidad de almacenamiento para tus email: algunas listas distribuyen muchos mensajes, los cuales a veces contienen adjuntos grandes. |

    | Note |
    |------|
    | Por supuesto puedes suscribirte en una misma lista con distintas cuentas de correo. En ese caso necesitarás repetir el proceso de suscripción por cada dirección de correo diferente. |

2.  Envia un **mensaje a {{conf.email}}@{{conf.host}}** desde la dirección que quieres suscribir a la lista.

    | Note |
    |------|
    | Sympa no es una persona sino un robot de gestión de listas de correo. Así que no sirve de nada enviarle palabras cariñosas! ;-) |

3.  En el asunto del mensaje, escribe: **subscribe nnombredelalista Nombre Apellidos** (cambia 'nombredelalista' por el nombre de la lista a la que te quieres suscribir e indica tu propio Nombre y Apellidos).
4.  **Deja el cuerpo del mensaje en blanco**.

    | Note |
    |------|
    | Para ahorrar tiempo, puedes enviar varios comandos en un mismo mensaje. Para hacer eso, sigue las instrucciones disponibles en la sección [Cómo funciona un servicio de listas de correo](howitworks) |

**Después de esto, recibirás un mensaje diciéndote si tu solicitud ha sido aceptada o no**: si la suscripción de la lista está sujeta a algún tipo de aprobación, el dueño de la lista debe decidir si te suscribe o no. Si es así, no envíes varias solicitudes: no sirve de nada ya que obtendrás el mismo resultado. Ppuedes posiblemente enviar un mensaje directamente al dueño de la lista (nombredelalista-request@{{conf.host}}) para explicar por qué quieres ser suscriptor de la lista...

| Note |
|------|
| Nota: algunas veces tendrás que confirmar tu solicitud de suscripción antes de que sea procesada. Si es así, por favor sigue las instrucciones que se indican en el mensaje que hayas recibido. |

Según el tipo de lista (lista con suscriptores sujetos a condiciones o no) y a la disponibilidad del dueño de la lista, **puede que no recibas noticias inmediatamente**. No sirve de nada enviar varias solicitudes.

**Si se acepta tu solicitud, el mensaje que recibirás confirmará tu suscripción a la lista. Éste mensaje**(la carta de bienvenida)**contiene varias piezas de información esencial:**

-   tu **contraseña de la lista**. Esta contraseña es la misma para todas las listas a las que estés suscrito con una misma cuenta de correo. Puedes [cambiarla en la web](#global_pref "Cómo cambiar tu contraseña") después de acceder al servidor de listas de correo;
-   **información detallada sobre la lista**: su propósito, la dirección de internet donde están disponibles el archivo de mensajes, etc.
-   las **reglas aplicables a la lista y a sus miembros**: temas permitidos y prohibidos, información legal, políticas de privacidad, etc.

**Debes guardar tu notificación de suscripción**: puede que la necesites antes para recordar tu contraseña o para enviar un comando preciso a Sympa (ejemplo: comando signoff). En gteneral, **te recomendamos que guardes todas tus notificaciones de suscripción a listas de correo**.

**Puedes también suscribirte a una lista a través de la interfaz de la lista de correo**. Para hacer eso, haz lo siguiente:

1.  Ve a la [página principal](%7B%7Bpath_cgi%7D%7D/home) del entorno web y **accede**.
2.  **Ve a la página información de la lista** de la que quieres suscribirte.
3.  En el menú lateral izquierdo, **haz clic en el enlace 'Suscribir'**.

### <span id="sympa_auth"></span>Entrar en el entorno de listas de correo

Para entrar al entorno de listas de correo, utilice el formulario de autenticación situado encima de la columna izquierda de la interfaz web. Cuando hayas entrado, ahí se mostrará tu dirección de correo electrónica y perfil de usuario (suscriptor, moderador o dueño).

El proceso de autenticación varía según tu situación personal:

-   **Si la organización que ofrece el servicio de listas de correo utiliza tecnología de Single sign-on** (una única cuenta y una única autenticación, por jemplo a travéz de un sistema CAS), preferirás entrar con tu cuenta única. Para hacer eso, pincha en el botón "Ir" al lado del testo '**Autenticación \[nombre del sistema utilizado\]**'. Entonces, escribe tu correo electrónico y contraseña para entrar al servidor de autenticación.

    | Note |
    |------|
    | Si ya has entrado en otro servicio que esté utilizando el mismo sistema de autenticaión, tu autenticación será automática. Refresca la página si es necesario. |

-   **Si no se aplica ningún proceso de autenticación única deberás utilizar tu contraseña de lista.** En ese caso, entra a través del método clásico: introduce la **dirección de correo con la que te suscribiste a la lista** como login y tu **contraseña de lista** en la casilla 'Contraseña'.

    | Note |
    |------|
    | Si no recuerdas tu contraseña de lista, haz clic en '¿Contraseña perdida?'. Después de indicar tu dirección de correo, recibirás un correo con una URL de validación. |

-   **Si el proceso de autenticación única no se te aplica y no tienes una contraseña todavía**, haga clic en '**¿Primer acceso?**' y escribe tu dirección de correo electrónica. Recibirás una URL de confirmación en esa dirección. Entonces podrás elegir tu contraseña.

| Note |
|------|
| Recuerda: la contraseña de lista es una contraseña especial que solo utilizarás para el servicio de listas de correo. |

### Comprobar tus suscripciones

Para ver todas las listas a las que estás suscrito, necesitas [acceder](#syma_auth) primero. Posteriormente se mostrará un listado de todas tus listas, incluyendo una breve descripción de cada una de ellas, en el formulario "Tus listas" de la columna izquierda.

**Para ver la página de información de una lista, pincha en el nombre de la misma**. La página de información incluye una descripción de la lista( objetivo, reglas aplicables cuando se envía un mensaje, etc.), cuya longitud variará según la lista.

Desde esta página de información, podrás:

-   cambiar tus [opciones de suscriptor](#options);
-   leer el [archivo de mensajes de la lista](arc.md)
-   [enviar un nuevo mensaje](file:///help/arc#arcsearch%3Ebuscar%20en%20el%20archivo%20de%20mensajes%3C/a%3E;%3C/li%3E%0A%20%20%20%20%20%20%20%20%3Cli%3E%3Ca%20href=);
-   [descargar documentos](shared.md#shared_read) desde el espacio web compartido de documentos;
-   [subir documentos](shared.md#shared_upload) al espacio de documentos compartidos;
-   [revisar los miembros](#subscribers) de la lista (en caso de estar disponible)
-   [suspender o reanudar](suspend.md) tu subcripcion a cada lista;
-   [darte de baja](#unsubscribe) de la lista.

<span id="subscribers"></span>El **número de personas suscritas** a la lista se muestra permanentemente en el **menú izquierdo**. **Para revisar los miembros de la lista, haz clic en el enlace 'Revisar miembros'** del menú izquierdo (si los dueños de la lista deciden denegar el acceso al listado de suscriptores, este enlace no estará disponible). El listado de suscriptores muestra las **direcciones de correo electrónico** y el **nombre** de cada uno de los suscriptores (la indicación del nombre depende del método de suscripción utilizado por los suscriptores).

| Note |
|------|
| Por defecto, cada página muestra 25 suscriptores. Puedes navegar a través de las páginas utilizando las flechas de navegación o mostrar más suscriptores por página. También podrás ordenar los suscriptores según la dirección de correo, dominio o nombre pinchando en la correspondiente cabecera de columna. |

**Los nombres de la lista de dueños y moderadores se muestra en el menú lateral izquierdo**. Nunca debes escribir directamente a lo dueño o moderador de la lista. Si quieres realizar alguna pregunta o hacer algún comentario, deberías utilizar la siguiente dirección: **nombre\_lista-request@{{conf.host}}** (cambia 'nombre\_lista' por el nombre de la lista en cuestión).

Para saber **cuando te suscribiste a la lista** y **cuando has actualizado por última vez tus opciones de suscripción**, **haz clic en el enlace "Opciones del suscriptor"** en el menú lateral izquierdo.

### <span id="pref"></span>Gestionar tus preferencias

Para **simplificar el uso de las listas**,**puedes definir una serie de preferencias personales**. Existen dos tipos de preferencias que puedes cambiar:

-   tus **opciones de suscriptor**, las cuales pueden variar según la lista;
-   tus **preferencias generales**, las cuales se aplican a todo el entorno de listas de correo Sympa.

#### <span id="options"></span>Cambiar tus opciones de suscriptor

**Tus opciones de suscriptor pueden variar de una lista a otra**. Para cambiarlas, haz lo siguiente:

1.  Ve a la [página principal](%7B%7Bpath_cgi%7D%7D/home) del entorno web y **accede**.
2.  **Ve a la página de información de la lista** en la que quieres cambiar tus opciones de suscriptor.
3.  En el menu lateral izquierdo, **haz clic en el enlace 'Opciones del suscriptor'**.
4.  <span id="deliverymode"></span>&lt;**Cambia el modo de recepción de mensajes** (estas opciones son mutuamente excluyentes, así que no puedes seleccionar varias a la vez):
    -   **recopilación en formato MIME**: en vez de recibir los mensajes de la lista de forma normal, recibirás regularmente una recopilación de ellos. Esta recopilación aglutina un grupo de mensajes de la lista, utilizando el formato MIME multiparte. La periodicidad de la recopilación la establece el dueño de la lista.
    -   **recopilación en texto sin formato**: en vez de recibir los mensajes de la lista de forma normal, recibirás regularmente una recopilación de ellos. La recopilación aglutina un grupo de mensajes de la lista, utilizando texto sin formato. La periodicidad de la recopilación la establece el dueño de la lista.
    -   **modo resumen**: en vez de recibir los mensajes de la lista de forma normal, tendrás regularmente un listado de ellos. Para leer los mensajes, debes navegar por el archivo web de la lista.
    -   **modo de notificación**: con este modo, recibirás todos los mensajes con el cuerpo del mensaje en blanco: de esta forma se te informa de cada mensaje enviado a la lista en tiempo real, sin riesgo de inundar tu carpeta de entrada.
    -   **no mail (útil para las vacaciones)**: este modo hace posible que no recibas mensajes de la lista. Es especialmente útil cuando no tienes acceso a tu correo durante un periodo largo de tiempo y sin embargo quieres mantenerte suscrito a la lista.
    -   **modo sólo texto**: este modo permite recibir únicamente la versión en texto (text/plain) de un mensaje enviado en varios formatos (texto sin formato y HTML).
    -   **modo sólo HTML**: este modo permite recibir sólo la versión HTML de mensajes enviados en ambos formatos.
    -   **modo URLizado**: este modo permite no recibir documentos adjuntos. Sin embargo estos documentos están disponibles en el archivo de la lista y puedes acceder a ellos a travéz de la URL proporcionada en el mensaje.
    -   **no recibes tus propios mensajes**: este modo permite no recibir una copia de tus propios mensajes.
    -   **estandar (recepción directa)**: este modo es el modo de entrega por defecto; éste modo cancela cualquier otro modo de entrega:
    -   suspendido : este modo le permite suspender su suscripción a una o más listas por un período determinado o no. A diferencia de darse de baja, puede realizar un seguimiento de su suscripción y reactivarla en cualquier momento visitando la sección "Administrar su suscripción".
5.  **Cambiar las opciones de visibilidad**:
    -   **listado en la página de revisión de la lista**: tu nombre y dirección de correo electrónico se mostrarán en el listado de miembros (si el dueño de la lista permitió a los suscriptores revisar los miembros de la lista).
    -   **ocultado**: tu nombre y dirección de correo no se mostrará en la lista de suscriptores. Sin embargo, tu dirección de correo será visible en el archivo de mensajes de la lista si envías uno.
6.  **Pincha en el botón 'Actualizar'**.

#### <span id="global_pref"></span>Cambiar tus preferencias generales

Las preferencias generales se aplican a todas las suscripciones así como la forma en que la interfaz de tu servidor de listas Sympa lo muestra. Para cambiar tus preferencias, haz lo siguiente:

1.  Ve a la [página principal](%7B%7Bpath_cgi%7D%7D/home) del entorno web y **accede**.
2.  En el formulario mostrado encima de la columna izquierda, **haz clic en el enlace 'Tus preferencias'**
3.  **Cambia tus preferencias**
4.  **Pincha en el botón 'Enviar' de cada opción** que cambias.

Puedes cambiar:

-   tu **nombre**: si te suscribes a una lista desde la interfaz web del servidor de listas, el campo 'Nombre' se rellenará automáticamente en la lista de suscriptores;
-   el **lenguaje que deseas para la interfaz web** (puedes cambiar el lenguaje en cada página de la interfaz web; tu elección se mantendrá incluso si cambias el lenguaje en otra página distinta a la página de 'Preferencias';
-   el **tiempo de vida de la cookie colocada por Sympa en tu navegador** ('Periodo de caducidad de la conexión'). Por defecto, la sesión caduca cuando cierras el navegador; si usas el servicio de listas con frecuencia, te recomendamos que elijas un tiempo de duración mas largo;

    | Note |
    |------|
    | Una cookie es un pequeño fichero que el servidor web guarda en tu disco duro, normalmente de forma temporal, con la intención de identificarte como un usuario del servicio. Contiene pequeñas piezas de información sobre tí: nombre, dirección de correo, última vez que accediste, etc. |

-   la **dirección de correo con la que te suscribes** a las listas (si te suscribes con distintas direcciones de correo, la dirección se cambiará a la dirección con la que hayas entrado);

    | Note |
    |------|
    | Ten cuidado: esta acción cambiará tus suscripciones a todas tus listas. Si quieres cambiar la dirección de una única lista de correo, es mejor que te des de baja de la lista y te suscribas de nuevo con la dirección de correo electrónica correcta. |

-   tu **contraseña de lista**.

La sección '**Tus otras direcciones de correo**' actua como un cambio de dirección de correo.

### Buscar una lista de correo

Puede que necesites buscar una lista de correo. Para hacerlo, tienes tres opciones:

-   **navegar por las diferentes secciones** mostradas en [el inicio del entorno web de la lista](%7B%7Bpath_cgi%7D%7D/home);
-   buscar una lista a travéz del **campo de búsqueda**: la cadena buscada devolverá todas aquellas listas cuyo nombre o descripción coincida con tu criterio de búsqueda (las descripciones de las listas generalmente consisten en sentencias cortas);
-   pinchar en la pestaña '[Lista de listas](%7B%7Bpath_cgi%7D%7D/lists)' al inicio de la página para **mostrar todas las listas disponibles**.

| Note |
|------|
| Según el dominio al que pertenezca tu dirección de correo (ejemplo: *cru.fr*, *fai.com*,etc.) y a la localización a la que perteneces, no tendrás acceso a las mismas listas. Sin embargo, puedes suscribirte a una lista que no se muestra si conoces el nombre. Para hacer esto, [utiliza tu cliente de correo](#subscribe). |

### <span id="archives"></span>Leyendo un archivo web de la lista

Por favor revisa la [**documentación del archivo**](arc.md)

### <span id="sendmsg"></span>Enviar un mensaje

Por favor revisa la [**documentación sobre envío de mensajes**](sendmsg.md)

### <span id="shared"></span>Utilizar el espacio web compartido de documentos

Por favor revisa la [**documentación sobre espacio web compartido de documentos**](shared.md).

### <span id="suspend"></span>Suspendidiento o continuando tu suscripción de cada lista

Por favor revisa la [**documentación de administración de la suscripción**](suspend.md)

### <span id="unsubscribe"></span>Desuscripción de listas

Para darte de baja de una lista, haz lo siguiente:

1.  Desde la dirección de correo con la que estás suscrito a la lista, envía un **mensaje a {{conf.email}}@{{conf.host}}**.
2.  En el campo asunto de tu correo electrónico, escribe: **unsubscribe nombre\_lista** (cambia 'nombre\_lista' por el nombre de la lista de la cual te quieres dar de baja).
3.  **Deja el cuerpo del mensaje en blanco**.

    | Note |
    |------|
    | Para ahorrar tiempo, puedes enviar varios comandos en un mismo mensaje. Para hacer eso, sigue las instrucciones disponibles en la sección [Cómo funciona un servicio de listas de correo](howitworks) |

También puedes darte de baja a través de la interfaz web de las listas de correo (necesitarás repetir la operación por cada lista de la que te quieras dar de baja):

1.  Ve a la [página principal](%7B%7Bpath_cgi%7D%7D/home) del entorno web y **accede**.
2.  **Ve a la página de información de la lista** de la que quieres darte de baja.
3.  **En el menú lateral izquierdo, haz clic en el enlace 'Darse de baja'**.

------------------------------------------------------------------------
