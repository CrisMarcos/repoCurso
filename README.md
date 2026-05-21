# Tutorial básico de Markdown

Markdown es un lenguaje de marcado ligero que permite dar formato a textos de forma sencilla. Se usa mucho en archivos `README.md`, documentación técnica, apuntes, blogs y plataformas como GitHub.

---

## 1. Títulos

Para crear títulos, se usa el símbolo `#`. Cuantos más símbolos `#` uses, menor será el nivel del título.

```markdown
# Título principal

## Título de segundo nivel

### Título de tercer nivel

#### Título de cuarto nivel
```

Resultado:

# Título principal

## Título de segundo nivel

### Título de tercer nivel

#### Título de cuarto nivel

---

## 2. Párrafos

Para escribir un párrafo normal, simplemente escribe el texto.

```markdown
Este es un párrafo escrito en Markdown.
```

Para separar párrafos, deja una línea en blanco entre ellos.

```markdown
Este es el primer párrafo.

Este es el segundo párrafo.
```

---

## 3. Negrita, cursiva y tachado

Puedes resaltar texto usando asteriscos `*` o guiones bajos `_`.

```markdown
**Texto en negrita**

_Texto en cursiva_

**_Texto en negrita y cursiva_**

~~Texto tachado~~
```

Resultado:

**Texto en negrita**

_Texto en cursiva_

**_Texto en negrita y cursiva_**

~~Texto tachado~~

---

## 4. Listas

### Listas desordenadas

Puedes crear listas usando guiones `-`, asteriscos `*` o signos `+`.

```markdown
- HTML
- CSS
- JavaScript
- Markdown
```

Resultado:

- HTML
- CSS
- JavaScript
- Markdown

### Listas ordenadas

Para crear listas numeradas, usa números seguidos de un punto.

```markdown
1. Crear el archivo
2. Escribir el contenido
3. Guardar los cambios
4. Subirlo a GitHub
```

Resultado:

1. Crear el archivo
2. Escribir el contenido
3. Guardar los cambios
4. Subirlo a GitHub

### Listas anidadas

También puedes crear sublistas usando espacios o tabulaciones.

```markdown
- Frontend
  - HTML
  - CSS
  - JavaScript
- Backend
  - Java
  - Spring
  - MySQL
```

Resultado:

- Frontend
  - HTML
  - CSS
  - JavaScript
- Backend
  - Java
  - Spring
  - MySQL

---

## 5. Enlaces

Para crear enlaces, se usa esta estructura:

```markdown
[Texto del enlace](https://www.ejemplo.com)
```

Ejemplo:

```markdown
[Visitar GitHub](https://github.com)
```

Resultado:

