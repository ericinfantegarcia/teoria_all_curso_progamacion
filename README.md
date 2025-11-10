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

Algunos documentos HTML pueden ser muy extensos y puede interesarnos navegar dentro de la misma página sin recargarla. Para ello utilizamos **anclas**, combinando el atributo `id` en el elemento destino con enlaces que apuntan a ese identificador.

### Definir el destino

    <h2 id="seccion1">Sección 1</h2>

### Enlace dentro de la misma página

    <a href="#seccion1" title="Sección 1">Ir a la sección 1</a>

### Enlace a un ancla en otro documento

    <a href="secciones.html#seccion1" title="Sección 1">Ir a la sección 1</a>

# Comentario: El atributo `id` marca el punto de destino y `href="#id"` o `href="archivo.html#id"` permite crear enlaces internos o entre páginas hacia esa ancla.


## Contenedores `<div>`

La etiqueta `<div>` define una **caja o contenedor de bloque** que sirve para agrupar diferentes elementos dentro de una página web.

### Usos principales

- Organizar contenido en secciones (cabecera, contenido, columnas, pie, etc.).
- Aplicar estilos CSS a grupos de elementos mediante clases o identificadores.
- Trabajar con JavaScript sobre partes específicas del documento.

### Ejemplo

    <div class="myDiv">
        <h2>Título dentro del div</h2>
        <p>Este es un texto dentro de un div.</p>
    </div>

# Comentario: `<div>` estructura y agrupa contenido, pero no aporta significado semántico; para eso existen los elementos semánticos.


## Elementos semánticos en HTML5

Los elementos semánticos permiten describir el contenido dándole un significado correcto, en lugar de usar solo `<div>` para todo.

### Ejemplos

- `<header>`: cabecera de la página o de una sección.
- `<footer>`: pie de página o de una sección.
- `<nav>`: bloque de navegación.
- `<section>`: sección temática de contenido.
- `<article>`: contenido independiente (noticia, post, entrada de blog).
- `<figure>`: contenido ilustrativo (imagen, gráfico, etc.), normalmente con `<figcaption>`.

# Comentario: El HTML semántico mejora la accesibilidad, el SEO y la claridad del código al indicar qué representa cada parte.


## Legibilidad y organización del código

La legibilidad del código fuente es la claridad con la que está escrito, de forma que cualquier persona pueda entenderlo fácil y rápidamente. Es fundamental que el HTML sea legible.

Debemos tener en cuenta que:

- Normalmente no trabajaremos solos.
- Otros desarrolladores pueden necesitar modificar nuestro código.
- Nosotros mismos tendremos que entenderlo tiempo después.

### Técnicas para mejorar la legibilidad

- Usar comentarios para marcar secciones o aclarar partes complejas.
- Mantener una indentación correcta y consistente.
- Organizar los archivos en directorios lógicos.
- Separar correctamente estructura (HTML), estilos (CSS) y lógica (JS) cuando proceda.

# Comentario: Un código bien organizado facilita el mantenimiento, la colaboración y la detección de errores.


## Comentarios en HTML

Los comentarios permiten añadir anotaciones que no se mostrarán en el navegador, pero son útiles para el desarrollador.

### Sintaxis

    <!-- comentario -->

### Ejemplo de uso estructural

    <body>
        <!-- Cabecera -->
        <!-- Menú de navegación -->
        <!-- Columna lateral con enlaces -->
        <!-- Sección principal con artículos -->
        <!-- Pie de página -->
    </body>

# Comentario: Es recomendable comentar secciones largas o importantes para localizar rápidamente cada parte del documento.


## Etiquetas básicas de HTML (resumen)

### Encabezados `<h1>` ... `<h6>`

Permiten especificar títulos y subtítulos del contenido.

- Son elementos de bloque.
- `<h1>` suele ser el título principal de la página.

### Párrafos `<p>`

Se utilizan para encerrar párrafos de texto (conjunto de frases relacionadas).

- Son elementos de bloque.

### Salto de línea `<br>`

Inserta un salto de línea dentro de un texto sin crear un nuevo párrafo.

- Es un elemento vacío (no tiene cierre).

### Separador de línea `<hr>`

Crea una línea horizontal divisoria que separa visualmente bloques de contenido.

- Es un elemento vacío de bloque.

### Énfasis `<em>` y `<strong>`

- `<em>`: marca texto con énfasis (normalmente cursiva).
- `<strong>`: marca texto con énfasis fuerte (normalmente negrita).

