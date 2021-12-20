# wifiCrack

Archivo.sh que facilita el uso de aircrack-ng para la auditoría de red WiFi. El programa instala las dependencia si no están.

## Dependencia

- aircrack-ng
- macchanger

## Agregue a variable de entorno

Si deseas utilizar esta herramienta desde cualquier directorio, agréguela a la variable de entorno o corra los siguientes comandos lo siguiente:

Baje el repositorio en caso de que aún no lo ha hecho.

> git clone https://github.com/CarlosDelRosario7/wifiCrack

Entre al directorio y copie el archivo a /usr/bin.

> cd wifiCrack
> chmod +x wifiCrack
> cp wifiCrack /usr/bin

Hecho esto, el programa estará listo para utilizarse desde cualquier directorio.

## Uso

> wifiCrack -t wlan0 -w wordlist/path

Donde:
- "wlan0" es el nombre de la tarjeta de red wifi que tienes. Generalmente suele ser "wlan0". Para saber el nombre de su tarjeta de red ejecute el siguiente comando...

> ifconfig

- "wordlist/path" es la dirección en donde está el diccionario que contiene las contraseñas. Con el siguiente comando...

> wordlists

Se dirigirá a donde están las wordlist del sistema. En caso de tener una descargada en su computador, puedes indicar su dirección en el programa sin problemas.
