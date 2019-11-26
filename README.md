# Prework: Buenas Prácticas y Entorno de Desarrollo<!-- omit in toc -->

## Tabla de Contenido<!-- omit in toc -->
- [Introducción a la línea de comandos](#introducción-a-la-línea-de-comandos)
  - [Manejo archivos y directorios](#manejo-archivos-y-directorios)
  - [Herramientas básicas (Comandos CAT, MORE, TAIL y OPEN)](#herramientas-básicas-comandos-cat-more-tail-y-open)
  
## Introducción a la línea de comandos

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