# Comentario: `<em>` y `<strong>` tienen valor semántico (indican importancia), no solo visual.

### Span `<span>`

`<span>` es un contenedor en línea que se usa para agrupar pequeñas partes de texto o elementos en una misma línea, generalmente para aplicar estilos o identificarlos.

- Es un elemento en línea.
- No rompe el flujo del texto.


## Listas en HTML

### Listas desordenadas `<ul>`

Se utilizan cuando el orden de los elementos no es relevante.

Estructura:

    <ul>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
    </ul>

Históricamente se podía usar el atributo `type` (`disc`, `square`, `circle`), aunque hoy se prefiere controlar la apariencia con CSS.

### Listas ordenadas `<ol>`

Se utilizan cuando el orden de los elementos sí es importante (pasos, instrucciones, etc.).

Estructura:

    <ol>
        <li>Paso 1</li>
        <li>Paso 2</li>
        <li>Paso 3</li>
    </ol>

Opciones de numeración con el atributo `type`:

- `type="1"` → 1, 2, 3...
- `type="A"` → A, B, C...
- `type="a"` → a, b, c...
- `type="I"` → I, II, III...
- `type="i"` → i, ii, iii...

Otros atributos útiles:

- `start="10"`: comienza la lista desde el número 10.
- `value="4"` en un `<li>`: fuerza un número concreto para ese elemento.

# Comentario: En cualquier tipo de lista, cada elemento debe ir siempre dentro de una etiqueta `<li>`.


## Listas de definición `<dl>`, `<dt>`, `<dd>`

Se utilizan para representar términos y sus definiciones.

Estructura general:

    <dl>
        <dt>HTML</dt>
        <dd>Lenguaje de marcas diseñado para estructurar documentos en la web.</dd>

        <dt>XML</dt>
        <dd>Metalenguaje extensible de etiquetas usado para definir otros lenguajes.</dd>
    </dl>

- `<dl>`: lista de definición.
- `<dt>`: término (definition term).
- `<dd>`: definición del término (definition description).

# Comentario: Son ideales para glosarios o para parejas concepto–explicación.


## Rutas en HTML (absolutas y relativas)

Cuando necesitamos enlazar a otros archivos (HTML, CSS, imágenes, etc.) usamos rutas para indicar su ubicación.

### Ruta absoluta

Especifica la dirección completa del recurso incluyendo el dominio.

Ejemplo:

    <img src="https://www.ejemplo.com/images/logo.png" alt="Logo del sitio">

- Útil cuando el recurso está en otro servidor o dominio.

### Ruta relativa

Especifica la ubicación del recurso en relación con el archivo actual.

Ejemplo de estructura:

    /mi-sitio/
        index.html
        /images/
            logo.png

Ejemplo de uso:

    <img src="images/logo.png" alt="Logo de mi sitio">

# Comentario: Las rutas relativas facilitan mover el proyecto completo sin romper los enlaces internos.


## Imágenes en HTML

Las imágenes son un recurso muy utilizado en el desarrollo web. Además de hacer más atractiva la aplicación, permiten transmitir información de forma visual.

La etiqueta para insertar imágenes es `<img>`, que es un elemento en línea y vacío (no tiene etiqueta de cierre clásica).

Sintaxis básica:

    <img src="media/logo.png" alt="Logo de la web" />

- `src`: indica la ruta (absoluta o relativa) del archivo de imagen.
- `alt`: texto alternativo que se mostrará si la imagen no se carga y que usan los lectores de pantalla.

# Comentario: Siempre hay que indicar el atributo `alt` para accesibilidad, SEO y buena práctica.

## Elementos semánticos en HTML5

El HTML semántico es clave para usar correctamente HTML. Los elementos semánticos describen el significado del contenido que encierran.

Un `<span>` agrupa contenido en línea y un `<div>` agrupa contenido en bloque, pero ninguno aporta significado semántico por sí mismo.  
En cambio, los elementos semánticos indican qué tipo de contenido contienen.

**Ejemplos de elementos semánticos:**

- `<header>`
- `<footer>`
- `<article>`
- `<section>`
- `<nav>`
- `<figure>`

Estos elementos proporcionan información sobre el tipo de contenido que contienen y ayudan a estructurar mejor la página.

# Comentario: El uso de elementos semánticos mejora accesibilidad, SEO y comprensión del código, porque cada zona tiene un rol claro.


## Legibilidad y organización del código

La legibilidad del código fuente es la claridad con la que está escrito, de forma que pueda entenderse de manera fácil y rápida.  
Es fundamental que el código HTML que generemos sea legible.

