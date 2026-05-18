# Prueba Curso
## Ejercicio 1: Explica con tus palabras qué es Git y para qué sirve. Después, responde también qué diferencia existe entre Git y GitHub.
- Git es un controlador de versiones.
- GitHub es la interfaz web del git.
## Ejercicio 2: Instala Git en tu equipo según tu sistema operativo. Cuando termines, abre la terminal y ejecuta el comando necesario para comprobar que Git se ha instalado correctamente. Escribe el comando utilizado y anota la versión que te aparece.
- $ git --version
## Ejercicio 3: Configura Git con tu nombre y tu correo electrónico en modo global. Después, ejecuta el comando necesario para comprobar que la configuración se ha guardado correctamente.
- $ git config --get user.name
- $ git config --get user.email
- $ git config --list
## Ejercicio 4: Crea una carpeta llamada repoCurso. Entra en ella desde la terminal e inicializa un repositorio Git. Después, explica qué carpeta interna crea Git al ejecutar este proceso y cuál es su función.
- $ git init
## Ejercicio 5: Dentro del repositorio anterior, crea un archivo llamado README.md con una breve descripción del proyecto. Después, comprueba el estado del repositorio con el comando correspondiente y describe qué información te muestra Git.
- $ git status
## Ejercicio 6: Añade el archivo README.md al área de preparación y realiza un primer commit con un mensaje descriptivo. Después, consulta el historial de commits del repositorio.
- $ git status
- $ git add .
- $ git commit -m "Segundo commit"
## Ejercicio 7: Investiga qué hace el comando git clone y explica en qué situaciones se utiliza. Después, escribe un ejemplo realista de uso con una URL de repositorio.

## Ejercicio 8: Busca una interfaz gráfica para trabajar con Git, como GitHub Desktop, SourceTree o la integración de Visual Studio Code. Indica cuál has elegido y responde qué ventajas puede tener usar una GUI frente a trabajar solo con comandos en terminal.

## Ejercicio 9: Crea una cuenta en GitHub, o utiliza una que ya tengas. Después, crea un repositorio remoto llamado tema1-git, súbelo a tu perfil y explica qué utilidad tienen plataformas como GitHub en un proyecto de desarrollo.

## Ejercicio 10: Investiga qué es GitLab y compáralo brevemente con GitHub. Después, responde qué tienen en común ambas plataformas y menciona al menos una diferencia importante entre ellas.