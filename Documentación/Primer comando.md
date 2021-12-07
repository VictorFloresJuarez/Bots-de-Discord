# Ahora vamos a crear nuestro primer comando

Dicho comando tendrá la siguiente forma:

![paso6.1](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso6.1.png?raw=true)


# Explicación

El 'client.event' es, en términos sencillos, el evento. A dichos eventos siempre les siguen las funciones predefinidas de ciertos tipos, en este caso la función on_message(message) es una función para cuando se envía cualquier mensaje en el canal de texto donde está el bot.

Ahora, el primer if se encarga de que el bot no responda a los mensajes que el mismo manda por el canal de texto.

El segundo básicamente está diciendo que si el mensaje introducido comienza por 'Ping' el bot debe enviar como mensaje 'Pong'
