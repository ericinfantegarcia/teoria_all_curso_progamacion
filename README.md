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




