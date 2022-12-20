> # Indice
> 1. Introduccion a HTML
> 2. Estructura de HTML
> 3. Formas de modificar el texto
> 4. Crear listas
> 5. Crear tablas
> 6. Multimedia (Fotos y videos)
> 7. Formularios y botones
> # Notas extras
> 1. Cual es la diferencia entre input(submit) y button

> # 1. Introduccion a HTML
- **DOCTYPE:** Indica la version de html.
- **lang:** Sirve para indicar que lenguaje se esta trabajando.
- **meta:** Sirve para agregar metadatos del documentos, como el titulo, el estilo, el tipo de codificacion, entre otros.
- **title:** Titulo en la pestaña del navegador.
- **link:** Enlaza archivos CSS
- **Style:** Se usa unicamente en caso de querer escribir CSS dentro de nuestro codigo HTML
- **script:** Enlaza o escribe JavaScript en el documento HTML
- **body:** Elementos visibles en nuestra pagina
```jsx
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Documento de prueba</title>
</head>
<body>
    
</body>
</html>
```
> # 2. Estructura de HTML
- **Div:** Contenedor general
- **Header:** Es el encabezado de una página web, el cual contiene información básica sobre el sitio web, tales como el nombre del sitio, un logotipo, un tema o menú de navegación, etc.
- **Main:** Etiqueta para contenido principal
- **nav:** Nav es la propiedad que usamos para insertar la barra de navegacion.
- **Seccion:** Una sección es una etiqueta HTML que se utiliza para agrupar contenido relacionado. Puede contener cualquier elemento HTML, como párrafos, enlaces, imágenes, encabezados, listas, tablas, etc.
- **article:** Es un elemento HTML que sirve para indicar que una sección de un documento es un artículo, el cual generalmente consiste en contenido autónomo, como una noticia o una reseña.
- **aside:** Este contenido normalmente se usa para representar contenido relacionado con el contenido principal, como contenido secundario, entradas de blog, un lado lateral con enlaces, publicidad, etc.
- **Footer:** Se utiliza para definir un espacio al final de una página web para contener información acerca del sitio web, como enlaces a la página de inicio, información sobre derechos de autor, términos y condiciones, etc.
```html
    <header></header>
    <nav></nav>
    <section></section>
    <article></article>
    <aside></aside>
    <footer></footer>
```


> # 3. Para el texto
```html
    <!--Codigo para modificar el texto del codigo-->
    <p>Nos ayuda a crear parrafos</p>
    <!--Titulos-->
    <h1></h1>
    <h2></h2>
    <h3></h3>
    <h4></h4>
    <h5></h5>
    <h6></h6>
    <!--Texto en negritas-->
    <b>Texto de prueba</b>
    <!--Texto en cursiva-->
    <i>Texto de prueba</i>
    <!--Texto subrayado-->
    <u>Texto de prueba</u>
    <!--Crear un enlace-->
    <a href="https://mail.google.com/mail/u/0/#inbox">Gmail</a>
    <!--Texto en negritas-->
    <strong>Texto en negritas</strong>
    <!--Texto en formato de cita-->
    <blockquote>Texto de prueba</blockquote>
    <!--Crea un salto de linea-->
    <br>
```

> # 4. Crear listas
- Lista desordenada
```html
<!--Crearemos una lista desordenada-->
    <ul>
        <li>Primer atributo</li>
        <li>Segundo atributo</li>
        <li>Tercer atributo</li>
    </ul>
```
- Lista ordenada
```html
    <ol>
        <li>Primer atributo</li>
        <li>Segundo atributo</li>
        <li>Tercer atributo</li>
    </ol>
```

> # 5. Crear tablas
- table: Crea una tabla  
- tr: Crea las filas  
- td: Crea las columnas  
- th: Crea el titulo de cada columna  
- col: Especifica las propiedades de las columnas
```html
<table>
        <tr>
          <th>Nombre</th>
          <th>Apellido</th>
        </tr>
        <tr>
          <td>Juan</td>
          <td>Pérez</td>
        </tr>
        <tr>
          <td>Ana</td>
          <td>Gómez</td>
        </tr>
      </table>
```
> # 6. Multimedia
> Paginas para mejorar nuestras imagenes
> 1. Tiny PNG: Te comprime las imagenes
> 2. Verefix: Retira metadatos de las imagenes
> 3. Pexels: Pagina para descargar imagenes
- Insertar una imagen
```html
<img src="direccion_de_la_imagen" alt="Texto alternativo">
```
- Insertar video
- **video:** Inserta un video
- **control:** Sirve para proporcionarle a nuestro video los controles para poder controlarlo como el tamaño de la pantalla, play, pause etc.
- **preload:** Nos sirve para que el video empiece a cargar en el momento en el que el usuario habra la web.
- **source:** La etiqueta source se puede colocar dentro de una etiqueta varias veces para poder especificar diferentes rutas.
```html
<section>
        <video src="" controls preload="auto"></video>
</section>
```
> # 7. Formularios y botones
- **form:** Crea un formulario
- **input:** Campo para introducir datos
- **Type:** Typo de input
- **label:** El titulo del input
- **Textarea:** Campo para introducir mucho teto
- **Button:** Para crear un boton 
```html
<form action="" method="post">
        <label for="name">Name:</label>
        <input type="number" id="name" name="name">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <input type="submit" value="Submit">
</form>
```
> - Autocompletar y require en formularios
- **placeholder:** Es el valor que quieres que tenga nuestro input
- **span:** Es el nombre que tendra nuestro formulario
- **autocomplete:** Es la propiedad que dejara guardar valores
- **require:** No dejara avanzar si este campo no se responde
```html
<form action="">
        <label for="nombre">
            <span>Cual es tu nombre</span>
            <input type="text" name="nombre" 
            id="nombre" autocomplete="name" required placeholder="Tu nombre">
        </label>
</form>
```


- Insertar botones
```html
<button>Click</button>
```
> # 8. Etiquetas con propiedades
```html
<!--No tiene ningún efecto en la estructura de la página web, pero se utiliza a menudo para darle estilo visual a determinados elementos.-->
<span></span>
```


> # Notas Extras
#### 1. Cual es la diferencia entre un input, submit y button.
- **Input:** Se utiliza para recibir datos del usuario contraseñas, usuario etc.
- **Submit:** Se utiliza para enviar formularios a la pagina de destino.
- **Button:** Se utilizan para iniciar una accion, como enviar un formulario, cambiar de pagina, entre otros.