Debemos tener presente que normalmente no trabajaremos solos, por lo que un código claro ayuda a otros a entender qué hemos hecho y por qué.  
Incluso si solo lo tocamos nosotros, un código legible facilita recordar y modificar el trabajo.

Por **organización del código fuente** entendemos:

- Estructurar la aplicación web en varios archivos.
- Clasificar esos archivos en los directorios adecuados.

**Técnicas para un código legible y bien organizado:**

- Usar comentarios.
- Mantener una indentación correcta.
- Organizar los archivos y carpetas de forma lógica.

# Comentario: Código limpio + indentación consistente + comentarios = mantenimiento mucho más fácil.


## Comentarios en HTML

En un documento HTML podemos añadir anotaciones que no se mostrarán en el navegador, pero que son útiles para el desarrollador.

**Sintaxis:**

    <!-- comentario -->

Es muy importante comentar el código fuente, sobre todo si se trata de un documento largo o con muchas secciones.

**Ejemplo:**

    <body>
        <!-- Cabecera -->
        <!-- Menú de navegación -->
        <!-- Columna lateral con enlaces -->
        <!-- Sección principal con artículos -->
        <!-- Pie de página -->
    </body>

# Comentario: Los comentarios permiten marcar secciones y entender rápidamente la estructura del documento.


## Etiquetas básicas de HTML

### Encabezados `<h1>` ... `<h6>`

Permiten definir títulos y subtítulos del contenido.

- Son elementos de bloque.

### Párrafos `<p>`

Se utilizan para encerrar párrafos de texto, es decir, frases relacionadas entre sí.

- Son elementos de bloque.

### Salto de línea `<br>`

Inserta un salto de línea dentro de un texto sin crear un nuevo párrafo.

- Es un elemento vacío (no tiene etiqueta de cierre).

### Separador de línea `<hr>`

Inserta una línea horizontal divisoria, útil para separar visualmente bloques de contenido.

- Es un elemento vacío de bloque.

### Énfasis `<em>` y `<strong>`

- `<em>`: aplica énfasis (normalmente cursiva).
- `<strong>`: aplica énfasis fuerte o importancia (normalmente negrita).

### Span `<span>`

`<span>` es un contenedor en línea que agrupa pequeñas partes de texto o elementos sin romper la línea, normalmente para aplicar estilos o identificar contenido.

# Comentario: `<em>` y `<strong>` añaden significado (énfasis/importancia). `<span>` solo agrupa contenido en línea, sin semántica.


## Listas en HTML

### Listas desordenadas `<ul>`

Se utilizan cuando el orden de los ítems no es relevante.

    <ul>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
    </ul>

### Listas ordenadas `<ol>`

Se utilizan cuando el orden sí es importante.

    <ol>
        <li>Paso 1</li>
        <li>Paso 2</li>
        <li>Paso 3</li>
    </ol>

Se puede cambiar el tipo de numeración con el atributo `type` (`1`, `A`, `a`, `I`, `i`) y ajustar el inicio con `start`.

# Comentario: Cada elemento de lista debe ir siempre dentro de `<li>` para que la estructura sea correcta.


## Listas de definición `<dl>`, `<dt>`, `<dd>`

Las listas de definición representan términos y sus definiciones.

    <dl>
        <dt>HTML</dt>
        <dd>Lenguaje de marcas para estructurar documentos en la web.</dd>

        <dt>XML</dt>
        <dd>Metalenguaje extensible de etiquetas para definir otros lenguajes.</dd>
    </dl>

- `<dl>`: lista de definición.
- `<dt>`: término.
- `<dd>`: definición del término.

# Comentario: Útiles para glosarios y pares concepto–explicación.


## Enlaces internos (anclas)

En documentos largos podemos querer saltar a puntos concretos de la misma página.  
Para ello usamos el atributo `id` y enlaces que apunten a ese `id`.

**Definir el destino:**

    <h2 id="seccion1">Sección 1</h2>

**Enlace dentro de la misma página:**

    <a href="#seccion1" title="Sección 1">Ir a la sección 1</a>

**Enlace desde otro documento:**

    <a href="secciones.html#seccion1" title="Sección 1">Ir a la sección 1</a>

# Comentario: `id` marca el punto de destino y `href="#id"` o `href="archivo.html#id"` crea el enlace hacia esa ancla.


## Contenedores `<div>`

`<div>` es un contenedor de tipo bloque que se utiliza para agrupar otros elementos.

