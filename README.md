# css-selectors
##### Emmanuel Torres Malena | 2021-1097


### Type selector

```css
div {
    color: red solid;
}
```
- Descripcion: Selecciona todos los ```<div>``` y les pone color rojo a las letras.
- Aplicacion: Estiliza todos los elementos ```div``` dentro de un documento HTML.

---
 ### Id selector

```css
#cool{
    padding: 25px;
}
```

- Descripcion: Selecciona el elemento que tiene el id **cool** y le agrega un padding de 25px.
- Aplicacion: Estiliza el elemento que tenga ese id especifico.
  
---

### Descendant Selector

```css
div p {
    text-align: center;
}
```

- Description: Selecciona los elementos ```<p>``` que esten dentro de un elemento ```<div>```, y posiciona el texto en el centro.
- Aplicacion: sirve para seleccionar un elemento que este dentro de otro. Se puede utilizar con class selectors, id selectors, etc.

---

### Class selectors

```css
.epic {
    border: 5px blue;
}
```

- Desciption: Selecciona todos los elementos que tengan la clase **epic**, y les pone un borde de 5px de color azul.
- Aplicacion: Selecciona todos los elementos que tengan esa clase. Un elemento puede tener un solo id, pero multiples clases.

---

### Combined selectors

```css
div.shift {
    display: grid;
}
```

- Description: Selecciona todos los elementos que esten dentro de un ```<div>```, y que tengan la clase **shift**; y les cambia el display de block a grid.
- Aplicacion: Sirve para combinar los class selectors con otros tipos de selectors.

---

### Comma Combinator

```css
div, span, .shift {
    background-color: green;
}
```

- Description: Selecciona a los ```<div>```, ```<span>```, y los elementos que tengan la clase **shift**; y les pone el fondo de color verde.
- Aplicacion: Sirve para seleccionar multiples elementos y agregarles las mismas reglas css.

---

### Universal Selector

```css
* {
    font-family: sans-serif;
}
```
- Description: Selecciona todos los elementos del documento, y le cambia la fuente de texto a sans-serif
- Aplicaion: Sirve para seleccionar todos los elementos de un documento HTML.

---

###

