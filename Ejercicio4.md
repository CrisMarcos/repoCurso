# Ejercicios - Tema 4: Tags, Releases, Workflows y Automatización en Git

## Ejercicio 1. Tags
Investiga qué es un tag en Git y explica con tus palabras para qué sirve. Después, crea un repositorio de prueba, realiza al menos un commit y añade un tag a ese punto del historial. Finalmente, ejecuta el comando necesario para mostrar todos los tags del repositorio.

## Ejercicio 2. Tags anotados
Crea varios commits en un repositorio y añade varios tags anotados cuando creas conveniente.

## Ejercicio 3. Releases
Crea una release usando algunos de los tags anteriores.

## Ejercicio 4. .gitignore
Crea un repositorio de prueba con varios archivos y carpetas, incluyendo algunos que no deberían subirse al repositorio, como archivos temporales, carpetas de dependencias o archivos de configuración local. Después, crea un archivo .gitignore y añade reglas para evitar que Git controle esos elementos. Finalmente, comprueba que Git deja de mostrarlos como cambios pendientes.

## Ejercicio 5. Hotfixes
Explica qué es un hotfix en Git y en qué situación se utiliza. Después, imagina que una aplicación ya publicada tiene un error urgente en producción. Describe qué pasos seguirías para crear una rama de hotfix, corregir el problema, integrar el arreglo en la rama principal y dejar el repositorio preparado para seguir trabajando con normalidad.

## Ejercicio 6. Trunk Based Development
Investiga en qué consiste el workflow trunk based. Después, explica cómo se organiza el trabajo en este modelo, qué papel tiene la rama principal y qué ventajas puede tener en equipos que integran cambios con mucha frecuencia. Finalmente, practica creando un repositorio donde uses esta estrategia para actualizar los cambios.

## Ejercicio 7. Forking Workflow y Feature Branch Workflow
Explica con tus palabras en qué consiste el forking workflow y en qué consiste el feature branch workflow. Después, compáralos brevemente indicando en qué se diferencian y en qué tipo de proyecto o equipo podría ser más recomendable cada uno de ellos.

## Ejercicio 8. Gitflow Workflow
Investiga cómo funciona el workflow gitflow. Después, identifica qué papel suelen tener ramas como master, develop, feature, release y hotfix. Responde qué ventajas puede ofrecer este modelo en proyectos grandes y qué posible inconveniente puede tener frente a workflows más simples.

Por último, crea un repositorio con toda la estructura de ramas necesaria para usar esta estrategia, haciendo varios commits y merges.

## Ejercicio 9. Hook pre-commit y commit-msg
Investiga qué es un hook en Git. Después, explica qué función tienen concretamente los hooks pre-commit y commit-msg. Finalmente, describe un ejemplo realista en el que pre-commit se usaría para validar el código antes de confirmar cambios y otro en el que commit-msg serviría para comprobar que el mensaje del commit sigue un formato determinado.

Trata de crear tu propio hook con o sin ayuda de una IA.

## Ejercicio 10. Hook pre-push
Explica qué hace el hook pre-push y en qué momento se ejecuta. Después, imagina que trabajas en un equipo donde no se puede subir código si los tests fallan. Describe cómo podría utilizarse este hook para impedir una subida incorrecta al repositorio remoto y qué ventaja tendría esta medida dentro de un flujo de trabajo colaborativo.