## Práctica 3: Seguridad y calidad
I. **Arquitectura hexagonal**  
1. ***Crear una rama llamada hexagonal*** 
![rama](https://user-images.githubusercontent.com/74604371/204703624-8f3806d8-5643-45aa-8dd0-219621734b60.JPG) <p align="center">_Crear rama llamada hexagonal_</p>  
2. ***Organizar codigo con arquitectura Hexagonal***  
![organizacion](https://user-images.githubusercontent.com/74604371/204704368-3ba22233-3bda-479c-b852-353f05a19ec2.JPG)<p align="center">_Organización de la carpeta SRC_</p>  
3. ***Crear carpeta models dentro de domain y cree un archivo de modelo.***  
![carpeta models](https://user-images.githubusercontent.com/74604371/204712932-2a0d8b6d-14e0-4ad7-bddb-7d51e4c8ef08.JPG)<p align="center">_Creacion de carpeta models, domain y archivos moto.model.ts - moto.ts_</p>  
4. ***Es momento de migrar la funcionalidad implementada en el controlador a un servicio***  
![motoServices](https://user-images.githubusercontent.com/74604371/204713295-f9d32e2a-d71f-481d-a55b-5c1f773c3494.JPG)<p align="center">_Funcionalidad del controlador migrada a un servicio, carpeta services/motos.service.ts_</p>  
5. ***Modificar el controlador motos.controller.ts para que se emplee el la implementación del servicio.***  
![controladores](https://user-images.githubusercontent.com/74604371/204713740-5e6368a7-3a63-40e4-9d84-fa7bcfc3e1a3.JPG)<p align="center">_Modificación del controlador para implementarción del servicio_</p>  
II. **Implementado seguridad**  
1. ***Instalar el paquete @nestjs/passport y passport***  
![npm install](https://user-images.githubusercontent.com/74604371/204715092-b915a940-a03c-48ef-8432-67297d8d64c2.JPG)<p align="center">_Instalación de los paquetes @nestjs/passport y passport_</p>  
2. ***Crear modulo de Autenticación***  
![uno](https://user-images.githubusercontent.com/74604371/204715476-95404010-d26c-4e5d-9c14-e0883c902325.JPG)<p align="center">_Ejecución de los comandos para crear modulos de autenticación_</p>  
3. ***Crear modulos para gestión de Usuarios***  
![image](https://user-images.githubusercontent.com/74604371/204715867-d988599c-e59a-4a90-ad4b-e7c0ade151bc.png)<p align="center">_Ejecución de los comandos para crear modulos de gestión de Usuarios_</p> 
4. ***Implementación del servidor con seguridad***
![image](https://user-images.githubusercontent.com/74604371/205186663-53df434e-24cd-48cd-909f-e4ea1e47a6ba.png)<p align="center">_Arquitectura del servidor y implementación de la seguridad_</p> 
***Link del repositorio: https://github.com/mezcly08/Practica_02/tree/Practica3_seguridad***  
III. ***Autenticación con JWT***
1. ***Organizar la estructura del servidor JWT y generar Token***  
![image](https://user-images.githubusercontent.com/74604371/205198667-5afa8c2d-ff91-4031-83a8-ebce3f080471.png)<p align="center">_Arquitectura del servidor en JWT y generar el token de access_</p>  
2.***Crear un nuevo registro en el servidor con JWT***  

3. ***Proteger los verbos HTTP***  
![image](https://user-images.githubusercontent.com/74604371/205200540-37a40755-5af6-432e-a3cf-021125ab5e6c.png)<p align="center">_Proteger los verbos HTTP_</p>  



