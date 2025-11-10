# Teoría Markdown
## Archivos Markdown

Podemos crear un archivo de texto plano con diferentes extensiones para archivos de Markdown dependiendo del destino del archivo:

- `.markdown`
- `.md`
- `.mkd`
- `.mkdown`
- `.text`
- `.mdown`

GitHub utiliza principalmente la extensión `.md` para los archivos, por ejemplo `README.md`.



## Etiquetas básicas de Markdown

### Encabezados

Los encabezados llevan asociado un estilo por defecto y sirven para iniciar secciones de documentos.

Ejemplos:

    # H1
    ## H2
    ### H3
    #### H4
    ##### H5
    ###### H6



### Estilos de letra

Itálica o cursiva:

    *texto*
    _texto_

Negrita:

    **texto**
    __texto__

Tachado:

    ~~texto~~

Anidar estilos (combinar formatos):

    **palabra1 _palabra2_**




### Listas

#### Listas ordenadas

    1. Primer elemento de lista
    2. Segundo elemento de lista
    3. Tercer elemento de lista

- El número en el código no tiene que ser exacto, Markdown genera la numeración correcta al mostrarlo.

Sublista ordenada (usando sangría):

    1. Elemento principal
        1. Sub-elemento ordenado

#### Listas desordenadas

    * Elemento de lista desordenada
    - Otro elemento de lista desordenada
    + Otro elemento de lista desordenada

Sublista desordenada:

    * Elemento
        * Sub-elemento



### Párrafos

Para crear un nuevo párrafo se deja una línea en blanco entre bloques de texto.

Ejemplo:

    Este es el primer párrafo.

    Este es el segundo párrafo.


### Código

Código en línea:

    Esto es `codigo_en_linea`.

Bloques de código:

Usamos tres acentos graves (backticks) antes y después del bloque:

    ```html
    <html>
        <head></head>
        <body></body>
    </html>
    ```


### Enlaces

