# Activar bot

Si eres observador, podrás notar que a pesar de que tu bot ya se unió a tu servidor este aparece como desconectado. Esto es porque el bot no está encendido, vamos a arreglar eso y despertar a ese dormilón.

Primero realiza todo este código en tu archivo main en tu proyecto:
![paso5.1](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.1.png?raw=true)

Ahora, regresa a Discord Developer Portal y vete a la pestaña que dice bot, copia el Token.
![paso5.2](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.2.png?raw=true)

Ahora, en replit, vete a la parte de secret. Haz click y en key introduce 'TOKEN' y en value pega lo que acabas de copiar.
![paso5.3](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.3.png?raw=true)

Tras esto inserta el segundo código que te aparece, el que está abajo del import os. Tu código ahora debe verse de esta forma:
![paso5.4](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.4.png?raw=true)

Ahora introduce estas sentencias extra en tu archivo main:
client = discord.Client()
client.run(my_secret)

Tu código ahora debe tener esta apariencia:

![paso5.5](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.5.png?raw=true)

Ahora al ejecutar el archivo podrás notar como tu bot pasa de estar desconectado a estar conectado.

Después de ejecutar:
![paso5.7](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso5.7.png?raw=true)

# Notas

El token funciona como una especie de ID para tu bot, cada bot tiene su TOKEN único.

El token funciona para que sepamos qué bot se está manipulando.

No debes compartir este token con nadie, con este cualquier persona desde cualquier lugar puede modificar el comportamiento de tu bot.

La sentencia client = discord.Client() es básicamente crear al bot en el código.

La sentencia client.run(my_secret) hará que el bot con el TOKEN = my_secret sea encendido.