**Usos principales:**

- Dividir la página en secciones.
- Aplicar estilos CSS a bloques concretos.
- Manipular partes específicas con JavaScript.

**Ejemplo:**

    <div class="contenido">
        <h2>Título de sección</h2>
        <p>Texto dentro del contenedor.</p>
    </div>

# Comentario: `<div>` sirve para maquetar y agrupar, pero no indica por sí mismo el significado del contenido.


## Rutas absolutas y relativas

Cuando enlazamos a otros archivos (HTML, CSS, imágenes, etc.) necesitamos indicar su ubicación.

### Ruta absoluta

Incluye la dirección completa con dominio.

    <img src="https://www.ejemplo.com/images/logo.png" alt="Logo Example">

### Ruta relativa

Se define en función de la ubicación del archivo actual.

Estructura de ejemplo:

    /mi-sitio/
        index.html
        /images/
            logo.png

Uso en `index.html`:

    <img src="images/logo.png" alt="Logo de mi sitio">

# Comentario: Las rutas relativas son recomendables dentro del mismo proyecto porque no dependen del dominio.


## Imágenes en HTML

Las imágenes son muy utilizadas para hacer más visual y atractiva una página web.

La etiqueta para insertar imágenes es `<img>`, que es un elemento en línea y vacío.

**Sintaxis básica:**

    <img src="media/logo.png" alt="Logo de la web" />

- `src`: ruta (absoluta o relativa) de la imagen.
- `alt`: texto alternativo que se muestra si la imagen no carga y que usan los lectores de pantalla.

# Comentario: Siempre se debe usar `alt` por accesibilidad, SEO y buenas prácticas.

## Elementos semánticos en HTML5

HTML semántico significa usar etiquetas que describen el tipo de contenido que encierran, facilitando la comprensión para personas y navegadores.

- `<header>`: cabecera de la página o sección.
- `<footer>`: pie de página o sección.
- `<nav>`: zona de navegación con enlaces principales.
- `<section>`: sección genérica de contenido relacionado.
- `<article>`: contenido independiente (post, noticia, etc.).
- `<aside>`: contenido relacionado pero secundario (barra lateral).
- `<main>`: contenido principal del documento.
- `<figure>` y `<figcaption>`: imágenes/medios con su pie.

# Comentario: Usar estas etiquetas en lugar de solo `<div>` da significado al contenido, mejora accesibilidad y SEO.


## Etiquetas de formularios: `<form>`

La etiqueta `<form>` crea un formulario para enviar datos a un servidor o realizar acciones.

Atributos comunes:

- `action`: URL a la que se envían los datos.

      <form action="procesar.php">

- `method`: método de envío (`get` o `post`).

      <form action="procesar.php" method="post">

- `enctype`: cómo se codifican los datos. Ejemplo para subir archivos:

      <form action="subir.php" method="post" enctype="multipart/form-data">

- `target`: dónde se muestra la respuesta.

  - `_self`: (por defecto) misma pestaña.
  - `_blank`: nueva pestaña/ventana.

# Comentario: `<form>` es el contenedor de todos los campos del formulario.


## Etiquetas de formularios: `<input>`

`<input>` crea campos interactivos. Es un elemento vacío (sin cierre separado).

Atributos comunes:

- `type`: define el tipo de campo.

      <input type="text">
      <input type="password">
      <input type="email">
      <input type="number">
      <input type="file">
      <input type="checkbox">
      <input type="radio">
      <input type="date">
      <input type="submit">
      <input type="reset">
      <input type="url">

- `id`: identificador único, útil para asociar `<label>`.

      <input id="nombre">

- `name`: nombre del campo (clave que recibe el servidor).

      <input name="nombre">

- `value`: valor inicial del campo.

- `placeholder`: texto de ayuda cuando el campo está vacío.

- `required`: campo obligatorio.

- `disabled`: desactiva el campo.

- `readonly`: solo lectura (no editable).

# Comentario: `name` es clave para el envío de datos; sin `name`, ese input no viaja al servidor.


## Input type radio y checkbox

### `type="radio"`

Botones de opción, permiten elegir **solo una** opción dentro de un grupo (mismo `name`).

```html
<form>
    <p>Elige tu género musical favorito:</p>
    <label><input type="radio" name="genero" value="rock" checked> Rock</label>
    <label><input type="radio" name="genero" value="pop"> Pop</label>
    <label><input type="radio" name="genero" value="jazz"> Jazz</label>
    <button type="submit">Enviar</button>
</form>

