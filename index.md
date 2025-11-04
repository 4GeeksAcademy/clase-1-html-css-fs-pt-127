# HTML Hello

## ¿Qué hacer a continuación?

Crea un archivo `index.html` con [la estructura básica de HTML](https://4geeks.com/es/lesson/what-is-html-learn-html-es#estructura-de-pgina) y ve el resultado en vivo corriendo un servidor web utilizando el siguiente comando:

```bash
$ pip3 install flask && python3 server.py
```

```bash
npm install -g http-server
```

# HTML Y CSS

✅ Estructura básica de HTML

- [ ] ¿Qué es HTML?
      HTML (HyperText Markup Language) es el lenguaje estándar para crear páginas web que conformaria el esqueleto.
      No es un lenguaje de programación es un lenguaje de etiquetas
- [ ] Estructura básica de un documento HTML:
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>Título de la página</title>
    </head>
    <body>
      <!-- Contenido aquí -->
    </body>
  </html>
  ```

## ✅ Etiquetas principales de HTML

- [ ] `<html>`: Define el inicio y fin del documento HTML.
- [ ] `<head>`: Contiene metadatos, enlaces a CSS, título, etc.
- [ ] `<title>`: Título que aparece en la pestaña del navegador.
- [ ] `<body>`: Todo el contenido visible de la página.
- [ ] `<h1>` a `<h6>`: Encabezados de diferentes niveles.
- [ ] `<p>`: Párrafos de texto.
- [ ] `<a>`: Enlaces.
- [ ] `<img>`: Imágenes.
- [ ] `<ul>`, `<ol>`, `<li>`: Listas.
- [ ] `<div>` y `<span>`: Contenedores genéricos.

## ✅ Atributos básicos de HTML

- [ ] `id`: Identificador único para un elemento.
- [ ] `class`: Clase para agrupar elementos y aplicar estilos.
- [ ] `src`: Fuente de una imagen o archivo.
- [ ] `href`: Dirección de un enlace.
- [ ] `alt`: Texto alternativo para imágenes.
- [ ] `style`: Permite agregar estilos CSS directamente.

## Podemos ver informacion en:

[MDN](https://developer.mozilla.org/es/docs/Web/HTML/Reference/Elements) o [W3SCHOOL](https://w3schoolsua.github.io/tags/tag_del_es.html#gsc.tab=0)

## ✅ ¿Qué es CSS?

- [ ] CSS (Cascading Style Sheets) es el lenguaje para definir el estilo visual de las páginas web.
- [ ] Se puede escribir en un archivo externo (`.css`), en la etiqueta `<style>` dentro del `<head>`, o directamente en el atributo `style` de un elemento HTML.

## ✅ Selectores en CSS

Los selectores es la forma en la que decimos a qué elementos del HTML se les aplican los estilos.

- [ ] Selector de etiqueta:
  ```css
  p {
    color: blue;
  }
  ```
- [ ] Selector de clase:
  ```css
  .mi-clase {
    font-size: 20px;
  }
  ```
- [ ] Selector de id:
  ```css
  #mi-id {
    background: yellow;
  }
  ```
- [ ] Selector universal:

  ```css
  * {
    margin: 0;
  }
  ```

**Jerarquía de aplicación de estilos en CSS:**

1.  Estilos del navegador (por defecto). Ej.El botón tiene un estilo predeterminado (color, borde, fuente) definido por el navegador, aunque no se haya especificado CSS. <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

2.  Estilos externos o heredados. Ej.Estilos heredados de los componentes padres <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

3. Selectores por etiqueta (`p`, `div`, `span`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
     <span style="font-size: 2em;">↓</span>
   </div>

4. Selectores por clase (`.clase`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

5. Selectores por atributo (`[type="text"]`, `[disabled]`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

6. Selectores por pseudo-clase (`:hover`, `:focus`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

7. Selectores por ID (`#identificador`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

8. Estilos en línea (`style="..."`) <br>

