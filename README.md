# Learning HTML5 [![Date](https://img.shields.io/badge/Date-18%2F07%2F2020-success)](http://www.fechadehoy.com/mexico)

_Apuntes de mi aprendizaje en HTML5._

> **H**yper **T**ext **M**arckup **L**anguaje, _(en español: Lenguaje de Marcado de HyperTexto)_ es un lenguaje que se utiliza para estructurar sitios web; HTML establece `¿qué?` se muestra.

Otras Guías de Estilos

-   [CSS](https://github.com/nhuamani/css)
-   [JavaScript](https://github.com/nhuamani/javascript)
-   [GIT](https://github.com/nhuamani/git)

## Table of Contents

1. [Sintaxis](#sintaxis)
    1. [Tipos de Elementos](#tipos-de-elementos)
        1. [Apertura / Cierre](#normal-elements-apertura-y-cierre)
        2. [Self Closing](#void-elements-self-closing)
2. [Categoría de Elementos](#categoria-de-elementos)
    1. [Inline-level elements](#inline-level-elements)
    2. [Block-level elements](#block-level-elements)
3. [Entidades HTML](#entidades-html)
4. [Estructura Básica](#estructura-básica)
5. [Estructura HTML 5](#estructura-html-5)

---

## Sintaxis

![Sintaxis de HTML](https://nhuamani.github.io/images/html-sintaxis.png)

[⇡ back to top](#table-of-contents)

### Tipos de Elementos

Hay seis tipos diferentes de elementos: void elements, the template element, raw text elements, escapable raw text elements, foreign elements, and normal elements.

#### Normal elements - apertura y cierre

```html
<!-- Example -->

<h1></h1>
<p></p>
<audio></audio>
<video></video>
<address></address>
...
```

> **Nota:** La mayor cántidad de elementos son de este tipo; pero existen mas tipos de elementos.

#### Void elements - Self Closing

```html
<!-- Example -->

<img/>
<meta/>
<link/>
<input/>
<br/>
<hr/>
<source/>
<col/>
<embed/>
<param/>
<track/>
<wbr/>
```

> ℹ [_WHATWG_](https://html.spec.whatwg.org/multipage/syntax.html#elements-2)

## Categoría de Elementos

### Inline-level elements

Los elementos **inline** se colocan uno al lado del otro hasta completar el espacio disponible, luego se colocan uno debajo del otro.

```html
<!-- Example -->

<code></code/>
<strong></strong>
<label></label>
<kbd></kbd>
<span></span> ★
...
```

> ℹ [_MDN_](https://developer.mozilla.org/es/docs/Web/HTML/Inline_elements)

### Block-level elements

Los elementos **block** reservan todo el espacio horizontal aunque no lo ocupen por completo.

```html
<!-- Example -->

<pre></pre>
<h1> through <h6>
<blockquote></blockquote>
<table></table>
<div></div> ★
...
```

> ℹ [_MDN_](https://developer.mozilla.org/es/docs/Web/HTML/Block-level_elements)

[⇡ back to top](#table-of-contents)

## Entidades HTML

Para poder incluir los caracteres **>** y **<**, cuando quires escribir código html en una página web y para los caracteres Unicode, aunque ya no es nesesario por el soporte de [Unicode UTF-8](https://unicode-table.com).

```html
<!-- Example -->

&copy;
<p>Las etiquetas html se escriben así:
    &lt;p&gt;hola&lt;/p&gt; // <!-- <p></p> -->
</p>
&alpha;
α
```
> 💡 &lt; es smaller than y &gt; greater than.

**[⇡ back to top](#table-of-contents)**

## Estructura Básica

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Document</title>
    </head>

    <body>
        <h1>My Firts Page</h1>
    </body>
</html>
```

> **Nota:** Con esta estructura ya tienes una página.

## Atributos

> 💡 _Algunos atributos no son obligatorios, no requieren valor._

```html
<!-- Example -->

<input required placehoder>
```

## Estructura HTML5

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta name="description" content="This is my first web page, thanks for visiting" />
        <title>First Document</title>
        <link rel="icon" href="favicon.ico" />
    </head>

    <body>
        <!-- This a comment -->
        <h1>My Firts Page</h1>
    </body>
</html>
```

## Estructura semántica HTML5
Organizational elements

## Comentarios

## Favicon en la pagina web

## Formato de texto (dividir más)

## Link

## Listas ordenadas

## Listas no ordenadas

## Tablas

## Imagenes

## Audio

## Video

## Iframe

## Iframes Maps

## Forms

## Temas de Interes

-   [Unicode UTF-8](https://unicode-table.com)
-   [ASCII Code](https://elcodigoascii.com.ar)

## Source

-   [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
-   [W3C Recommendation (2017)](https://www.w3.org/TR/html52/)
-   [Living Standard (2020))](https://html.spec.whatwg.org/)
-   [Mozilla Developer Network](https://developer.mozilla.org/es/docs/Web/HTML)

**[☝ back to top](#table-of-contents)**
