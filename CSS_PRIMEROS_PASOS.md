### CSS (Cascading Style Sheets) (🎨)
CSS es un lenguaje de estilo utilizado para dar estilo y diseñar páginas web. Permite controlar la apariencia y presentación de los elementos HTML en un documento. Con CSS, puedes definir colores, tipografías, márgenes, tamaños, diseños y más.

### Selectores (🎯)
Los selectores en CSS se utilizan para seleccionar elementos HTML a los que se les aplicarán los estilos. Puedes seleccionar elementos por su etiqueta, clase, ID o atributos. Aquí tienes algunos ejemplos de selectores:

- Selector de etiqueta: `p` selecciona todos los párrafos en el documento.
- Selector de clase: `.clase` selecciona todos los elementos con la clase "clase".
- Selector de ID: `#id` selecciona el elemento con el ID "id".

```css
/* Ejemplo de selectores CSS */
p {
  color: blue;
}

.clase {
  font-size: 16px;
}

#id {
  background-color: yellow;
}
```

### Propiedades y valores (🎨)
Las propiedades en CSS especifican qué aspecto se aplicará a un elemento seleccionado, y los valores determinan cómo se verá ese aspecto. Aquí tienes algunos ejemplos de propiedades y valores:

- `color`: define el color del texto.
- `font-size`: establece el tamaño de la fuente.
- `background-color`: define el color de fondo.

```css
/* Ejemplo de propiedades y valores CSS */
p {
  color: blue;
  font-size: 18px;
}

.clase {
  background-color: yellow;
}
```

### Reglas CSS (⚖️)
Las reglas CSS se componen de un selector y un bloque de declaración. El bloque de declaración contiene una o más propiedades y sus valores asociados. Aquí tienes un ejemplo de una regla CSS:

```css
/* Ejemplo de regla CSS */
selector {
  propiedad1: valor1;
  propiedad2: valor2;
}
```

### Modelo de caja (📦)
El modelo de caja en CSS describe cómo se representa visualmente un elemento HTML. Cada elemento tiene un contenido, un relleno, un borde y márgenes. Puedes controlar estos aspectos utilizando propiedades como `width`, `height`, `padding`, `border`, `margin`, entre otras.

```css
/* Ejemplo del modelo de caja CSS */
.elemento {
  width: 200px;
  height: 100px;
  padding: 10px;
  border: 1px solid black;
  margin: 20px;
}
```

### Selectores de pseudo-clases y pseudo-elementos (🎯)
CSS también ofrece selectores de pseudo-clases y pseudo-elementos para aplicar estilos a elementos en estados específicos o partes específicas de un elemento. Algunos ejemplos comunes incluyen `:hover`, `:active`, `:first-child` y `::before`.

```css
/* Ejemplo de selectores de pseudo-clases y pseudo-elementos CSS */
a:hover {
  color: red;
}

p:first-child {
  font-weight: bold;
}

p::before {
  content: "Antes de: ";
}
```
