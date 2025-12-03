---
layout: default
title: "Modificación y compilación de Kernels"
---

## Lección 1. Kernel Linux

<details>
  <summary><strong>MATERIAL</strong></summary>

  <br>

- [Documentación (PDF)](https://github.com/HugoGD/Sistemes2.0/blob/main/unidad1/DOCUMENTACION%20ACT%201.pdf)
- [Documentación Practica Kernel (PDF)](https://github.com/HugoGD/Sistemes2.0/blob/main/unidad1/ACTIVITAT1.pdf)

</details>

## KERNEL

Nos situamos en la carpeta de descargas

<img width="686" height="101" alt="image" src="https://github.com/user-attachments/assets/3491d1c1-c638-4529-bbd7-438e34e92cd3" />

Nos descargamos el Kernel que vamos a usar en mi caso el 6.8.1

<img width="546" height="90" alt="image" src="https://github.com/user-attachments/assets/ae4d60d7-6a09-4585-81c4-c095bfb29ed0" />

Descomprimimos el archivo del kernel

<img width="683" height="77" alt="image" src="https://github.com/user-attachments/assets/4a3f43e8-bd99-43e2-8cc5-d3a89329df0a" />

Entramos dentro de la carpeta del kernel

<img width="685" height="49" alt="image" src="https://github.com/user-attachments/assets/6df77d99-a1c9-4755-8f6d-e8de1b050263" />

Hacemos la copia de main.c

<img width="681" height="98" alt="image" src="https://github.com/user-attachments/assets/25feb8b6-b2cf-4185-b1d4-952c9d5f1e4e" />

Modificamos el kernel para saber lo que queremos que nos salga

<img width="684" height="524" alt="image" src="https://github.com/user-attachments/assets/88dd0b7f-8706-4c64-ac33-0bd59ceccaa7" />

Creamos el parche

<img width="688" height="119" alt="image" src="https://github.com/user-attachments/assets/ccbfaddf-dd47-4d1e-a79c-b802fc9118ce" />

Aplicamos el parche y comprobamos que se a aplicado

<img width="685" height="140" alt="image" src="https://github.com/user-attachments/assets/1c102b03-9466-4cc3-aeac-be25149a198a" />

Comentamos los TIMEOUT de /etc/default/grub

<img width="677" height="553" alt="image" src="https://github.com/user-attachments/assets/6cf88508-d64c-49e9-aa73-046673f35d03" />

Hacemos el update-grub para que se apliquen las modificaciones

<img width="660" height="208" alt="image" src="https://github.com/user-attachments/assets/a74d4dca-840e-4a0b-97de-33f8d797f980" />

Hacemos el menuconfig y quitamos la virtualización en el archivo de configuración

<img width="684" height="596" alt="image" src="https://github.com/user-attachments/assets/5f35a8b6-d844-4763-b175-c25de8360bff" />

<img width="686" height="644" alt="image" src="https://github.com/user-attachments/assets/0da7626e-9038-433e-baf7-4a422d7b6d67" />

Guardamos en .config

<img width="648" height="373" alt="image" src="https://github.com/user-attachments/assets/e5bb8c6e-49c4-4407-a48d-4c0a41140516" />

<img width="607" height="135" alt="image" src="https://github.com/user-attachments/assets/cfc1383e-4d4c-4e3f-b353-e299c8b67300" />

Comprobamos que existe

<img width="683" height="250" alt="image" src="https://github.com/user-attachments/assets/92d48328-4adc-4294-9f75-da2c5e857841" />

Limpiamos compilaciones anteriores

<img width="668" height="79" alt="image" src="https://github.com/user-attachments/assets/1e635ca3-3e54-4e37-8411-52224cf31fb6" />

Preparamos las dependecias

<img width="685" height="515" alt="image" src="https://github.com/user-attachments/assets/b14a9289-23de-469a-8f19-f432443dc9e1" />

Iniciamos la compilacion

<img width="691" height="563" alt="image" src="https://github.com/user-attachments/assets/ceda7e12-b77a-4809-bbdf-b85a439dc108" />



