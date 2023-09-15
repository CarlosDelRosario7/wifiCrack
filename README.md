# wifiCrack

Archivo.sh que facilita el uso de aircrack-ng para la auditoría de red WiFi. El programa instala las dependencias si no están.

## Dependencias

- aircrack-ng
- macchanger

## Agregue a variable de entorno

Si deseas utilizar esta herramienta desde cualquier directorio, agréguela a la variable de entorno o corra los siguientes comandos:

Baje el repositorio en caso de que aún no lo ha hecho.

```shell
git clone https://github.com/CarlosDelRosario7/wifiCrack
```

Entre al directorio y copie el archivo a /usr/bin.

```shell
cd wifiCrack
sudo cp wifiCrack /usr/bin
```

Hecho esto, el programa estará listo para utilizarse desde cualquier directorio.

## Uso

```shell
wifiCrack -t wlanX -w wordlist/path
```

Donde:
- "wlanX" es el nombre de la tarjeta de red wifi que tienes. Generalmente suele ser "wlan0". Para saber el nombre de su tarjeta de red ejecute el siguiente comando...

```shell
ifconfig
```

- "wordlist/path" es la dirección en donde está el diccionario que contiene las contraseñas. Con el siguiente comando...

```shell
wordlists
```

Se dirigirá a donde están las wordlist del sistema. En caso de tener una descargada en su computador, puedes indicar su dirección en el programa sin problemas.

### Nota 1
En caso de que logró descifrar la clave, pero la red es oculta y no conoces su nombre, ejecute el siguiente comando:

```shell
cat Captura-01.csv
```

El nombre suele estar debajo de "ESSID".

### Nota 2
En la actulidad, solo funciona bien en **Kali Linux**. Trataré de que también funcione en las demás ditros.
