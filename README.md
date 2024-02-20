# Curso Introductorio Git y Github

## ¿Qué es Git?
Git es un sistema de control de versiones distribuido que permite a los desarrolladores rastrear y gestionar los cambios en el código fuente de manera eficiente. Es ideal para la colaboración en equipo, ya que facilita la integración de cambios de múltiples fuentes.

## ¿Qué es GitHub?
GitHub es una plataforma en línea que utiliza Git para almacenar y gestionar repositorios de código. Permite la colaboración entre desarrolladores y ofrece herramientas para el trabajo en equipo, como seguimiento de problemas, solicitudes de extracción y gestión de proyectos.

## Conceptos Básicos

### Repositorio
Un **repositorio** en Git es como un gran archivo de almacenamiento donde se guardan todos los archivos de tu proyecto junto con el historial de todos los cambios realizados a cada archivo. Piensa en ello como un álbum de fotos que registra cada paso de tu proyecto.

### Staging Area (Área de Preparación)
La **staging area** es como una sala de espera para tus archivos. Cuando realizas cambios en tus archivos, estos se encuentran en el "working directory" (directorio de trabajo). Al añadir estos archivos a la staging area, estás preparándolos para ser parte de tu próximo "commit". Es como decir, "Ok, estos cambios están listos para ser guardados permanentemente".

### Commit
Un **commit** es como un punto de guardado en el tiempo de tu proyecto. Cada commit guarda una versión específica de tu proyecto. Si cometes un error, puedes volver a un commit anterior. Es como un "guardar" en un videojuego, pero para tu código.

### Branch (Rama)
Imagina un **branch** o rama en Git como una versión paralela de tu proyecto. Es como trabajar en un borrador de un documento mientras el documento original permanece intacto. En principio, todos los proyectos en Git comienzan con una sola rama llamada `master` o `main`, pero puedes crear nuevas ramas para experimentar con cambios o desarrollar nuevas características, sabiendo que tu rama principal no será afectada.

### Repositorio Remoto
Un **repositorio remoto** es como una copia de seguridad de tu proyecto que se almacena en Internet, no en tu computadora personal. Esto te permite compartir tu proyecto con otros, y también actúa como un respaldo seguro. Piensa en ello como almacenar tus fotos tanto en tu teléfono como en la nube; si pierdes tu teléfono, aún tienes las fotos en la nube.

### Push (Empujar)
El comando **push** se usa para enviar tus cambios locales (por ejemplo, commits que has hecho en tu computadora) a un repositorio remoto. Es como actualizar la versión en línea de tu proyecto con los últimos cambios que has realizado localmente. 

### Clone
**Clonar** es el acto de crear una copia local de un repositorio que está en un servidor remoto (como GitHub). Esto te permite trabajar en el proyecto desde tu propia máquina. Es como descargar un proyecto completo para trabajar en él localmente.


## Comandos Básicos de Git

### ```git init```
Inicializa un nuevo repositorio de Git en tu directorio actual.

### ```git add <nombre del archivo 1> <nombre del archivo 2> ```
Agrega archivos al área de preparación (staging area) para que sean incluidos en el próximo commit.

### ```git add .```
Agrega todos los archivos al staging area dentro de tu folder

### ```git commit -m "Mensaje Descriptivo de tu commit"```
Guarda los cambios en el repositorio con un mensaje descriptivo.

### ```git remote add origin <url>  ```
Agrega un nuevo remoto, es decir, agrega tu repositorio a la nube, como github

### ```git push origin <branch>```
Envía los commits locales a un repositorio remoto.

### ``` git pull ```
Obtiene los cambios que existen de tu repositorio remoto 

### ``` git revert <commit_hash> ```
Deshace los cambios y vuelve a un commit anterior

### ``` git clone <repositorio remoto> ```
Clona un repositorio remoto, si es privado tendrás que tener acceso al mismo

## Receta de Cocina
1. Encuentra tu proyecto y asegurate que estás en el directorio
2. Abre la terminal o cmd dentro del directorio de tu proyecto
3. Incia tu repositorio local con ``` git init ```
4. Agrega tus archivos con ``` git add . ``` 
5. O si quieres agregar archivos específicos ``` git add <archivo> ```
6. Crea un commit con ``` git commit -m "mensaje" ```
7. Crea tu branch principal ``` git branch -M main ```
8. Agrega tu repositorio remoto donde quieras que esté hosteado ``` git remote add origin <url> ```
9. Sube tus cambios con ``` git push -u origin main ```
10. Repetir pasos 4,5,6 y 9 para nuevos cambios

## Implementación con Netbeans

### Inicia un repositorio en tu proyecto

![Selecciona si quieres iniciar un proyecto o clonar](https://cdn.discordapp.com/attachments/787786979940368384/1209550692419764254/image.png?ex=65e754dd&is=65d4dfdd&hm=04fbdea5bc809569ef7a49720c7cd4ac78cea54776f23a685a96135812617701&)

### Si tienes uno existente en github, puedes clonarlo
![Wizard para clonar](https://cdn.discordapp.com/attachments/787786979940368384/1209554543222726707/clone-wizard-small.png?ex=65e75873&is=65d4e373&hm=3d4f1d5d532b5a6403de6747dbb2cd1f2a7d7076ddf954193a54aca04aaefb74&)


### Una vez que hayas creado el repositorio los archivos añadidos aparecerán de la siguiente manera
![Se pone en verde el archivo](https://cdn.discordapp.com/attachments/787786979940368384/1209553531866972344/image.png?ex=65e75782&is=65d4e282&hm=575e1aa086884d2f0df70a7677d1b38d7fcabd0d71dbfb359b33865227cca20f&)

### Y tendrás un nuevo menú para trabajar con tu repositorio
![Nuevo Menu](https://cdn.discordapp.com/attachments/787786979940368384/1209558949528084603/image.png?ex=65e75c8e&is=65d4e78e&hm=8f01295ba566335b6087eee78f6419349810a4551e82bc9ae9ca7df2484067ee&)

### Viendo los cambios al trabajar en tu proyecto

- Azul: Líneas que han cambiado desde la versión anterior
- Verde: Líneas que han sido añadidas desde la versión anterior
- Rojo: Líneas que han sido removidas desde la versión anterior

![Ejemplo de las líneas](https://cdn.discordapp.com/attachments/787786979940368384/1209555882388492330/left-margin.png?ex=65e759b2&is=65d4e4b2&hm=0b2341392e5c91a28085f1b5e0c057d4399b780ad423c4eaf85a1fe745510730&)

### Haz tu commit
Netbeans te proporciona una GUI para poder escribir tu mensaje, ver los archivos que serán cambiados, borrados y/o agregados.

![Commit](https://cdn.discordapp.com/attachments/787786979940368384/1209560122830098523/image.png?ex=65e75da5&is=65d4e8a5&hm=d9efff6ce680bcb8ec44257d45cda5e7ccd8e10d5907481fa84ecdf4edc98148&)

### Sube tus cambios a tu repositorio de github
Entra a Teams --> Remote --> Push. Escribe tu repositorio (no olvides https) y digita tus credenciales

![Push](https://cdn.discordapp.com/attachments/787786979940368384/1209561211289608192/image.png?ex=65e75ea9&is=65d4e9a9&hm=90983be7cb7675600fd3bcf8b4b450d11130119e2875f8b06ec5d32b4f7f7b7a&)