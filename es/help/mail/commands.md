Lista de los comandos de la interfaz de correo Sympa
----------------------------------------------------

Todos los comandos deben enviarse a {{conf.email}}@{{conf.host}}.

Es posible enviar varios comandos en un único mensaje. Los comandos se deben introducir en el cuerpo del mensaje (un comando por línea).

### Comandos para usuarios

`HELP` recibe un listado de todos los comandos disponibles.

`LISTS`: recibe una lista de todsa las listas gestinadas en el servidor.

`WHICH`: recibe un listado de todas las listas a la cual el usuario está suscrito.

`CONFIRM clave`: confirmar el envío de un mensaje (según la forma en que esté configurada la lista)

`QUIT`: indica el final de los comandos (usados para ignorar una firma)

`INFO lista`: obtiene la información sobre la lista

`REVIEW list`: recibe una lista de todos los miembros de la lista

`SUBSCRIBE lista nombre`: suscripción (o confirmación de suscripción) a la lista de la cuenta que envía el correo (nombre es el nombre del usuario con el que quiere aparecer en la lista, y es opcional)

`INVITE lista email`: invitar a alguien a suscribirse a la lista

`UNSUBSCRIBE lista email`: darse de baja de la lista. La dirección de correo electrónico es necesaria solo si te quieres dar de baja con una dirección distinta a la dirección con la que envías el mensaje

`UNSUBSCRIBE * email`: darte de baja de todas las listas a las que estás suscrito.

`SET lista NOMAIL`: suspende la recepción de mensajes de la lista

`SET lista DIGEST`: recibir mensajes en modo recopilación (digest)

`SET lista DIGESTPLAIN`: recibir mensajes en modo recopilación en texto sin formato

`SET lista SUMMARY`: solo recibe un listado de mensajes (los asuntos)

`SET lista NOTICE`: solo recibe los asuntos de los mensajes

`SET lista MAIL`: modo normal de recepción de mensajes

`SET lista CONCEAL`: Ya no estar más en el listado (Ocultar la dirección de suscripción)

`SET lista NOCONCEAL`: la dirección del suscriptor será visible con el comando REView

`INDEX lista`: recibe un listado de ficheros del archivo

`GET lista fichero`: recibe un fichero del archivo de la lista

`LAST lista`: recibe los mensajes más recientes de la lista

### Comandos para los dueños de lista

`ADD lista email nombre`: añade un miembro a la lista

`DEL lista email`: borra a un suscriptor de la lista

`STATS lista`: comprueba las estadísticas de la lista

&lt;`REMIND lista`: envía a todos los suscriptores un recordatorio personalizado con las direcciones con las que están suscritos a la lista

### Comandos para moderadores de listas

`DISTRIBUTE lista codigo`: aprueba un mensaje

`REJECT lista codigo`: rechaza un mensaje moderado

`MODINDEX lista`: comprueba la lista de mensajes a moderar
