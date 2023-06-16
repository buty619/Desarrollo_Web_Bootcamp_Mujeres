### Unidades de medida en CSS (📏)
Las unidades de medida en CSS se utilizan para especificar tamaños y dimensiones de elementos. Algunas de las unidades de medida más comunes son:

- `px` (píxel): Unidad de medida basada en píxeles, que representa un punto en una pantalla.
- `%` (porcentaje): Unidad de medida relativa al tamaño del elemento padre.
- `em`: Unidad de medida relativa al tamaño de la fuente del elemento.
- `rem`: Unidad de medida relativa al tamaño de la fuente del elemento raíz (generalmente el `<html>`).
- `vh` (viewport height): Unidad de medida relativa al porcentaje del alto de la ventana del navegador.
- `vw` (viewport width): Unidad de medida relativa al porcentaje del ancho de la ventana del navegador.

Aquí tienes un ejemplo de cómo se utilizan algunas unidades de medida en CSS:

```css
/* Ejemplo de unidades de medida en CSS */
div {
  width: 300px;
  font-size: 16px;
  padding: 1em;
  margin-bottom: 5vh;
}
```

### Media Queries (📱)
Las media queries en CSS permiten aplicar estilos específicos a diferentes dispositivos o condiciones de visualización. Se utilizan para crear diseños responsivos y adaptar la apariencia de un sitio web según el tamaño de la pantalla o las características del dispositivo.

Las media queries se definen utilizando el `@media` rule y se especifica una condición mediante una expresión de consulta. Aquí tienes un ejemplo de una media query que se aplica cuando el ancho de la pantalla es menor o igual a 600px:

```css
/* Ejemplo de media query en CSS */
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }

  h1 {
    color: red;
  }
}
```

En este ejemplo, los estilos dentro de la media query se aplicarán solo cuando el ancho de la pantalla sea menor o igual a 600px. En este caso, el fondo del `body` se cambiará a un color azul claro y el color del `h1` se cambiará a rojo.

Las media queries permiten crear diseños adaptables y optimizados para diferentes dispositivos, como teléfonos móviles, tabletas y computadoras de escritorio.
