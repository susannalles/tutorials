---
layout: default
title: CSS
date:   2020
author: Susanna Allés Torrent
nav_order: 4
---

## CSS: Style

To give style to a page, we can proceed in three different ways: 

1. Include the command inside the tag (not a good practise). E.g. `<p style=“font-size:12px”>`
2. Add the css inside the `<head>` tag, like this:

```html
<head>
	<title>Title of the page</title>
	<style type= “text/css”>
	(...)
	</style>
</head>
```

3. Create a different file that will contain all CSS rules `style.css` and will be included in the `<head>` of the HTML document:

`<link type="text/css" rel="stylesheet" href="style.css" />`

The most used option is the 3, because when we create, for example, a static website, we will not have to change the rules every time we create a page or HTML file, but all the rules will be in a separate file and we will have to change it only once.

The CSS syntax is simple but can get quite complicated. The basic structure of a CSS rule is as follows: 

```css
selector{
property: value; 
}
```

The selector can be any HTML tag or element or any class or identifier. The property is the characteristic that we want to modify, such as the background or font color, the font size and family, etc. Whereas the value is the actual aspect that we want to give to that or those HTML elements. 

The comments inside the CSS are marked like this: `/* Comment */`

Let's see which commands are the most basic: 
 
### Font Type:

- `font-size: Xpx;`
- Family font (Arial, Verdana, Impact, … ): `font-family: Arial;`
- There are different types of fonts: serif, sans-serif, cursive… Normally we choose several font types, in case the machine does not have the first one, it goes to the second one: `font-family: Tahoma, Verdana, sans-serif;`
- The sizes can be given in `px` pixels (e.g. `font-size:15px;`) and set to a fixed size, or in `em` which gives a size relative to the screen: `1em` corresponds to the default size, `0.5em` to half the size, and `2em` to twice the size. 

### Colors:

- `color: green;`
- Colors can be expressed in different ways: 
  * simple colors with names: `black`, `pink`, `violet`, `green`, `yellow`
  * hexadecimal values (# and 6 digits). Vid. [HTML Color Picker](https://www.w3schools.com/colors/colors_picker.asp).
- `background-color: red;`

### Alignment:
  
- center, right, left : `text-align:center;`


### Sizes: 
  
- `height:` the height is expressed in pixels
- `width:` the width is also expressed in pixels

It is especially useful for `div`: 

```css
div{
	background-color:#cc0000;
	height:100px;
	width:100px;
}
```

### Text decoration: 

We can give an special feature to certain elements. For instance, for the links, `<a>`, we can determine what color we want to be or if it needs to be underlined or not: 

```css
a{
	text-decoration: none;
}
```

### Borders:
  
Specially for tables, but also for `<div>`,  is useful to use borders. For instance, if we have a table: 

```css
selector{
	border: 1px solid black;
}
```

- `border-radius:` this would be to round the borders. 


Las reglas CSS pueden y deben darse de manera general, sin necesidad de añadir el atributo style a cada etiqueta. Para ello utilizaremos los atributos `@class` y `@id`: 
- `@class` sirve para dar estilo a una clase de elementos que comparten una serie de características. 
- `@id` sirve para dar un identifador único y por tanto otorogar una serie de características propias. 

Por ejemplo: 

- `<div class=“texto”>` suponemos que hay más de una `<div>` que queremos con las mismas características. En la CSS deberíamos señalarlo así, por ejemplo: 

```css
.texto{
	font-size:15px;
	font-family:Arial;
	color:blue;
}
```

Mientras que una `<div id= “contenedor”>` señala que es la única en todo el documento que habrá unas características concretas. En la CSS se reflejaría con el símbolo `#`:

```css
#contenedor{
	background-color: yellow;
}
```

#### Pseudo-selectores
  
Muy utilizado cuando queremos modificar parcialmente el comportamiento de un elemento, como en los links. Hay tres tipos diferentes: 

- `a:link:` link que no se ha todavía consultado
- `a:visited:` link consultado
- `a:hover:` cuando pasamos el cursor por encima. 

```css
selector:pseudo-class-selector{
	propiedad:valor}

a:hover {
    color: #cc0000;
    font-weight: bold;
    text-decoration: none;
}
```

#### Posición de los elementos `<div>`

- Apariencia:
	- `display` puede contener 5 valores:
	- `block`: los sitúa en bloque
	- `inline-block`: los sitúa en bloque sin sus medidas originales
	- `inline`:los sitúa en bloque sin sus medidas originales
	- `none`: desaparecen

- Margen: 
	- `margin`: espacio que hay fuera del elemento
	- `margin-top: /*some value*/`
	- `margin-right: /*some value*/`
	- `margin-bottom: /*some value*/`
	- `margin-left: /*some-value*/`

Pueden marcarse todos a la vez empezando por el de arriba: `margin: 1px 2px 3px 4px;`

- `border`: el borde es lo que delimita el elemento propiamente dicho
- `padding`: es el espacio entre el contenido y el borde

- Floatting:
	- `float:right`
	- `float:left;`

- Position: Hay cuatro tipos de posición: 
	- `absolute`: se posiciona en relación al primer elemento padre que no tiene `position:static`; si no hay tal elemento, el elemento con posición absoluta se coloca en relación al elemento `<html>`. 
	- `static`: La posición por defecto es `static`.
	- `relative`: es la más utilizada
	- `fixed`: para fijar un elemento en la pantalla (los menús por ejemplo)


Actualmente existen diferentes opciones para construir un sitio web estático. [Bootstrap](http://getbootstrap.com/) y [Foundation](http://foundation.zurb.com/) son dos de ellos, así como [Jekyll](http://jekyllrb.com/). 