Sintaxis básica:

    [Texto del enlace](https://ejemplo.com/ "Título opcional del enlace")

- El texto del enlace va entre corchetes `[]`.
- La URL va entre paréntesis `()`.
- El título entre comillas es opcional (aparece al pasar el ratón por encima).

### Imágenes

Sintaxis inline:

    ![Texto alternativo](https://ruta-de-la-imagen.png "Título opcional de la imagen")

Sintaxis con referencia:

    ![alt text][logo]

    [logo]: https://ruta-de-la-imagen.png "Título opcional"



### Tablas

Ejemplo de tabla en Markdown:

    | Tables        | Are           | Cool |
    |--------------:|:------------:|-----:|
    | col 3 is      | right-aligned| $1600|
    | col 2 is      | centered     |   $12|
    | zebra stripes | are neat     |    $1|

- La primera línea define los encabezados.
- La segunda línea usa guiones y dos puntos para marcar alineación:
  - `:---` izquierda
  - `:---:` centrado
  - `---:` derecha
- No es necesario que las barras verticales estén perfectamente alineadas visualmente.



### Notas al pie de página

Ejemplo:

    Texto con nota al pie[^1]

    [^1]: Aquí encuentras el texto de la nota al pie.



### Listas de verificación

Ejemplo de checklist:

    - [ ] A
    - [x] B
    - [ ] C

- `[ ]` crea una casilla vacía.
- `[x]` crea una casilla marcada.
- Es importante dejar un espacio en blanco entre los corchetes en las casillas vacías.

# Introducción a HTML

HTML (HyperText Markup Language) es el lenguaje de marcado estándar para crear páginas web. Es el lenguaje más importante de Internet, ya que sin HTML no se vería nada en el navegador.

HTML define la estructura y el contenido de las páginas web mediante etiquetas. Es adaptable, tiene una estructura lógica y es fácil de entender. HTML **describe el contenido**, no su comportamiento (eso lo hacen otros lenguajes como JavaScript) ni su diseño visual (para eso usamos CSS).

Los elementos HTML son los bloques de construcción de las páginas web.

Cada elemento HTML está delimitado por etiquetas como `<html>`, `<head>`, `<body>`, `<p>`, `<h1>`, etc.

# Nota:
HTML es un lenguaje de marcado, no un lenguaje de programación. No tiene bucles, condicionales o funciones como tal; su función es estructurar la información.

## Significado de HTML (HyperText Markup Language)

- **HyperText**: texto que enlaza con otros contenidos (otras páginas o recursos). Es la base del funcionamiento de la web como red de documentos conectados.
- **Markup**: marca o etiqueta. Todas las páginas web están construidas en base a etiquetas. Una etiqueta HTML identifica partes del contenido, por ejemplo:
  
  ```html
  <p>Hola</p>

## Introducción a HTML

HTML (HyperText Markup Language) es el lenguaje de marcado estándar para crear páginas web. Es esencial porque sin HTML no se mostraría contenido en el navegador.

HTML define la estructura y el contenido de las páginas web mediante etiquetas. Es un lenguaje:

- Basado en etiquetas.
- Lógico y fácil de leer.
- Que describe el contenido, no el estilo (CSS) ni la lógica de programación (JavaScript).

Las siglas significan:

- **HyperText**: texto que puede enlazar con otros documentos o recursos.
- **Markup**: marcado o etiquetado del contenido usando etiquetas.
- **Language**: conjunto de reglas y sintaxis propias, pero no es un lenguaje de programación.

# Comentario: Importante dejar claro que HTML organiza y marca contenido, no programa lógica.

## Elementos HTML

Un elemento HTML suele estar formado por:

- Etiqueta de apertura.
- Contenido.
- Etiqueta de cierre.

Ejemplo:

    <p>Mi gato es muy gruñón</p>

- `<p>` es la etiqueta de apertura.
- `Mi gato es muy gruñón` es el contenido.
- `</p>` es la etiqueta de cierre.

Los elementos deben anidarse correctamente:

    <p>Texto con <b>negrita</b> correcta</p>

Ejemplo incorrecto:

    <p>Texto con <b>negrita</p></b>

## Atributos HTML

Los atributos añaden información extra a un elemento.

Ejemplo:

    <p class="editor-note">Mi gato es muy gruñón</p>

Reglas básicas:

- Se escriben en la etiqueta de apertura.
- Formato: nombre="valor".
- Siempre separados por espacios.

Ejemplos típicos:

    <img src="imagen.jpg" alt="Descripción">
    <a href="https://ejemplo.com">Enlace</a>

Existen elementos vacíos (sin contenido interno), como:

    <img src="foto.jpg" alt="Foto">
    <br>
    <input type="text">

## Resumen de normas básicas de etiquetas HTML

- Normalmente vienen en pares: apertura y cierre.
- Algunas son vacías y no tienen cierre (img, br, input).
- Deben anidarse correctamente.
- Los atributos se indican en la etiqueta de apertura con nombre="valor".
- Recomendación: usar siempre minúsculas en etiquetas y atributos.

# Comentario: Estas normas evitan errores comunes y aseguran que el navegador interprete bien la página.

## Estructura básica de un fichero HTML

Una página HTML básica incluye:

- Declaración `<!DOCTYPE html>`.
- Elemento `<html>`.
- Dentro de `<html>`, un `<head>` y un `<body>`.

Ejemplo:

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8">
        <title>Mi página de prueba</title>
        <link rel="icon" href="favicon.png">
    </head>
    <body>
        <img src="images/firefox-icon.png" alt="Mi imagen de prueba">
    </body>
    </html>

Explicación rápida:

- `<!DOCTYPE html>`: tipo de documento (HTML5).
- `<html>`: raíz del documento.
- `<head>`: metadatos, título, enlaces a CSS, scripts, iconos, SEO, etc.
- `<body>`: contenido principal visible.

Ejemplos de metadatos habituales en `<head>`:

    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="robots" content="index, follow">
    <meta name="description" content="Descripción de la página">
    <link rel="stylesheet" href="styles.css">

## Elementos de bloque y de línea

Dentro del `<body>` los elementos se dividen en:

### Elementos de bloque (block)

- Ocupan todo el ancho disponible.
- Empiezan en una nueva línea.
- Pueden contener otros elementos.

Ejemplos:

    <h1>...</h1>
    <p>...</p>
    <div>...</div>
    <ul>...</ul>
    <li>...</li>
    <section>...</section>
    <article>...</article>
    <header>...</header>
    <footer>...</footer>
    <blockquote>...</blockquote>
    <pre>...</pre>

### Elementos de línea (inline)

- Ocupan solo el espacio necesario.
- Se colocan dentro de la línea, sin saltar a otra nueva.
- Normalmente forman parte de un bloque.

Ejemplos:

    <a>...</a>
    <em>...</em>
    <strong>...</strong>
    <span>...</span>
    <q>...</q>
    <img ...>
    <code>...</code>
    <abbr>...</abbr>
    <cite>...</cite>


# Teoría HTML (Ampliación)

# Comentario: Esta sección amplía la teoría de HTML con enlaces internos (anclas), contenedores, elementos semánticos, legibilidad, comentarios, listas, rutas e imágenes.

## Enlaces internos (anclas)

Algunos documentos HTML pueden ser muy extensos y puede interesarnos navegar dentro de la misma página. Para ello usamos anclas, combinando el atributo `id` en el elemento destino con enlaces que usan `href="#id"`.

Para marcar el destino:

```html
<h2 id="seccion1">Sección 1</h2>

Comentario: El atributo id identifica el punto al que queremos saltar y el enlace con href="#id" crea la navegación interna o entre documentos hacia esa ancla.
Contenedores <div>

Un <div> es una caja o contenedor de tipo bloque que se utiliza para agrupar diferentes elementos dentro de una página web.

Se usa para:

Organizar contenido en secciones (cabecera, cuerpo, pie, columnas, etc.).

Aplicar estilos CSS a conjuntos de elementos.

Trabajar con JavaScript sobre partes concretas del documento.

Ejemplo:

<div class="myDiv">
    <h2>Título dentro del div</h2>
    <p>Este es un texto dentro de un div.</p>
</div>

Comentario: <div> sirve para dividir y agrupar contenido, pero no aporta significado semántico; solo estructura.
Elementos semánticos en HTML5

Los elementos semánticos permiten describir el contenido dándole un significado correcto, mejor que usar solo <div> para todo.

Ejemplos:

<header>: cabecera de la página o sección.

<footer>: pie de página o sección.

<nav>: bloque de navegación.

<section>: sección temática de contenido.

<article>: contenido independiente (noticia, post, entrada de blog).

<figure>: contenido ilustrativo (imagen, gráfico, etc.) con posible pie.

Comentario: El HTML semántico ayuda a que navegadores, buscadores y lectores de pantalla entiendan qué es cada parte del contenido.
Legibilidad y organización del código

La legibilidad del código fuente es la claridad con la que está escrito para que cualquier persona pueda entenderlo de manera fácil y rápida. Es fundamental que el código HTML sea legible.

Debemos tener en cuenta que:

Normalmente no trabajaremos solos.

Otro desarrollador debe poder entender qué hemos hecho y por qué.

Incluso nosotros mismos, al volver al proyecto, necesitamos recordar la lógica.

Por organización del código entenderemos:

Estructurar la aplicación en varios archivos cuando sea necesario.

Colocar los archivos en directorios adecuados.

Técnicas clave:

Uso de comentarios.

Buena indentación.

Organización coherente de los archivos.






