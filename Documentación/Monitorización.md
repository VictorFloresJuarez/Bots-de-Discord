# Monitorización

Ahora, si bien nuestro bot ya está activo 24/7, no es del todo evidente cuando este se enciende, así que se harán dos pasos ahora

# Paso 1:

Copia y pega el siguiente código antes del evento de on_message:

@client.event
async def on_ready():
  print('Se ha iniciado el {0.user}'.format(client))

Tu código ahora debe tener esta apariencia:

![paso8.1](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso8.1.png?raw=true)

# Paso 2:

Al ejecutar tu código copia el link que sale en esta pestaña:

![paso8.2](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso8.2.png?raw=true)

Con dicho link ve a UptimeRobot y agrega un nuevo monitor. Llena los espacios como la siguiente captura: utilizando tu link y el nombre de tu bot

![paso8.3](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso8.3.png?raw=true)

Crea el monitor, detén la ejecución de bot y vuelve a correr el bot. Tras esto refresca la página de UptimeRobot un par de veces

![paso8.4](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso8.4.png?raw=true)
