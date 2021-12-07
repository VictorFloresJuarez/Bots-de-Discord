# Ejemplos de comandos

A continuación te presento un par de ejemplos de comandos con los que podrás hacer cosas divertidas.

    if message.content.startswith('algo'):
      await message.channel.send('algo')
    
    
El comando ya visto, lo que hace es bastante evidente, siempre y cuando detecte que el comienzo del mensaje sea con el string que recibe como parámetro hará algo. Esta es la estructura básica de los comandos en discord. Es por eso que comandos de bots de música, por ejemplo, para reproducir una canción necesitan tener !play precediendo el nombre de la canción

----------------------------------------------------------------------------------------------------

Otra forma de ese comando sería esta:

    if message.content('algo'):
      await message.channel.send('algo')
    
----------------------------------------------------------------------------------------------------
    
Dicho comando ahora funciona de la siguiente manera, si TODO el contenido del mensaje es igual al string 'algo' entonces enviará un mensaje. Ahora quiero que notes que siempre usamos message.content. Porqué? No sería suficiente con imprimir solo message? Pues no, porque resulta que message es es una clase totalmente distinta a un String, es por eso que siempre que se quiera manipular el contenido del mensaje se debe usar como message.content. 


    if message.content.startswith('Copia lo que digo: '):
      await message.channel.send(message.content)
    
    
Ese comando anterior sería un uso de lo dihcho antes, es un comando que envía lo que el usuario dijo siempre y cuando comienza por 'Copia lo que digo:'
