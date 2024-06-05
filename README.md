#### Emmanuel Torres Malena | 2021-1097


### Type selector

```css
div {
    color: red solid;
}
```
- Descripcion: Selecciona todos los ```<div>``` y les pone color rojo a las letras.
- Applicacion: Estiliza todos los elementos ```div``` dentro de un documento HTML.

---
 ### Id selector

```css
#cool {
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
.epic {s <a>
    border: 5px blue;
}
```

- Descripcion: Selecciona todos los elementos que tengan la clase **epic**, y les pone un borde de 5px de color azul.
- Aplicacion: Selecciona todos los elementos que tengan esa clase. Un elemento puede tener un solo id, pero multiples clases.

---

### Combined selectors

```css
div.shift {
    display: grid;
}
```

- Descripcion: Selecciona todos los elementos que esten dentro de un ```<div>```, y que tengan la clase **shift**; y les cambia el display de block a grid.
- Aplicacion: Sirve para combinar los class selectors con otros tipos de selectors.

---

### Comma Combinator

```css
div, span, .shift {
    background-color: green;
}
```

- Descripcion: Selecciona a los ```<div>```, ```<span>```, y los elementos que tengan la clase **shift**; y les pone el fondo de color verde.
- Aplicacion: Sirve para seleccionar multiples elementos y agregarles las mismas reglas css.

---

### Universal Selector

```css
* {
    font-family: sans-serif;
}
```
- Descripcion: Selecciona todos los elementos del documento, y le cambia la fuente de texto a sans-serif
- Aplication: Sirve para seleccionar todos los elementos de un documento HTML.

Este operador se puede combinar con otros selectores, por ejemplo:

```css
div * {
    font-family: sans-serif;
}
```

- Descripcion: Selecciona todos los elementos dentro de un div, y la cambia la fuente de texto a sans-serif.

---

### Adjacent Sibling Selector

```css
plate + apple {
    margin: 50px;
    padding: 20px;
}
```

- Descripcion: Selecciona el primer elemento ```apple``` que esta despues de un elemento ```plate```, y le aplica un margin de 50px y un padding de 20px.
- Aplicacion: Sirve para seleccionar elemento que esta directamente despues de otro elemento; y selecciona unicamente uno.

---

### General Sibling Selector

```css
plate ~ pickle {
    display: none;
}
```

- Descripcion: Selecciona todos los ```pickle``` que estan despues de un ```bento```, y les cambia el display a none para que se oculten.
- Aplicacion: Sirve para seleccionar los elementos que estan despues de otro elemento; este selecciona a todos.

---
 
### Child Selector

```css
div > ul {
	text-decoration: none;
}
```

- Descripción: A cualquier elemento ```<ul>```, que sea hijo directo de un ```<div>```, se le eliminará cualquier decoración de texto.
- Aplicación: Se utiliza para seleccionar elementos que son hijos directos de un elemento padre específico. Se representa con el símbolo **``>``**

---

### First Child Pseudo-Selector

```css
orange:first-child {
    color: blue;
}
```

- Descripción: Selecciona cualquier elemento ``<orange>`` que sea el primer hijo de su elemento padre, y le aplica el color azul.
- Aplicación: Se utiliza cuando se desea aplicar estilos específicos exclusivamente al primer hijo de un elemento contenedor. Para usarlo debemos utilizar **`:first-child`**

---
### Only Child Pseudo-Selector

```css
pickle:only-child {
    color: green;
}
```

- Descripción: Selecciona cualquier elemento ``<pickle>`` que sea el único hijo de su elemento padre, y le aplica el color verde.
- Aplicación: Se utiliza cuando se desea aplicar estilos específicos exclusivamente un elemento que sea el único hijo de un elemento contenedor. Es práctico usarlo en situaciones en la que se quiere destacar un elemento único de un contenedor, y aplicarle estilos solamente si no tiene hermanos. Para usarlo debemos utilizar **`:only-child`**

---

### Nth Child Pseudo-Selector

```css
plate:nth-child(3) {
    display: none;
}
```

- Descripción: Selecciona el tercer elemento ``<plate>`` de cada contenedor padre. y le cambia el display a none .
- Aplicación: Se utiliza para aplicar estilos basados en la posición de los elementos dentro de su padre. Para usarlo debemos utilizar **`:nth-child(n)`**

---

### Nth Last Pseudo-Selector

```css
li:nth-last-child(3) {
    margin: 200px;
    padding: 20px;
    border: 5px red solid;
}
```

- Descripción: Selecciona, desde el final hacia arriba, el tercer elemento ``<bento>`` dentro de cada contenedor padre. y le agrega un margin de 200px, un padding de 20px y un border de 5px solido de color rojo .
- Aplicación: Se utiliza para seleccionar uno o más elementos basándose en su posición desde el final de su elemento padre. Para usarlo debemos utilizar **`:nth-last-child(n)`**

