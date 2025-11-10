# Teoría Markdown

<!-- Documento resumen con la teoría básica de Markdown:
     archivos, encabezados, estilos de texto, listas, código,
     enlaces, imágenes, tablas, notas al pie y listas de verificación. -->

## Archivos Markdown

Podemos crear un archivo de texto plano con diferentes extensiones para archivos de Markdown dependiendo del destino del archivo:

- `.markdown`
- `.md`
- `.mkd`
- `.mkdown`
- `.text`
- `.mdown`

GitHub utiliza principalmente la extensión `.md` para los archivos, por ejemplo `README.md`.

<!-- Explicación: estas son las extensiones habituales de archivos Markdown.
     En GitHub casi siempre veremos `.md`. -->

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

<!-- Explicación: el número de almohadillas indica el nivel del título.
     # es el más importante (H1) y ###### el menos importante (H6). -->

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

<!-- Explicación: con estos símbolos añadimos formato al texto.
     Se pueden combinar para usar negrita y cursiva al mismo tiempo. -->


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

<!-- Explicación: `*`, `-` o `+` crean listas con viñetas.
     La sangría (tabulador o espacios) crea sublistas dentro de otra lista. -->

### Párrafos

Para crear un nuevo párrafo se deja una línea en blanco entre bloques de texto.

Ejemplo:

    Este es el primer párrafo.

    Este es el segundo párrafo.

<!-- Explicación: si no dejamos línea en blanco, Markdown lo interpreta como un mismo párrafo. -->

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

<!-- Explicación:
     - Los backticks (`) se usan para marcar código.
     - Con tres backticks creamos bloques de código.
     - Podemos indicar el lenguaje (html, javascript, etc.) tras los tres backticks. -->

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

<!-- Explicación:
     - La sintaxis de imagen es igual que la de enlace, pero con `!` delante.
     - El texto alternativo describe la imagen y mejora la accesibilidad. -->

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

<!-- Explicación: las tablas se construyen con `|` y `-`.
     Los dos puntos controlan la alineación de cada columna. -->

### Notas al pie de página

Ejemplo:

    Texto con nota al pie[^1]

    [^1]: Aquí encuentras el texto de la nota al pie.

<!-- Explicación:
     - `[^1]` es la referencia en el texto.
     - `[^1]:` define el contenido de la nota al pie. -->

### Listas de verificación

Ejemplo de checklist:

    - [ ] A
    - [x] B
    - [ ] C

- `[ ]` crea una casilla vacía.
- `[x]` crea una casilla marcada.
- Es importante dejar un espacio en blanco entre los corchetes en las casillas vacías.

<!-- Explicación:
     Muy usado en GitHub para listas de tareas y seguimiento de trabajo. -->

     
