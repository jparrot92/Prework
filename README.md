# Prework: Buenas Prácticas y Entorno de Desarrollo<!-- omit in toc -->

## Tabla de Contenido<!-- omit in toc -->
- [Introducción a la línea de comandos](#introducción-a-la-línea-de-comandos)
  - [Instalación de Ubuntu Bash en Windows](#instalación-de-ubuntu-bash-en-windows)
  - [Manejo archivos y directorios](#manejo-archivos-y-directorios)
  - [Herramientas básicas (Comandos CAT, MORE, TAIL y OPEN)](#herramientas-básicas-comandos-cat-more-tail-y-open)
  
## Introducción a la línea de comandos

### Instalación de Ubuntu Bash en Windows
Lo primero que necesitas es que tu computadora tenga instalado Windows 10 de 64 bits y tengas tu sistema operativo actualizado (sobre todo con el “Windows 10 Anniversary Update”

Una vez hayas verificado que tu computadora cumple con los requisitos entra a los settings del sistema (Ajustes)
![primeraImagen](https://user-images.githubusercontent.com/18260051/69757002-1da16000-115c-11ea-84f1-1bca17bb6174.png)

Luego entra a la opción de Actualizaciones y Seguridad
![segundaImagen](https://user-images.githubusercontent.com/18260051/69757003-1da16000-115c-11ea-9ca4-fe348458ea62.png)

En el menú de la izquierda has click en opciones para desarrolladores y habilita el “Modo Desarrollador”
![terceraImagen](https://user-images.githubusercontent.com/18260051/69757005-1da16000-115c-11ea-80db-ee36cb5f80c6.png)
![CuartaImagen](https://user-images.githubusercontent.com/18260051/69757001-1da16000-115c-11ea-9521-700207c4de6f.png)


Después, accede al panel de control y haz click en “Programas”

![5taimagen](https://user-images.githubusercontent.com/18260051/69757000-1d08c980-115c-11ea-8b47-1ad337945f6a.png)

Una vez ahí, haz click en activar o desactivar características de windows
![sextaImagen](https://user-images.githubusercontent.com/18260051/69757004-1da16000-115c-11ea-9034-4f600ac820a3.png)
Aquí, busca la opción de “Windows Subsystem for Linux” y actívala, instala eso y permite que tu computadora se reinicie.

Luego, entra al menú inicio, escribe bash y sigue los pasos que te indique, en caso de que te diga que no tienes ninguna distribución sólo ve a la tienda de aplicaciones y descargaba Ubuntu para Windows.
![ultimaImage](https://user-images.githubusercontent.com/18260051/69757006-1e39f680-115c-11ea-8653-d4f96e7367dc.png)

Luego, ejecuta Ubuntu, crea tu usuario y contraseña y estás lista o listo para continuar.

![resultImage](https://user-images.githubusercontent.com/18260051/69758429-c8ffe400-115f-11ea-9551-f687750b125d.png)

### Manejo archivos y directorios
* **ls**: Nos permite listar los archivos y directorios que se encuentren dentro de la carpeta en la que estamos ubicados, podemos pasarle distintos parámetros a este comando:
  * **-a** podemos ver los archivos ocultos.
  * **-l** nos lista los contenidos mostrando sus permisos y propietarios.
  * **-t** nos lista los contenidos según su fecha.
* **clear**: Nos limpia la pantalla.
* **pwd**: Nos retorna la ruta absoluta en la cual nos encontramos.
* **mkdi**r: Crea una carpeta.
* **cd**: Nos mueve a alguna carpeta que le indiquemos, dentro de los archivos ocultos vimos que existe:
  * **.**: Refiere a la carpeta en la cual estamos ubicados.
  * **..**: Se refiere a la carpeta padre en la cual nos encontramos.
* **history**: Muestra el histórico de todos los comandos que hemos ejecutado.
* **touch**: Crea un archivo vacío con el nombre que le indiquemos.
* **nano**: Es un editor dentro de la consola, podemos abrir cualquier archivo y modificarlo.
* **mv**: Permite mover archivos entre distintas carpetas, solamente debemos indicarle el nombre del archivo y la ruta de destino.
* **rm**: Elimina únicamente un archivo, añadiendo el parámetro -rf podemos eliminar directorios también.

### Herramientas básicas (Comandos CAT, MORE, TAIL y OPEN)
* **cat**: permite visualizar un archivo completo en la terminal.
* **more**: muestra por partes un archivo dentro de la terminal.
* **tail**: muestra las últimas 10 líneas de cada archivo, se puede modificar pasándole el parámetro con el número de líneas -15.
* **open**: abre un archivo con el programa que tengamos por defecto.




