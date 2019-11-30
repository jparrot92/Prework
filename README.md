# Prework: Buenas Prácticas y Entorno de Desarrollo<!-- omit in toc -->

## Tabla de Contenido<!-- omit in toc -->
- [Introducción a la línea de comandos](#introducción-a-la-línea-de-comandos)
  - [Instalación de Ubuntu Bash en Windows](#instalación-de-ubuntu-bash-en-windows)
  - [Manejo archivos y directorios](#manejo-archivos-y-directorios)
  - [Herramientas básicas (Comandos CAT, MORE, TAIL y OPEN)](#herramientas-básicas-comandos-cat-more-tail-y-open)
  - [Crea llaves SSH](#crea-llaves-ssh)
- [Configuración entorno de desarrollo](#configuración-entorno-de-desarrollo)
  - [Cómo instalar NodeJS](#cómo-instalar-nodejs)
  - [Instalación y configuración de VSCode](#instalación-y-configuración-de-vscode)
  
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

### Crea llaves SSH
Las llaves SSH nos van a ayudar para autentificarnos con servidores. SSH utiliza criptografía asimétrica, o sea, tenemos dos llaves:

* **Pública**: la llave pública la podemos compartir por internet.
* **Privada**: debes tenerla en un sitio seguro y no debe ser compartida.
Tener una llave SSH nos permitirá una conexión fácil y segura con servidores, en el caso de la escuela de JavaScript nos va a servir para conectarnos con GitHub.

Para crear una llave SSH utilizamos el siguiente comando:
```bash
ssh-keygen -t rsa -b 4096 -C llave, puede ser tu correo> 
```

## Configuración entorno de desarrollo

### Cómo instalar NodeJS
Node es el entorno de ejecución que tenemos para JavaScript en el lado del servidor, está basado en el motor V8 de Google Chrome. Fue creado por Ryan Dahl en el 2009, es Open Source y multiplataforma.

**Revisión de Node en nuestro sistema**

En la mayoría de sistemas basados en Unix ya viene instalado por defecto Node, para asegurarnos de que esté instalado debemos irnos a nuestra terminal de comandos y ejecutar:
```bash
$ node -v
```

Esto nos debería mostrar la versión de node que tenemos instalados en el sistema, por ejemplo:
```bash
$ node -v v12.4.0
```

Si la respuesta que obtenemos es:
```bash
$ node -v command not found: node
```

Debemos instalarlo

**Instalación de Node en MacOS**

Para esta instalación vamos a requerir de homebrew. Este es un gestor de paquetes excelente para Mac y que vamos a usar en varias clases de este curso, si no lo tienes instalado lo mejor es que lo hagas. En este link https://brew.sh/index_es encontrarás los pasos necesarios para instalarlo.
Una vez tengamos instalado homebrew solo debemos ejecutar en la terminal
```bash
$ brew install node
```

Este proceso podría tardar un rato dependiendo de la velocidad a la conexión a internet, ya que cuando se intenta instalar un paquete con homebrew este intenta actualizar todos los paquetes que se han instalado con él. Una vez esté listo puedes escribir en la terminal:
```bash
$ node -v
```

y ya debería aparecerte la versión instalada que tienes de Node. Igualmente, con npm ejecutaremos:
```bash
$ npm -v
```

y debería salirte la versión que tienes de npm.

**Instalación de Node en Linux**

Dependiendo de tu distribución de Linux deberás ejecutar comandos distintos, esto porque entre distribuciones cambiar el gestor de paquetes:
En distribuciones basadas en Debian y Ubuntu debes ejecutar:
```bash
$ sudo apt update
```
```bash
$ sudo apt install nodejs
```
```bash
$ sudo apt install npm
```

En distribuciones basadas en Arch:
```bash
$ pacman -S nodejs npm
```

**Instalación de Node en Windows:**

Esta es la instalación más sencilla y es una instalación clásica en Windows, únicamente descargamos un programa y le damos continuar, o si prefieres configuras la instalación según las opciones que están disponibles. El programa se descarga desde acá https://nodejs.org/en/#download y seleccionas la versión que desees (recomendada la versión igual o superior a las 12)

**Cómo ejecutar Node**

Una vez se tenga instalado Node en el sistema podemos hacer uso de él, en esta clase haremos un uso básico de sus comandos, a lo largo de la Escuela de JavaScript será utilizado. Lo primero que haremos será ejecutarlo y escribir un Hola mundo. En la terminal haremos lo siguiente:
```bash
$ node
> console.log('Hola mundo')
Hola mundo
>
```

Al escribir node se nos abrirá un shell interactivo donde podremos escribir código en JavaScript. Esta herramienta es esencial en el desarrollo porque es aquí donde podremos probar funcionalidades antes de insertarlas en nuestro proyecto.

**Cómo utilizar npm**

npm es el manejador de paquetes de Node con él podemos instalar dependencias a nuestro proyecto o instalar programas globalmente en nuestro sistema.

## Instalación y configuración de VSCode
Si la primera mejor amiga del programador es la línea de comandos, es momento de instalar y configurar el segundo mejor amigo del programador: el **editor de código.**

Existen multiples editores de código, para la escuela de JavaScript vamos a utilizar Visual Studio Code. Vamos a añadir diferentes plugins para VSCode:

* **Git Blame**: va a mostrar el autor de la línea de código en la que estemos trabajando.
* **ESLint**: es una herramienta de análisis de código estático para identificar patrones problemáticos encontrados en el código JavaScript, o sea, nuestro linter. Debemos instalar y configurar eslint para que siga el estilo de código que le indiquemos.
* **Color Highlight**: resalta el color que estemos escribiendo.
* **SASS**: es un preprocesador de CSS.
