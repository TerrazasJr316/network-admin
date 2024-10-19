# Conexión remota entre windows y linux

Asignar una direccipon IP para realizar la conexión de punto a punto
(verificar que sea correcto el ping entre amabos equipos) usar el siguiente comando en Ubuntu:

```console
ping <dominio_o_direccion_IP>
```

Intalar servicio de telnet en Ubuntu:

```console
sudo apt-update
sudo apt install telnet
```

cechar el puerto correcto del servicio:

```console
$ nmap localhost
# 23  telnet/tcp
```

Ahora en sistema Windows ingresar el siguiente comando (esta toma el papel del cliente):

```console
telnet <dominio_o_dirección_IP_servidor> 23
```

Por ultmimo requerirá las credenciales para acceder a su arvchivero del servidor:

```console
user: <nombre_servidor>
password:
ls
# permite obtener una lista de todo los recurso del servidor
```
