### Preguntas frecuentes (FAQ) de usuarios

#### No puedes suscribirte a una lista

Este problema puede ocurrir debido a las siguientes motivos:

-   **El dueño de la lista olvidó procesar tu solicitud de suscripción**: equivocarse es de humanos, y tu solicitud puede haberse perdido entre otros muchos mensajes. Vuelve a solicitar la suscripción antes de [contactar con los dueños directamente](#contactadmin).
-   **Las suscripciones a la lista están reservadas a cierto tipo de gente**. Para saber más, [contacta con los dueños de la lista](#contactadmin).

#### No puedes autenticarte en la interfaz web de las listas de correo.

Este problema puede ocurrir debido a las siguientes motivos:

-   **No tienes contraseña**. Para obtener una contraseña, sigue el enlace [¿Primer acceso?](%7B%7Bpath_cgi%7D%7D/firstpasswd) de la página inicial. Recibirás una contraseña nueva por email.
-   **Introduciste una contraseña incorrecta**. Si has olvidado tu contraseña, puedes reestablecerla. Para hacerlo, utiliza el enlace [¿Contraseña perdida?](%7B%7Bpath_cgi%7D%7D/renewpasswd) de la página de inicio.
-   **No estás utilizando un nombre de usuario correcto** (la dirección de correo con la que te suscribiste a la lista).

| Note |
|------|
| Para evitar equivocarse al escribir la contraseña, puedes escribirlo en otra aplicación (como tu cliente de correo) y copiarlo y pegarlo dentro del navegador web. |

#### No recibes ningún mensaje enviado a una lista

Este problema puede tener muchos motivos:

-   <span id="notsubscribedyet"></span>**Nunca te has suscrito a la lista**:
    -   Tal vez cometiste un error en tu dirección de correo cuando intentaste suscribirte.
    -   Tal vez te suscribiste con otra dirección de correo diferente a la que estás consultando
    -   Puede que tu solicitud de suscripción fuese rechazada por los dueños de la lista.

    En cualquier caso, intenta [suscribirte](user.md#subscribe) de nuevo.
-   <span id="notsubscribedanymore"></span>**Ya no eres suscriptor de la lista**:
    -   Si tu dirección de correo ha generado rebotes por un tiempo, automáticamente el sistema te habrá desuscrito (o incluso puede que lo haya hecho el administrador). Intenta [suscribirte de nuevo](user.md#subscribe) después de asegurarte que tu dirección de correo no tiene problemas otra vez.
    -   Si no has respetado las diferentes reglas que se aplican a la lista, los dueños podrían haberte excluido de la lista...
    -   Puede que te haya desuscrito alguien malintencionadamente, en caso de que la lista no requiera confirmación para las solicitudes de suscripción o desuscripción... en ese caso, intenta [suscribirte de nuevo](user.md#subscribe).
-   **Tu [modo de entrega](user.md#deliverymode)no permite que recibas mensajes**: por ejemplo, encaso de tener configurado el modo de entrega 'Nomail'.
-   **La bandeja de entrada está llena**. Ten cuidado: cuando tu bandeja de entrada no está completamente llena, solo recibes pequeños mensajes, lo cual hace difícil entender cual es el problema... Además, si tu dirección de correo ocasiona problemas de forma regular, puede que seas dado de baja por el sistema o por los dueños de la lista. De esa forma, deberías limpiar tu bandeja de entrada regularmente.
-   **Tu bandeja de entrada está sujeta a algunas restricciones**: no te permiten recibir mensajes con adjuntos, prohíben algunos tipos de adjuntos o limitan el tamaño máximo del mensaje de entrada; en ese caso, te agonsejamos que utilices el [Modo Urlize](user.md#deliverymode).

#### No puedes enviar mensajes a una lista

Este problema puede tener muchos motivos:

-   **No te has [suscrito nunca](#notsubscribedyet)** a la lista.
-   **Ya [no estás suscrito a la lista](#notsubscribedanymore)**.
-   **Estás utilizando otra dirección** distinta a la dirección con la que te suscribiste a la lista.
-   **Si la lista está moderada, la distribución del mensaje dependerá de la disponiblidad del moderador**: ¡puede que no monitoricen la lista día y noche! Así que la distribución de tu mensaje puede retrasarse un poco.
-   **Si la lista es una lista moderada, tuy mensaje puede haber sido rechazado por un moderador**. En caso de haber recibido alguna notificación, puedes solicitar alguna explicación mandando un mensaje a nombredelalista-request@{{conf.host}}.
-   **El mensaje que estás intentando mandar no cumple con las condiciones para ser distribuido** en la lista: puede que sea muy grande, que contenga algún tipo de adjunto prohibido o incluso que contenga cualquier tipo de adjunto (en caso de que los adjuntos estén prohibidos en la lista).
-   **El problema puede venir dato también por tu cuenta de correo electrónico**:
    -   El servidor de correo está temporalmente inaccesible.
    -   Tu bandeja de entrada está llena y no permite que se te envíen nuevos mensajes.
    -   Tu bandeja de entrada está sujeta a algunas restriccione: no permite que envíes mensajes con adjuntos, prohibe algunos tipos de adjuntos o limita el tamaño máximo de los mensajes que envías.
-   Por último, ¡**puede que te hayas equivocado en la dirección de la lista** cuando hayas mandado el mensaje!.

#### No puedes darte de baja de una lista

Este problema puede tener muchos motivos:

-   **Estás utilizando otra dirección** distinta a la dirección con la que te suscribiste a la lista.
-   **Estás suscrito a través de una fuente de datos dinámica**(ejemplos: base de datos, directorioLDAP, etc.) que no permite que te des de baja. [Consulta con los dueños de la lista](#contactadmin) para conocer más detalles.
-   **Los dueños de la lista se olvidaron de procesar tu solicitud de desuscripción**: equivorse es de humanos, y tu solicitud puede haberse perdido entre muchos otros mensajes. Vuelve a realizar la solicitud antes de [contactar con los dueños de la lista directamente](#contactadmin).

#### <span id="contactadmin"></span>Quieres contactar con los dueños de la lista

Los nombres de los dueños y moderadores de la lista aparecen en el menú lateral izquierdo. Sin embargo, nunca debes escribir directamente a un dueño o a un moderador: primero, la persona con la que intentas contactar puede estar ausente, y de todas formas, es mejor informar a todos los dueños y moderadores de tu solicitud. Cuando tengas alguna cuestión u observación, **la dirección a la que deberías escribir es: nombre\_lista-request@{{conf.host}}** (reemplaza 'nombre\_lista' por el nombre de la lista).
