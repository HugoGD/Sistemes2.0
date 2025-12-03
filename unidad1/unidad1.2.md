---
layout: default
title: "Infectar maquinas desde su instalación"
---

## Sprint 1. Infectar maquina Windows

[Material teórico HugoGD (PDF)](https://github.com/HugoGD/Sistemes2.0/blob/main/unidad1/DocumentacionACT2.pdf)
<br>
[Documentación Practica (PDF)](https://github.com/HugoGD/Sistemes2.0/blob/main/unidad1/ACTIVITAT1.pdf)

### Instalación NSSM
Instalamos él .zip, seguidamente lo extraemos y seguimos los pasos de instalación:

<img width="370" height="634" alt="image" src="https://github.com/user-attachments/assets/46665198-5cbb-4c7e-b908-267f5282e7e8" />

Ahora instalamos paso a paso.

Ejecutamos nssm install <Nombe del servicio>

<img width="623" height="250" alt="image" src="https://github.com/user-attachments/assets/4176f5de-d7d3-4a11-a1de-3636be0e2cd0" />

Colocamos el SCRIPT que queremos que se ejecute con el servicio

Este script buscará un puerto random el cual será el escogido para monitorear y poder acceder al ordenador remotamente, en este caso el puerto es el 3389 y en caso de que este activo se hará en el 13389, también desactiva firewall y windows defender para poder permitir la conexión externa.


<img width="625" height="561" alt="image" src="https://github.com/user-attachments/assets/cb2d3305-ef26-4565-a31d-dd073b60d702" />

Colocamos en la creación del servicio los siguientes parametros:
**path:** Con lo que se ejecutara el script
**startup directory:** El directorio donde se encontraran los scripts que se ejecutaran, tantos como queramos.
**Arguments:** Le colocamos la linea que ejecutara el script

<img width="536" height="265" alt="image" src="https://github.com/user-attachments/assets/390503f8-62c9-4aa5-959c-008f8d640a6d" />

Le damos a instalar y saldra una nueva pestaña en la que pone que se a instalado correctamente.

Ahora abrimos el menu de “Ejecutar” con “windows + R” y colocamos **services.msc**

<img width="625" height="220" alt="image" src="https://github.com/user-attachments/assets/14b3dfae-079d-4459-abe5-ba72983a4c26" />

Entregamos permisos de ejecución al script

<img width="626" height="46" alt="image" src="https://github.com/user-attachments/assets/1a16c2e1-a067-40d5-8908-c1fac3577c00" />

Ahora reiniciamos la maquina y comprobamos que se pueda ejecutar desde que se arranca

<img width="615" height="584" alt="image" src="https://github.com/user-attachments/assets/59f76767-6fd8-4661-b923-26d9d71ea129" />

Ahora colocamos este comando “rdesktop -u Admin -p Admin 192.168.56.105:3389” para iniciar la conexión.

<img width="621" height="349" alt="image" src="https://github.com/user-attachments/assets/6b0db62f-3082-4760-b46c-47fd979a3f90" />