---

### First of Type Selector

```css
p:first-of-type {
    font-size: 20px;
    color: darkgreen;
}
```


- Descripción: Selecciona el primer elemento ``<p>`` dentro de cada contenedor padre, y le cambia el tamaño de fuente a 20px y le pone de color verde oscuro
- Aplicación: Se utiliza para aplicar estilos específicos al primer elemento de un tipo particular dentro de su contenedor padre. Para usarlo debemos utilizar **`:first-of-type`**. Un buen uso para este puede ser para destacar el primer parrafo o encabezado dentro de una sección o artículo.

---

### Nth of Type Selector

```css
tr:nth-of-type(odd) {
    background-color: lightblue;
}
```


- Descripción: Selecciona, todos los elementos ``<tr>`` que estén en posiciones impares, y le aplica un color de fonda azul claro.
- Aplicación: Se utiliza para seleccionar uno o más elementos basándose en su posición dentro de su grupo de hermanos del mismo tipo (el mismo tipo de etiqueta). Para usarlo debemos utilizar **`:nth-of-type(n)`**

---

### Nth of Type with Formula Selector

```css
p:nth-of-type(3n+1) {
    color: purple;
    font-weight: bold;
}
```


- Descripción: Selecciona, cada tercer ``<p>`` comenzando desde el primero (una secuencia: 1, 4, 7, ...), y le aplica un color morado y la pone en negrita.
- Aplicación: Al agregar formulas al **`:nth-of-type(n)`** podemos aplicar estilos a elementos basados en patrones regulares.  Para usarlo debemos utilizar **`:nth-of-type(an+b)`**, donde **a** define el paso de iteración (cada **a** elementos), y la **b** define el punto de inicio. 

---

### Only of Type Selector
```css
p:only-of-type {
    font-style: italic;
}
```


- Descripción: Selecciona el único elemento ``<p>`` dentro de cada contenedor padre y le aplica estilo cursivo
- Aplicación: Se utiliza para seleccionar un elemento que es el único de su tipo dentro de su elemento padre. Para usarlo debemos utilizar **`:only-of-type`**

---

### Last of Type Selector
```css
div:last-of-type {
    border: 1px solid red;
}
```


- Descripción: Selecciona el ultimo ``<div>`` dentro de cada contenedor padre y le aplica un borde rojo de 1px.
- Aplicación:  Se utiliza cuando se desea aplicar estilos al último elemento de su tipo dentro de su contenedor padre. Para usarlo debemos utilizar **`:last-of-type`**


---

### Empty Selector

```css
div:empty {
    background-color: lightgray;
}
```


- Descripción: Selecciona los ``<div>`` que están vacíos (sin contenido dentro de ellos), y les aplica un fondo gris claro. Todos los demás ``<div>`` que si tengan contenido no van a ser afectados.
- Aplicación: Se utiliza para seleccionar elementos que no tienen contenido, es decir, están vacíos, Para usarlo debemos utilizar **`:empty`**

---

### Not(x)

```css
p:not(.special) {
    color: blue;
}
```


- Descripción: Selecciona todos los elementos `<p>` que no tienen la clase **.especial**, y les aplica un color azul.
- Aplicación: Se utiliza para seleccionar elementos que no coinciden con el selector **`x`** .  Para usarlo debemos utilizar **`:not(x)`**

---
### Attribute Selector

 Aplicación: son utilizados para seleccionar elementos HTML basados en los atributos y los valores de esos atributos. Hay varias formas de utilizar estos selectores:

##### Normal

```css
input[type="text"] {
    background-color: lightgray;
}
```


- Descripción: Este selector aplica un fondo gris claro a todos los elementos ``<input>`` que tengan un atributo **type** con el valor *text*

##### Attribute Value Selector

```css
a[href*="postgresql.org"] {
    color: blue;
}
```


- Descripción: Este selector aplica un color azul a todos los``<a>`` cuyo atributo **href** sea el string *"postgresql.org"*.

##### Attribute Starts With Selector

```css
a[href^="https://"] {
    color: green;
}
```


- Descripción: Este selector aplica un color verde a todos los ``<a>`` cuyo atributo **href** comience con *"https://"*. Para indicar este selector se utiliza el símbolo **`^`**

##### Attribute Ends With Selector

```css
a[href^="https://"] {
    color: green;
}
```


- Descripción: Este selector aplica un color rojo a todos los ``<a>`` cuyo atributo **href** termine con  *".pdf"*. Para indicar este selector se utiliza el símbolo **`$`**

##### Attribute Wildcard Selector

```css
input[type~="password"] {
    border: 1px solid black;
}
```


- Descripción: Este selector aplica un borde de 1px sólido negro a todos los elementos `<input>` cuyo atributo **type** contiene la palabra *"password"* como una palabra completa. Para indicar este selector se utiliza el símbolo **`~`**





