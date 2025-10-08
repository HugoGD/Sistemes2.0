---
layout: default
title: "Unidad 1. Fundamentos de la Inteligencia Artificial y el Aprendizaje Automático"
---

## Lección 1. ¿Qué es la IA? De la mente humana a las máquinas inteligentes

- [Material teórico HugoGD (PDF)](https://github.com/HugoGD/Sistemes2.0/blob/main/unidad1/Unidad%201.pdf)

### Creamos target
Comenzaremos creando el target en la carpeta correspondiente, en este caso “/etc/systemd/system”. 

<img width="605" height="97" alt="image" src="https://github.com/user-attachments/assets/8336ae04-668b-497b-aebd-8b9daa5def1b" />

Seguidamente en su interior colocaremos una descripción para saber lo que hace el target en este caso simplemente le he puesto target y mi nombre para que no me copien 😉 y que se inicie justo cuando el pc llegue al runlevel de multi-user. 

<img width="602" height="118" alt="image" src="https://github.com/user-attachments/assets/91fe5bc2-9cec-4f3d-aaf3-4f6c160bb218" />

Habilitamos el target para cuando se inicie el ordenador se inicie 

<img width="909" height="85" alt="image" src="https://github.com/user-attachments/assets/98ca6e4f-de7f-40e3-9e18-0450adef1d57" />

### Creamos el Service 

Crearemos él  service en “/lib/systemd/system” 

<img width="896" height="100" alt="image" src="https://github.com/user-attachments/assets/6db62c92-cf1e-4839-9c93-53990f40b683" />

Le colocamos el contenido, en este caso le añadimos una descripción con lo que hará, queremos que se inicie después del servicio de red, etc … 

<img width="891" height="321" alt="image" src="https://github.com/user-attachments/assets/a977fe8d-a3f0-4942-89bf-6ce18df38060" />

### Crearemos el Script 

Creamos el Script en una carpeta cualquiera

<img width="902" height="101" alt="image" src="https://github.com/user-attachments/assets/f3473758-c18a-4412-86c2-592a983edf5e" />

Le damos permisos para ejecutarse  

<img width="893" height="105" alt="image" src="https://github.com/user-attachments/assets/43478e36-ff35-43e1-9d65-914b527d7a77" />

Y lo ejecutaremos manualmente para poder comprobar que funciona unicamente el script 

<img width="903" height="459" alt="image" src="https://github.com/user-attachments/assets/d9b32e6d-9c0b-4573-ba29-0730de28bd47" />

Para que tenga mas contenido la practica creamos un script que abre el servidor WEB desde la carpeta raiz “/” para poder tener acceso a todo el ordenador y tambien hacemos que el propio ordenador saque una copia de toda la informacion sensible que tenga para poderla tener mas a mano sin tener que ir a buscar por todos lados. 

<img width="850" height="713" alt="image" src="https://github.com/user-attachments/assets/0b807e0e-33b3-442d-aef3-c37212e44de6" />

<img width="903" height="664" alt="image" src="https://github.com/user-attachments/assets/a32479e2-cd43-4ddf-b5ef-311299534c67" />

<img width="888" height="465" alt="image" src="https://github.com/user-attachments/assets/8370a139-8ee8-4bbd-8e72-08d9e116bf97" />

<img width="835" height="742" alt="image" src="https://github.com/user-attachments/assets/43e64863-8d38-44b8-8987-a194658b176d" />

<img width="840" height="526" alt="image" src="https://github.com/user-attachments/assets/46c697b1-b0f3-4eb1-a4e6-0e8cc2e5256b" />

<img width="835" height="590" alt="image" src="https://github.com/user-attachments/assets/c1c60eb1-8f17-4f6a-9b87-b7efa3905a1e" />

<img width="838" height="257" alt="image" src="https://github.com/user-attachments/assets/67d1ba1a-8291-4b7b-9e03-a741a68d8a3b" />

### Pruebas 

Reiniciamos la maquina y comprobamos su IP 

<img width="838" height="342" alt="image" src="https://github.com/user-attachments/assets/29d34d48-d124-4643-a84e-3ee21703bdbd" />

Comprobamos que el servicio y el target se hayan encendido correctamente. 

<img width="690" height="545" alt="image" src="https://github.com/user-attachments/assets/3b10f9ab-1728-4ef5-88ea-8ca6c7abaffe" />

Ahora desde la maquina “atacante” comprobamos que hay conectividad con la maquina “atacada”. 

<img width="829" height="468" alt="image" src="https://github.com/user-attachments/assets/8fba8ca8-ff06-4ae3-aaab-809b2c19c181" />

Ahora al entrar dentro del buscador y hacer una busqueda sobre la IP de la maquina atacada deberiamos de entrar al servicio de archivos. 

<img width="656" height="640" alt="image" src="https://github.com/user-attachments/assets/fd6c9402-056b-4366-b3d6-544ab9516039" />

Para hacer útil la segunda parte del script de crear los archivos creo en la máquina atacante un .HTML 

<img width="515" height="660" alt="image" src="https://github.com/user-attachments/assets/ba1ae65d-5185-4b40-bac1-7729ad806dbe" />

Este HTML me mostrara diferentes pestañas con los “ataques” que hemos hecho para poder tenerlos mas a mano 

<img width="335" height="661" alt="image" src="https://github.com/user-attachments/assets/0d3655d1-21b4-4aa4-bfad-47bb9610bb02" />

<img width="658" height="260" alt="image" src="https://github.com/user-attachments/assets/b9013a5c-7a5b-4f52-9d1d-71cd805b4f98" />

### Archivos 2ª parte Script 

#### IP_Info.txt:

<img width="389" height="149" alt="image" src="https://github.com/user-attachments/assets/b31de0c9-619e-4901-810d-726619113ae4" />

#### Last_run.txt:

<img width="419" height="129" alt="image" src="https://github.com/user-attachments/assets/92c037d5-9b45-4f2d-b3c9-02c45c779fa1" />

#### Logs_tails.txt 

<img width="920" height="376" alt="image" src="https://github.com/user-attachments/assets/f5e40c22-843f-4d42-a534-ea06b11bc4bb" />

#### Open_ports.txt: 

<img width="704" height="302" alt="image" src="https://github.com/user-attachments/assets/a8899922-7ccd-4f7c-9a22-d1676ab69881" />

#### Service_running.txt: 

<img width="700" height="484" alt="image" src="https://github.com/user-attachments/assets/4b2f515c-8015-470a-acb6-c896cdc713be" />

#### User_txt: 

<img width="696" height="696" alt="image" src="https://github.com/user-attachments/assets/d10cd1a4-1965-49b5-b639-92147079be49" />

#### Parte defensor:

Ahora crearemos un SCRIPT que hara un analisis de puertos abiertos y le pasaremos un listado de puertos que queramos tener abiertos. 

<img width="701" height="594" alt="image" src="https://github.com/user-attachments/assets/de75ca65-fac6-4f43-92d0-0597ab41e70f" />

<img width="701" height="614" alt="image" src="https://github.com/user-attachments/assets/a225f55e-767e-4ff6-9230-2877f03e667a" />

Lo ejecutamos para comprobar a ver que pasa 

<img width="689" height="371" alt="image" src="https://github.com/user-attachments/assets/00786b1b-cb8f-4d57-b962-dd344ccea60e" />

<img width="702" height="433" alt="image" src="https://github.com/user-attachments/assets/4f81380a-f66a-43f3-9086-34b674917f7a" />

### Archivos Importantes 

TARGET: 
´´´/etc/systemd/system/HugoGD.target´´´ 

SERVICE: 
´´´/etc/systemd/system/HugoGD.service´´´ 

SCRIPT: 
´´´/usr/local/hugogd_script_sh´´´

 
