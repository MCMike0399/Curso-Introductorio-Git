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

### ```git remote add <nombre> <url>  ```
Agrega un nuevo remoto, es decir, agrega tu repositorio a la nube, como github

### ```git push```
Envía los commits locales a un repositorio remoto.

### 

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