<div style="display: flex; justify-content: center; align-items: center; height: 30px; margin: 10px;">
  <span style="font-size: 2em;">↓</span>
</div>

9. `!important` ← 🔥 fuerza máxima (rompe la jerarquía normal)

## ✅ Estilos principales en CSS

- [ ] `color`: Color del texto.
- [ ] `background-color`: Color de fondo.
- [ ] `font-size`: Tamaño de la fuente.
- [ ] `margin`: Espacio exterior del elemento.
- [ ] `padding`: Espacio interior del elemento.
- [ ] `border`: Borde del elemento.
- [ ] `width` y `height`: Ancho y alto.
- [ ] `display`: Tipo de visualización (block, inline, flex, etc).

---

## ✅ Ejemplo de uso de CSS

```css
body {
  background-color: #f0f0f0;
  color: #333;
}

h1 {
  font-size: 2em;
  text-align: center;
}

.mi-clase {
  padding: 10px;
  border: 1px solid #ccc;
}
```

## ✅ Seudoclases en CSS

Las seudoclases son palabras clave que se añaden a los selectores (precedidas por :) para definir un estado especial de un elemento.
No se aplican por clase o ID, sino por el estado o la interacción del usuario con el elemento.

Por ejemplo:

```css
button:hover {
  background-color: blue;
}
```

Interacción del usuario

- [ ] :hover → cuando el cursor está sobre el elemento

- [ ] :active → cuando el elemento está siendo presionado (clic en progreso)

- [ ] :focus → cuando el elemento recibe el foco (ej. input activo)

- [ ] :focus-visible → cuando el foco es visible (ej. con teclado, no con clic)

- [ ] :visited → cuando un enlace ya fue visitado

- [ ] :link → para enlaces que aún no han sido visitados

🧱 Estructura y posición

- [ ] :first-child → selecciona el primer hijo de su padre

- [ ] :last-child → selecciona el último hijo de su padre

- [ ] :nth-child(n) → selecciona el hijo número n

- [ ] :nth-of-type(n) → selecciona el n-ésimo elemento de un tipo concreto (ej. p, li)

- [ ] :not(selector) → excluye elementos que coinciden con un selector

- [ ] :empty → selecciona elementos sin contenido (ni texto ni hijos)

- [ ] :only-child → selecciona elementos que son el único hijo de su padre

🧩 Formularios y validación

- [ ] :checked → selecciona inputs marcados (checkbox, radio)

- [ ] :disabled → elementos desactivados

- [ ] :enabled → elementos activados

- [ ] :required → campos obligatorios

- [ ] :optional → campos opcionales

- [ ] :valid → campos con datos válidos según la validación

- [ ] :invalid → campos con datos no válidos

## ✅ Tipos de display en CSS

El display define cómo se comporta un elemento en el flujo del documento y cómo se relaciona con los demás.

### 🏗️ 1. display: block

👉 Ocupa todo el ancho disponible y comienza en una nueva línea.

📘 Ejemplo:

```html
<div style="display: block; background: green;">Bloque 1</div>
<div style="display: block; background: blue;">Bloque 2</div>
```

🔹 Resultado:

Cada div aparece en una línea distinta.

<div style="display: block; background: green;">Bloque 1</div>
<div style="display: block; background: blue;">Bloque 2</div>

Ocupa todo el ancho del contenedor, aunque su contenido sea pequeño.

🧱 Ejemplos de elementos que ya son block por defecto:

- [ ] `<div>`

- [ ] `<p>`

- [ ] `<section>`

- [ ] `<h1> a <h6>`

### 🧾 2. display: inline

👉 Ocupa solo el ancho de su contenido y no fuerza salto de línea.

📘 Ejemplo:

```html
<span style="display: inline; background: green;">Texto 1</span>
<span style="display: inline; background: blue;">Texto 2</span>
```

🔹 Resultado:

Ambos span aparecen en la misma línea.
<span style="display: inline; background: green;">Texto 1</span>
<span style="display: inline; background: blue;">Texto 2</span>

