### El DOM (🌐)

El DOM es una representación en memoria de un documento HTML que permite a los programas acceder y manipular su contenido, estructura y estilo. Es una interfaz de programación para documentos HTML y XHTML. Básicamente, el DOM crea una estructura en forma de árbol de todos los elementos y nodos del documento.

### Anatomía de un documento HTML (📄)

Un documento HTML consta de varias partes, y cada una de ellas cumple una función específica. Aquí están las partes principales de la anatomía de un documento HTML:

1. Doctype (📜): La primera línea de un documento HTML es el Doctype, que declara el tipo de documento y su versión. Por ejemplo:
   
   ```html
   <!DOCTYPE html>
   ```

2. Etiqueta `<html>` (🌐): La etiqueta `<html>` es el elemento raíz del documento HTML. Todo el contenido del documento se encuentra dentro de esta etiqueta. Por ejemplo:

   ```html
   <!DOCTYPE html>
   <html>
     ...
   </html>
   ```

3. Etiqueta `<head>` (📋): La etiqueta `<head>` contiene información meta y enlaces a archivos externos, como hojas de estilo CSS y scripts JavaScript. No se muestra en el navegador. Por ejemplo:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <meta charset="UTF-8">
       <title>Título de la página</title>
       <link rel="stylesheet" href="estilos.css">
     </head>
     ...
   </html>
   ```

4. Etiqueta `<body>` (💡): La etiqueta `<body>` contiene el contenido visible del documento, como texto, imágenes, enlaces y elementos interactivos. Todo lo que se muestra en el navegador va dentro de esta etiqueta. Por ejemplo:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       ...
     </head>
     <body>
       <h1>Título de la página</h1>
       <p>¡Hola, mundo!</p>
       <img src="imagen.jpg" alt="Imagen">
       <a href="https://www.ejemplo.com">Enlace</a>
     </body>
   </html>
   ```

5. Etiqueta `<script>` (📜): La etiqueta `<script>` se utiliza para incluir scripts JavaScript en el documento. Puede ir tanto en la sección `<head>` como en la sección `<body>`. Por ejemplo:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       ...
       <script src="script.js"></script>
     </head>
     <body>
       ...
       <script>
         alert('¡Hola, mundo!');
       </script>
     </body>
   </html>
   ```

Estas son las partes principales que conforman la anatomía de un documento HTML. El DOM permite acceder y manipular estos elementos y nodos utilizando código JavaScript.
