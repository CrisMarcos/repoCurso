# Ejercicios - Tema 2: Ramas
## Ejercicio 1. Crear y listar ramas
### Crea un repositorio nuevo llamado tema2-ramas y realiza un primer commit con un archivo README.md. Después, crea dos ramas nuevas llamadas feature/header y feature/footer. Por último, ejecuta el comando necesario para mostrar todas las ramas disponibles e indica cuál es la rama activa.
- git add .
- git commit -m "Add Ejercicio2.md"
- git push

- git checkout -b feature/header
- git checkout main
- git checkout -b feature/footer
- $ git branch
  bugfix/camera
  bugfix/gps
  bugfix/login
  feature/camara
* feature/footer
  feature/gps
  feature/header
  feature/login
  main

La activa es la que se muestra en la terminal en verde y la que tiene un asterisco, en este caso feature/footer

## Ejercicio 2. Cambiar entre ramas
### Sitúate en la rama feature/header y crea un archivo llamado header.html con una estructura básica. Haz un commit con un mensaje descriptivo. Después, cambia a la rama feature/footer y comprueba si el archivo header.html existe también en esa rama. Explica por qué ocurre ese comportamiento.
- git checkout main
- git pull
- git checkout feature/header
- Creamos el archivo header.html
- git add .
- git commit -m "Add header to the project"
- git push --set-upstream origin feature/header
- git checkout main
- git pull
- git checkout feature/footer

En la rama feature/footer no existe el archivo header.html, ya que no se ha actualizado, ni remeoto, ni bajado los cambios a feature/footer

## Ejercicio 3. Fusión de una rama sin conflicto
### En la rama feature/footer, crea un archivo llamado footer.html y guarda los cambios con un commit. Después, vuelve a la rama principal y fusiona feature/footer. Comprueba el historial de commits y explica qué ha ocurrido tras hacer el merge.
- Creamos el fichero footer.html
- git add .
- git commit -m "Add footer to the project"
- git checkout main
- git merge feature/footer
- git log
- git push
- Si nos vamos a github.com veremos que estamos un commit por detras, si nos situamos en la rama feature/header

## Ejercicio 4. Provocar un conflicto sencillo
### Crea una rama nueva llamada feature/title. Modifica en esa rama una misma línea del archivo README.md, por ejemplo el título principal, y haz un commit. Después, vuelve a la rama principal, modifica exactamente esa misma línea con un contenido diferente y haz otro commit. Intenta fusionar feature/title en la rama principal y observa qué mensaje muestra Git.
- git checkout -b feature/title
- Modificamos el fichero
- git add .
- git commit -m "changes in one line"
- git push --set-upstream origin feature/title
- Aparece la pull request en github.com
- git checkout main
- Hacemos cambios en la misma linea
- git add .
- git commit -m "Changes in the same line as the branch feature/title"
- Nos vamos a github, creamos la pull request y nos aparece que tenemos conflictos, creamos la pull request y nos aparece un mensaje que dice "This branch has conflicts that must be resolved"

## Ejercicio 5. Identificar archivos en conflicto
### Explica con tus palabras por qué se ha producido el conflicto.
- Se ha producido el conflicto porque hemos tocado la misma linea desde dos ramas diferentes y git no sabe con cual quedarse.

## Ejercicio 6. Resolver un conflicto manualmente
### Abre el archivo en conflicto y localiza las marcas <<<<<<<, ======= y >>>>>>>. Resuelve el conflicto manualmente dejando una única versión final coherente del contenido. Después, añade el archivo al área de preparación y completa el proceso de fusión con el commit correspondiente.
- Desde github.com, le damos a "Resolve conflicts".
- Elegimos el codigo con el que nos queremos quedar.
- Le damos a "Mark as resolved".
- Y hacemos commit.
- Y nos aparece como que ya no hay errores (No conflicts with base branch).
- Hacemos merge.
- Confirmamos merge.
- Borramos branch.
- Nos vamos a VSCode y actualizamos main
- git pull

## Ejercicio 7. Conflicto con varias líneas
### Crea una nueva rama llamada feature/about y añade una pequeña sección de presentación en un archivo about.md. Después, desde la rama principal, modifica también esa misma sección pero con un texto distinto. Intenta fusionar ambas ramas y resuelve el conflicto combinando parte del contenido de las dos versiones en lugar de quedarte solo con una.
- git checkout -b feature/about
- Creamos fichero
- git add .
- git commit -m "Add file about.md"
- git push --set-upstream origin feature/about
- Hacemos la pull request desde el github.com
- Nos vamos a VSCode y actualizamos main (git pull)
- Nos cambiamos de rama
- git checkout feature/about
- git pull
- git add .
- git commit -m "Changes a section of the file"
- git push
- Se hace un cambio en el mismo fichero desde main (en github.com) y se realiza el commit desde github.com.
- En VSCode hacemos: 
cmarcos@11LAPJRVTST3 MINGW64 /d/DOCUMENTOS/OTROS/CURSOS/INDRAWEB/GIT/repoCurso (feature/about)
$ git pull origin main
- Nos aparece una ventana en Visual para resolver los conflictos.
- Le damos a"Resolver en el Editor de combinación"
- Nos quedamos con lo que nos interese.
- Le damos a "Completar la fución mediante combinación".
- Hacemos el merge (se nos abre la inerfaz de git en visual), la damos a Continuar.
- Despues le damos a Sincronizar cambios (en la interfaz de git en visual).
- Le damos a Aceptar en el pop-up.
- git checkout main
- git merge feature/about
- git push.

## Ejercicio 8. Resolver un conflicto en VSCode o en GitHub
### Provoca de nuevo un conflicto entre dos ramas modificando la misma línea de un archivo. Si antes resolviste los conflictos usando VSCode trata de resolverlo diréctamente en GitHub o viceversa.

## Ejercicio 9. Tipos de ramas
### Investiga brevemente para qué se suelen utilizar ramas de tipo feature, bugfix, hotfix y release. Después, propón un ejemplo de nombre válido para cada una dentro de un proyecto web.

## Ejercicio 10. Caso práctico completo
### Imagina que estás trabajando en equipo y dos personas han editado la misma parte del archivo index.html: una ha cambiado el texto del encabezado y otra ha cambiado ese mismo texto en otra rama distinta. Describe paso a paso cómo resolverías el conflicto, indicando qué comandos usarías desde el momento en que Git detecta el conflicto hasta que la fusión queda completada.