No se pueden aplicar propiedades como width o height (no tienen efecto).

🧱 Ejemplos de elementos inline por defecto:

- [ ] `<span>`

- [ ] `<a>`

- [ ] `<strong>`

### ⚙️ 3. display: inline-block

👉 Mezcla lo mejor de ambos mundos:

Se comporta como inline (no rompe la línea),

pero acepta ancho y alto (width, height).

📘 Ejemplo:

```html
<span
  style="display: inline-block; width: 100px; height: 50px; background: green;"
>
  Bloque en línea 1
</span>

<span
  style="display: inline-block; width: 100px; height: 50px; background: blue;"
>
  Bloque en línea 2
</span>
```

🔹 Resultado:

Permite controlar su tamaño sin saltar de línea.

<span style="display: inline-block; width: 100px; height: 50px; background: green;">
  Bloque en línea 1
</span>

<span style="display: inline-block; width: 100px; height: 50px; background: blue;">
  Bloque en línea 2
</span>

### 🧮 4. display: none

👉 El elemento no se muestra ni ocupa espacio.

📘 Ejemplo:

```html
<p style="display: none;">No me verás</p>
```

🔹 Resultado:

El elemento desaparece completamente del DOM visual (aunque sigue en el HTML).

### 🧭 5. display: flex

👉 Convierte al elemento en un contenedor flexible (Flex Container)
y a sus hijos en ítems flexibles (Flex Items).

🧱 display: flex en detalle
🧩 Activar Flex

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  display: flex;
  background: #eee;
  height: 100px;
}
.item {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
```

Ahora todos los elementos hijos (.item) se distribuyen en una sola línea, horizontalmente por defecto.

📘 Ejemplo:

<div class="container1">
  <div class="item1">1</div>
  <div class="item1">2</div>
  <div class="item1">3</div>
</div>
<style>
.container1 {
display: flex;
background: #eee;
height: 100px;
}
.item1 {
background: green;
padding: 5px;
height:30px;
width: 30px;
margin: 5px;
}

</style>

🧭 Propiedades principales de Flexbox

#### 1. flex-direction

📘 Ejemplo:

```css
.container {
  display: flex;
  flex-direction: column;
  background: #eee;
  height: 200px;
}
.item {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
```

<div class="container2">
  <div class="item2">1</div>
  <div class="item2">2</div>
  <div class="item2">3</div>
</div>
<style>
.container2 {
display: flex;
flex-direction: column;
height: 200px;
background: #eee;
}
.item2 {
background: green;
padding: 5px;
height: 30px;
width: 30px;
margin: 5px;
}
</style>

#### 2. justify-content

Alinea los elementos en el eje principal.

Valor Descripción

- flex-start --> A la izquierda (inicio)
- center --> Al centro
- flex-end --> A la derecha (final)
- space-between --> Espaciados uniformemente
- space-around --> Espacio igual alrededor
- space-evenly --> Espacio igual entre todos

📘 Ejemplo:

```css
.container {
  display: flex;
  justify-content: space-between;
  background: #eee;
  height: 200px;
}
.item {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
```

<div class="container3">
  <div class="item3">1</div>
  <div class="item3">2</div>
  <div class="item3">3</div>
</div>
<style>
.container3 {
  display: flex;
  justify-content: space-between;
  background: #eee;
  height: 200px;
}
.item3 {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
</style>

3. align-items

Alinea los ítems en el eje cruzado (perpendicular).

Valor Descripción
flex-start Arriba
center Centro
flex-end Abajo
stretch Estira los ítems
baseline Alinea según texto base

📘 Ejemplo:

```css
.container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 200px;
  background: #eee;
}
.item {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
```

🎨 Ejemplo visual en código:

<div class="container">
  <div class="item"></div>
  <div class="item"></div>
  <div class="item"></div>
</div>

<style>
.container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 200px;
  background: #eee;
}
.item {
  background: green;
  padding: 5px;
  height: 30px;
  width: 30px;
  margin: 5px;
}
</style>
