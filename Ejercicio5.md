# Ejercicios - Tema 5: GitLab, Restore, Revert, Pipelines y GitHub Actions
A continuación, encontrarás 10 ejercicios prácticos sobre trabajo con GitLab, restauración de cambios, reversión de commits, pipelines y automatización con GitHub Actions. Intenta resolverlos antes de consultar la teoría.

## Ejercicio 1. Crear un repositorio en GitLab y clonarlo
Crea un nuevo repositorio en GitLab con el nombre tema5-gitlab. Después, copia la URL del repositorio y clónalo en tu equipo con el comando correspondiente.

## Ejercicio 2. Add, commit y push en GitLab
Dentro del repositorio clonado, crea un archivo README.md con una breve descripción del proyecto. Después, añade el archivo al área de preparación, realiza un commit con un mensaje descriptivo y sube los cambios al repositorio remoto. Finalmente, comprueba en GitLab que el archivo aparece correctamente en el proyecto.

## Ejercicio 3. Crear una rama y hacer un Merge Request
Crea una nueva rama de trabajo en tu repositorio de GitLab, realiza un pequeño cambio en un archivo y súbelo al repositorio remoto. Después, crea un Merge Request desde GitLab para proponer la integración de esa rama en la rama principal. Explica con tus palabras para qué sirve un Merge Request y por qué resulta útil en proyectos colaborativos.

## Ejercicio 4. Roles en GitLab y gestión de miembros
Investiga cómo se gestionan los miembros de un proyecto en GitLab desde la sección Manage y Members. Después, explica qué función tienen los roles dentro de un repositorio y por qué no todos los colaboradores deberían tener los mismos permisos. Finalmente, menciona al menos dos roles diferentes y describe brevemente qué nivel de acceso puede tener cada uno.

## Ejercicio 5. git restore file
Modifica el contenido de un archivo que ya esté siendo controlado por Git, pero sin hacer commit. Después, utiliza git restore nombre-del-archivo para deshacer los cambios realizados en ese archivo. Finalmente, comprueba el estado del repositorio y explica qué ha ocurrido.

## Ejercicio 6. git restore --staged file
Realiza cambios en un archivo y añádelo al área de preparación con git add. Después, utiliza git restore --staged nombre-del-archivo para sacarlo del área de preparación sin perder los cambios en el directorio de trabajo. Finalmente, ejecuta git status y explica la diferencia entre restaurar un archivo normal y restaurarlo desde el área de preparación.

## Ejercicio 7. git revert <commit-hash>
Realiza varios commits en un repositorio de prueba. Después, elige uno de ellos y reviértelo con el comando git revert <commit-hash>. Finalmente, consulta el historial del repositorio.

## Ejercicio 8. GitLab Revert
Investiga qué opción ofrece GitLab para revertir cambios desde su interfaz web. Después, explica en qué situación podría resultar útil hacer un revert desde GitLab en lugar de hacerlo manualmente desde la terminal. Finalmente, responde qué precaución deberías tener antes de revertir cambios en un repositorio compartido.

## Ejercicio 9. GitLab Pipelines
Investiga qué es una pipeline en GitLab y para qué sirve dentro de un proyecto. Después, imagina un repositorio en el que cada vez que se sube código se ejecutan automáticamente tests y comprobaciones. Explica qué ventajas tiene este sistema en un equipo y por qué puede ayudar a detectar errores antes de integrar cambios en la rama principal.

## Ejercicio 10. GitHub Actions y Secrets
Investiga qué es GitHub Actions y qué utilidad tiene dentro de un repositorio. Después, localiza en GitHub la ruta Settings → Secrets & Variables → Actions → New repository secret y explica para qué sirven los secrets. Crea un workflow sencillo y un secreto.