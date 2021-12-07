# Mantener activo

Ahora tenemos un problema. Si ya lo notaste cada que detienes la ejecución o cierras el proyecto en replit el bot detiene la ejecución. Esto es un problema porque necesitas tener la página abierta todo el timepo. Una solución a esto se consigue haciendo estos pasos:

# Paso 1:

Crea un nuevo archivo en tu proyecto, el nombre puede ser el que gustes, la extensión de este debe ser .py, para que te des una idea en dicho archivo estará el código que mantiene el bot encendido. Para que le pongas un nombre representativo.

![paso7.1](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso7.1.png?raw=true)

# Paso 2:

En dicho archivo copia y pega este código:

from flask import Flask
from threading import Thread

app = Flask('')

@app.route('/')
def home():
  return "Hello, I am alive!"

def run():
  app.run(host='0.0.0.0', port=8080)

def keep_alive():
  t = Thread(target=run)
  t.start()
  
![paso7.2](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso%207.2.png?raw=true)
  
# Paso 3:

En el archivo main realiza el siguiente import: from mantenerEncendido import keep_alive

# Paso 4: 

Agrega esta sentencia antes del client.run: keep_alive()

# Vista final

Si seguiste todos los pasos correctamente tu código debe tener esta apariencia:

![paso7.3](https://github.com/VictorFloresJuarez/Bots-de-Discord/blob/main/Recursos/paso7.3.png?raw=true)