[Visitar GitHub](https://github.com)

---

## 6. Imágenes

Las imágenes son parecidas a los enlaces, pero empiezan con un signo de exclamación `!`.

```markdown
![Texto alternativo](ruta-o-url-de-la-imagen)
```

Ejemplo:

```markdown
![Logo de Markdown](https://markdown-here.com/img/icon256.png)
```

El texto alternativo es importante porque describe la imagen si no se puede cargar o si el usuario utiliza un lector de pantalla.

---

## 7. Código

Markdown permite mostrar código de dos formas: en línea o en bloque.

### Código en línea

Usa comillas invertidas simples `` ` ``.

```markdown
La etiqueta `h1` se usa para títulos principales en HTML.
```

Resultado:

La etiqueta `h1` se usa para títulos principales en HTML.

### Bloques de código

Usa tres comillas invertidas antes y después del bloque.

````markdown
```javascript
const greeting = "Hola, Markdown";
console.log(greeting);
```
````

Resultado:

```javascript
const greeting = "Hola, Markdown";
console.log(greeting);
```

También puedes indicar el lenguaje para que se aplique resaltado de sintaxis, por ejemplo:

````markdown
```html
<h1>Hola mundo</h1>
```
````

````

```markdown
```css
body {
  font-family: Arial, sans-serif;
}
````

````

```markdown
```sql
SELECT * FROM users;
````

````

---

## 8. Citas

Para crear una cita, usa el símbolo `>`.

```markdown
> Esta es una cita en Markdown.
````

Resultado:

> Esta es una cita en Markdown.

También puedes crear citas con varias líneas:

```markdown
> Markdown es sencillo.
> Permite escribir documentación clara.
> Se usa mucho en GitHub.
```

Resultado:

> Markdown es sencillo.  
> Permite escribir documentación clara.  
> Se usa mucho en GitHub.

---

## 9. Líneas horizontales

Para separar secciones, puedes usar tres guiones, tres asteriscos o tres guiones bajos.

```markdown
---
```

Resultado:

---

También funcionan:

```markdown
---
---
```

---

## 10. Tablas

Puedes crear tablas usando barras verticales `|` y guiones `-`.

```markdown
| Tecnología | Uso principal                |
| ---------- | ---------------------------- |
| HTML       | Estructura de una página web |
| CSS        | Estilos y diseño             |
| JavaScript | Interactividad               |
| Markdown   | Documentación                |
```

Resultado:

| Tecnología | Uso principal                |
| ---------- | ---------------------------- |
| HTML       | Estructura de una página web |
| CSS        | Estilos y diseño             |
| JavaScript | Interactividad               |
| Markdown   | Documentación                |

También puedes alinear columnas:

```markdown
| Izquierda | Centro | Derecha |
| :-------- | :----: | ------: |
| Texto     | Texto  |   Texto |
| Texto     | Texto  |   Texto |
```

Resultado:

| Izquierda | Centro | Derecha |
| :-------- | :----: | ------: |
| Texto     | Texto  |   Texto |
| Texto     | Texto  |   Texto |

---

## 11. Checklists o listas de tareas

En plataformas como GitHub, puedes crear listas de tareas con casillas.

```markdown
- [x] Crear el archivo README.md
- [x] Añadir títulos
- [ ] Añadir imágenes
- [ ] Revisar el documento
```

Resultado:

- [x] Crear el archivo README.md
- [x] Añadir títulos
- [ ] Añadir imágenes
- [ ] Revisar el documento

---

## 12. Escapar caracteres especiales

Algunos símbolos tienen significado especial en Markdown. Si quieres mostrarlos como texto normal, puedes usar una barra invertida `\`.

```markdown
\*Este texto no aparece en cursiva\*
```

Resultado:

\*Este texto no aparece en cursiva\*

Otros caracteres que a veces conviene escapar son:

```markdown
\#
\- \*
\[
\]
\(
\)
```

---

## 13. Ejemplo completo de README.md

Este es un ejemplo básico de estructura para un archivo `README.md`.

````markdown
# Nombre del proyecto

Breve descripción del proyecto.

## Tecnologías utilizadas

- HTML
- CSS
- JavaScript

## Instalación

1. Clona el repositorio:

```bash
git clone https://github.com/usuario/nombre-del-proyecto.git
```
````

2. Entra en la carpeta del proyecto:

```bash
cd nombre-del-proyecto
```

3. Abre el archivo `index.html` en el navegador.

## Uso

Explica brevemente cómo se utiliza el proyecto.

## Autor

Creado por Nombre del autor.

## Licencia

Este proyecto está bajo la licencia MIT.

---

## 14. Buenas prácticas al escribir Markdown

- Usa títulos claros y jerárquicos.
- No abuses de la negrita.
- Deja líneas en blanco para mejorar la legibilidad.
- Usa listas para ordenar información.
- Añade ejemplos de código cuando expliques comandos o sintaxis.
- Mantén el archivo `README.md` actualizado.
- En GitHub, comprueba siempre cómo se visualiza el archivo después de subirlo.

---

## 15. Resumen rápido de sintaxis

| Elemento          | Sintaxis                 |
| ----------------- | ------------------------ |
| Título 1          | `# Título`               |
| Título 2          | `## Título`              |
| Negrita           | `**texto**`              |
| Cursiva           | `*texto*`                |
| Tachado           | `~~texto~~`              |
| Lista desordenada | `- elemento`             |
| Lista ordenada    | `1. elemento`            |
| Enlace            | `[texto](url)`           |
| Imagen            | `![alt](url)`            |
| Código en línea   | `` `código` ``           |
| Bloque de código  | Tres comillas invertidas |
| Cita              | `> texto`                |
| Línea horizontal  | `---`                    |
| Checklist         | `- [ ] tarea`            |

---

## Conclusión

Markdown es una herramienta sencilla pero muy útil para escribir documentación clara y bien estructurada. Con unas pocas reglas puedes crear archivos `README.md`, apuntes, guías y documentación técnica de forma rápida y legible.


# Hooks

> Para modificar los hooks hay que entrar en .git -> hooks y borrar el .sample del hook que queramos

> Si queremos modificarlos directamente desde VSCode debemos ir a File -> Preferences -> Settings -> Escribir en el buscador files.exclude y eliminar o modificar el patrón **/.git

############################# pre-commit:

```sh
#!/bin/sh
echo "Hola desde el hook"
exit 0
```
-------------------------------------------------------

```sh
#!/bin/sh

echo "Comprobando console.log en archivos preparados para commit..."

files=$(git diff --cached --name-only --diff-filter=ACM | grep -E '\.(js|jsx|ts|tsx|vue)$')

found=0

for file in $files; do
  if git show ":$file" | grep -n "console\.log" > /dev/null; then
    echo "Se ha encontrado console.log en: $file"
    found=1
  fi
done

if [ "$found" -eq 1 ]; then
  echo ""
  echo "Commit cancelado. Elimina los console.log antes de hacer commit."
  exit 1
fi

echo "No se han encontrado console.log."
exit 0
```
--------------------------------------------------------
```sh
#!/bin/sh

echo "Ejecutando comprobación..."

if grep -R "console.log(" . --exclude-dir=.git --include="*.js" > /dev/null; then
  echo "Error: has dejado un console.log en archivos JS"
  exit 1
fi

echo "Todo correcto"
exit 0
```

############################# commit-msg:
```sh
#!/bin/sh

commit_msg_file="$1"
commit_msg=$(cat "$commit_msg_file")

if [ ${#commit_msg} -lt 10 ]; then
  echo "Error: el mensaje del commit debe tener al menos 10 caracteres"
  exit 1
fi

exit 0
```
--------------------------------------------------------
```
git commit -m "mensaje corto" --no-verify
```
--------------------------------------------------------
```sh
#!/bin/sh

commit_msg_file="$1"
commit_msg=$(cat "$commit_msg_file")

case "$commit_msg" in
  feat:*|fix:*|docs:*)
    exit 0
    ;;
  *)
    echo "Error: el mensaje debe empezar por feat:, fix: o docs:"
    exit 1
    ;;
esac
```

############################# pre-push:
```sh
#!/bin/sh

branch=$(git branch --show-current)

if [ "$branch" = "main" ]; then
  echo "Error: no puedes hacer push directamente a main"
  exit 1
fi

echo "Push permitido en la rama $branch"
exit 0
```