## Evidencias Practica 1
### Elavorado por: Carlos Hoyos
1. ***Configuración del entorno:*** El estudiante deberá configurar su dispositivo de elección para ejecutar una imagen virtualizada de Linux, este será un suministro importante para el resto de prácticas.  
La imagen virtualizada escogida es: **Arch Linux**,  también se realizó la instalación de las Guest Additions.  
![ARCH](https://user-images.githubusercontent.com/74604371/204191957-eb907b62-6b02-4d17-b628-3b4b44cc91a5.png)<p align="center">_Instalación correctamente de Arch Linux_</p>
2. ***Instalar docker***  
Para instalar docker utilizamos la herramienta **paru**, despues utilizamos los comandos para instalar docker.  
![comandos docker](https://user-images.githubusercontent.com/74604371/204170151-62b9917a-d7b2-4323-973f-0e25856722d7.jpg) <p align="center">_Comandos utilizados para instalar docker utilizando Paru_</p>  
Ahora tenemos que crear un grupo para utilizar los servicios de docker, de tal manera que mi usuario tenga los privilegios de un administrador.  
![comandos para privilegios](https://user-images.githubusercontent.com/74604371/204170467-e8898b00-ed34-4bfb-8146-90471e85766d.jpg) <p align="center">_Comandos para dar privilegios_  </p>  
Se instaló correctamente docker y se le dió privilegios al usuario, comprobemos la instalación de Docker llamando a "docker pull hello-world".  
![ejecucion docker](https://user-images.githubusercontent.com/74604371/204170685-66d31b23-6528-41e4-abb7-6dbaa41cd27e.png)<p align="center">_ejecución de docker_ </p>  
3. **Reconocimiento de herramientas de red:** Identificar configuración de red por medio del comando ip e ifconfig. Identificar servicios y puertos ocupados en el sistema con los comandos ss, netstat y lsof.  
- **comandos**  
  - **Ip e Ifconfig**  
![ifconfig](https://user-images.githubusercontent.com/74604371/204173544-c9d38398-6c77-4fcc-ad9f-22e3abfefca2.jpg)<p align="center">_en rojo se encuentra la ip de la tarjeta wifi del pc_ </p>  
  - **ss:** La salida devuelve una lista de sockets abiertos que no escuchan con conexiones establecidas.  
![comando ss](https://user-images.githubusercontent.com/74604371/204174122-1d83af55-21fb-45f9-ad39-cfecef3be952.png)<p align="center">_comando ss color azul dirección de la máquina local y el puerto. Y color amarillo dirección de la máquina y el puerto remotos._ </p>  
  - **netstat:** es una herramienta de línea de comandos que muestra las conexiones de red(entrantes y salientes), tablas de enrutamiento y una serie de estadísticas de interfaz de red.  
  ![comando netstat](https://user-images.githubusercontent.com/74604371/204175563-a02b9257-1041-4abe-8bca-efb629f7346d.JPG)<p align="center">_comando netstat para ver las conexciones de red._ </p>  
  - **lsof:** recuperar detalles sobre varios tipos de archivos abiertos por diferentes procesos en ejecución.  
  ![comando lsof](https://user-images.githubusercontent.com/74604371/204176994-982cffd4-b6e3-4358-a794-4317d9ba2869.JPG)<p align="center">_comando lsof detalles sobre tipos de archivos abiertos._ </p>  
4. **Identificar servicios desplegados:** El estudiante deberá identificar 5 servicios diferentes listados por las herramientas de red y determinar a qué aplicaciones posiblemente están relacionados. 
![servidor UDP y TCP](https://user-images.githubusercontent.com/74604371/204192499-67093e4e-2715-4427-b033-cae7ee3a1555.JPG)<p align="center">_Servicios desplegados en este caso es de tipo TCP y UDP_ </p>  
5. **Evaluar scripts en Python:** Al estudiante se le entregarán scripts en Python para desplegar un ejemplo de cliente servidor con protocolos TCP y UDP, el estudiante evaluará el rendimiento de los dos servicios y debe descubrir la ocupación de los puertos por medio de las herramientas previamente estudiadas. 
  -**Cliente y Servidor TCP:**  
  ![Cliente y Servidor TCP](https://user-images.githubusercontent.com/74604371/204185381-7ec9b512-be35-4df6-9759-189d734181db.JPG) <p align="center">_ejecucion del cliente y servidor TCP_ </p>  
  -**Cliente y Servidor UDP:**   
  ![cliente y servidor UDP](https://user-images.githubusercontent.com/74604371/204184342-0a629a6a-7857-4749-8509-aa2d7068552a.JPG) <p align="center">_ejecucion del cliente y servidor UDP_ </p>  
En este caso los protocolos **TCP** y **UDP** estan utilizando el mismo puerto, pero como en el protocolo **UDP** no requiere una conexión de larga duración solo utiliza el puerto cuando por una corta duración, en el protocolo **TCP** ambos extremos de un conector TCP/IP estén conectados, lo que deja escuchando siempre al servidor
