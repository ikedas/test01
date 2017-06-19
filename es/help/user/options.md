Esta es una descripción de los modos de recepción disponibles en Sympa. Estas opciones se excluyen mutuamente, lo que significa que no puedes configurar dos modos de recepción simultaneamente. Solo algunos de los modos podrían estar disponibles para listas de correo específicas.

-   Recopilación (Digest)
    En vez de recibir mensajes de correo individuales de la lista, el suscriptor recibirá periódicamente un lote de mensajes en una Recopilación. Esta recopilación aglutina un grupo de mensajes de la lista, utilizando el formato MIME multiparte.
    La periodicidad de envío de estas Recopilaciones la define el dueño de la lista.
-   RecopilaciónPlano (DigestPlain)
    Similar a la opción Recopilación en la que el usuario recibirá periódicamente los mensajes por lotes en una Recopilación. Con RecopilaciónPlano la recopilación se manda en texto sin formato, con todos los documentos adjuntos extraídos. RecopilaciónPlano es útil si tu programa de correo electrónico no muestra correctamente los mensajes con formato multipartes.
    La periodicidad de envío de estas Recopilaciones la define el dueño de la lista.
-   Sumario
    En vez de recibir mensajes de correo individuales de la lista, el subscriptor recibirá periódicamente una lista de mensajes. Este modo es mas parecido al modo de recepción Recopilación pero el suscriptor recibe solo la lista de los mensajes.
-   ~~Nomail~~
    Este modo se usa cuando un subscriptor no quiere seguir recibiendo correo de la lista, pero sin embargo desea mantener la posibilidad de enviar mensajes a la lista. Este modo por lo tanto evita al subscriptor tener que cancelar la subscripción y darse de alta nuevamente más tarde.
-   Txt
    Este modo se usa cuando un subscriptor solo desea recibir en texto sin formato, los correos enviados en el formato HTML y texto sin formato.
-   Html
    Este modo se usa cuando un subscriptor solo desea recibir en formato HTML, los correos enviados en el formato HTML y texto sin formato.
-   Urlize
    Este modo se usa cuando un subscriptor no quiere recibir ficheros adjuntos. Los ficheros adjuntos son reemplazados por una URL que apunta al fichero compartido en la web de la lista.
-   Not\_me
    Este modo se usa cuando un subscriptor no quiere recibir copias de los mensajes que él/ella ha enviado a la lista.
-   Normal
    Esta opción se usa principalmente para cancelar los modos nomail, resumen (summary) o recopilación (digest). Si el subscriptor estaba en modo nomail, él volverá a recibir mensajes de correo individuales de la lista.

