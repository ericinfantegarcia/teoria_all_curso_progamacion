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


