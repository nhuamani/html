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
        1. [Apertura / Cierre](#normal-elements---apertura-y-cierre)
        2. [Self Closing](#void-elements---self-closing)
2. [Categoría de Elementos](#categoria-de-elementos)
    1. [Inline-level elements](#inline-level-elements)
    2. [Block-level elements](#block-level-elements)
3. [Entidades HTML](#entidades-html)
4. [Estructura Básica](#estructura-básica)
5. [Estructura HTML 5](#estructura-html-5)

---

## Sintaxis

![Sintaxis de HTML](https://nhuamani.github.io/images/html-sintaxis.png)

### Tipos de Elementos

Hay seis tipos diferentes de elementos: void elements, the template element, raw text elements, escapable raw text elements, foreign elements, and normal elements.

#### Normal elements - apertura y cierre

```html
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
<img />
<meta />
<link />
<input />
<br />
<hr />
<source />
<col />
<embed />
<param />
<track />
<wbr />
```

> 💡 _En HTML5, no es obligatorio cerrar las etiquetas self-closing._

> ℹ [_WHATWG_](https://html.spec.whatwg.org/multipage/syntax.html#elements-2)

[⇡ back to top](#table-of-contents)

## Categoría de Elementos

### Inline-level elements

Los elementos **inline** se colocan uno al lado del otro hasta completar el espacio disponible, luego se colocan uno debajo del otro.

```html
<code></code>
<strong></strong>
<label></label>
<kbd></kbd>
<span>★</span>
...
```

> ℹ [_MDN_](https://developer.mozilla.org/es/docs/Web/HTML/Inline_elements)

### Block-level elements

Los elementos **block** reservan todo el espacio horizontal aunque no lo ocupen por completo.

```html
<pre></pre>
<cite></cite>
<blockquote></blockquote>
<table></table>
<div>★</div>
...
```

> ℹ [_MDN_](https://developer.mozilla.org/es/docs/Web/HTML/Block-level_elements)

[⇡ back to top](#table-of-contents)

## Entidades HTML

Para poder incluir los caracteres **>** y **<**, cuando quires escribir código html en una página web y para los caracteres Unicode, aunque ya no es nesesario por el soporte de [Unicode UTF-8](https://unicode-table.com).

```html
&copy;
<p>
    Las etiquetas html se escriben así: &lt;p&gt;hola&lt;/p&gt;
    <!-- <p></p> -->
</p>
&alpha; α
```

> 💡 _&lt; es smaller than y &gt; greater than._

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

> 💡 Si la pagina no tiene la instrucción `<!DOCTYPE html>`, el navegador se pone en **quirks mode**

Leé este articulo para saber más.

-   [_Cómo funcionan los navegadores_](https://www.html5rocks.com/es/tutorials/internals/howbrowserswork/)

[⇡ back to top](#table-of-contents)

## **Atributos**

![Atributos en HTML](https://nhuamani.github.io/images/html-atributos.png)

> **Nota:** Caracteristicas de los atributos

### Tipos de atributos

#### Atributos Booleanos

```html
<input required placehoder />
```

> 💡 _Algunos atributos no requieren valor._

#### Atributos Opcionales y Obligatorios

```html
<!-- Atributo obligatorio-->
<img src="imagen.png" alt="imagen" />
<a href="#">Link</a>

<!-- class y id son un Atributo Opcional -->
<img src="imagen.png" alt="imagen" class="imagen-banner" id="imagen" />
```

#### Atributos **data-\***

Algunas propiedades de JavaScript se pone como atributo: la forma elegante de poner un atributo a una &lt;etiqueta&gt; HTML es con **data-ng-app , data-ng-filter**

```html
<!-- Atributo personalizados-->
<div data-ng-app data-menu-active></div>
```

> 💡 _Este tipo de atributos es utilizado en los framework Angular React y Vue._

[⇡ back to top](#table-of-contents)

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

### Favicon

> 💡 _Los favicon **favorites icon** en español (icono de página): se recomienda utilizar el tamaño 16x16 píxeles o 32x32 píxeles y en formato .ico o .png_

Puedes generar tus iconos en:

-   [Favicon-generator](https://www.favicon-generator.org/)
-   [Favicomatic](https://favicomatic.com/)
-   [Favicon generator](https://realfavicongenerator.net/)

## Estructura Semántica

### Organizational elements

Los elementos `<span></span>` y `<div></div>` son etiquetas genericas para los casos en que no hay una etiqueta especifica, no significan nada por sí solo, tambien se utiliza para agrupar elementos, `span` para los **Inline** y `div` para los **Block**.

### Elementos de Seccion

```html
<!-- Encabezado -->
<header></header>

<!-- Navegación, para menus -->
<nav></nav>

<!-- Pie de página -->
<footer></footer>

<!-- Contenido independiente -->
<article></article>

<!-- Contenido relacionado pero secundario -->
<aside></aside>

<!-- Secciones o divisores de un contenido -->
<section></section>

<!-- Para mostrar el contenido principal, debe ser único -->
<main></main>
```

### Estrucutra Semantica en HTML5

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Sample page</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta name="description" content="This is my first project with its detailed description." />
        <link rel="icon" href="https://github.githubassets.com/favicons/favicon.svg" />
        <link rel="stylesheet" type="text/css" href="style.css" />
    </head>
    <body>
        <header>
            <img src="assets/img/brand.png" alt="Brand Image" />
            <nav>
                <ul>
                    <li>Review</li>
                    <li>Mobile</li>
                    <li>Camera</li>
                    <li>Tablet</li>
                </ul>
            </nav>
        </header>

        <main>
            <h1>Recent News</h1>
            <article>
                <header>
                    <h2>SpaceX buys Amazon</h2>
                </header>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque voluptatibus, alias repellat temporibus quibusdam, voluptas eveniet
                    velit ex porro sunt quas pariatur nulla dolores aliquid commodi quidem enim fugiat hic!
                </p>
                <footer>
                    <p>Published June, 10 of 2021</p>
                </footer>
            </article>
        </main>

        <aside>
            <section>
                <h2>Follow in Twitter</h2>
            </section>
        </aside>

        <footer>
            <p>&copy; Company Name - 2021</p>
        </footer>
    </body>
</html>
```

> 💡 Evita aplicar los estilos directamente a las etiquetas.

> 💡 Se recomienda tener solo un `<h1></h1>` en la página.

#### Source

-   [Validador semántico de HTML5](https://validator.w3.org/)

## Semantica de Etiquetas

```html
<b>Bold text</b>
<i>Italic Text</i>
<u>Underline Text</u>
<sup>Superindice</sup>
<sub>Superindice</sub>
<del>Superindice</del>
<mark>100 hasta la 120</mark>
<address>100 hasta la 120</address>
<pre>Preformat</pre>
<code>console.log('Hello World!')</code>
<strong>Importancia</strong>
<em>Ènfasis</em>
<q>Citas (inline)</q>
<blockquote>Citas (block)</blockquote>
<cite>Citas Biblíografia</cite>
```

[⇡ back to top](#table-of-contents)

## Comentarios

Los comentarios se escriben de esta forma:

```html
<!-- this is a comment -->
```

[⇡ back to top](#table-of-contents)

## Formato de texto (dividir más)

[⇡ back to top](#table-of-contents)

## Link

El Elemento HTML Anchor <a> crea un enlace a otras páginas de internet, archivos o ubicaciones dentro de la misma página, direcciones de correo, o cualquier otra URL.

```html
<a href="https://example.com">Website</a>
```

### Atributos

**href**

```html
<!-- anclaje a un archivo externo -->
<a href="https://www.nhuamani.github.io/"> Enlace externo </a>

<!-- enlace a un elemento en esta página con id="attr-href" -->
<a href="#attr-href"> Descripción de enlaces de la misma página </a>
```

**target="\_blank"**

Por defecto es el target `_self` tambien existen `_parent` y `_top`.

```html
<!-- anclaje a un archivo externo -->

<a href="https://www.nhuamani.github.io/" target="_blank" rel="noopener noreferrer"> Enlace externo </a>
```

> **Nota:** Cuando se utiliza target, considera agregar rel="noopener noreferrer" para evitar el uso de la API window.opener.

**mailto:**

```html
<!-- anclaje a un archivo externo -->

<a href="mailto:nowhere@nhuamani.dev">Enviar correo a nowhere</a>
```

**tel:**

```html
<!-- anclaje a un archivo externo -->

<a href="tel:+491570156">+49 157 0156</a>
```

**download:**

Este atributo, indica descargar a los navegadores una URL en lugar de navegar hacia ella.

```html
<!-- anclaje a un archivo externo -->

<a href="https://octodex.github.com/images/Sentrytocat_octodex.jpg" download="true">Dowload Octodex</a>
```

[⇡ back to top](#table-of-contents)

## Listas ordenadas

[⇡ back to top](#table-of-contents)

## Listas no ordenadas

[⇡ back to top](#table-of-contents)

## Tablas

[⇡ back to top](#table-of-contents)

## Imagenes

[⇡ back to top](#table-of-contents)

## Audio

[⇡ back to top](#table-of-contents)

## Video

[⇡ back to top](#table-of-contents)

## Iframe

[⇡ back to top](#table-of-contents)

## Iframes Maps

[⇡ back to top](#table-of-contents)

## Forms

[⇡ back to top](#table-of-contents)

## Microdatos

Sets de atributos para especificar un elemento **que es semanticamente**.

Permiten especificar el significado del texto, usando un set de parametros especificados en [schema.org](https://schema.org).

Se indica con los siguientes atributos:

-   **itemscope** - (indica contexto, es un atributo booleano o vacio)
-   **itemtype** -(indica el tipo de schema, extraida desde [schema.org](http://schema.org))
-   **itemprop** - (indica el tipo de dato)

-   [Schema ](https://schema.org)_(Standar)_

### Google

-   [Structured Data - Google](https://developers.google.com/search/docs/guides/intro-structured-data)
-   [Testing Tools Structured Data](https://search.google.com/structured-data/testing-tool)

```html
<article itemscope itemtype="https://schema.org/Person">
    <img itemprop="image" src="profile.png" alt="Nilton Huamaní" />
    <h2 itemprop="name">Nilton Huamani</h2>
    <p itemprop="jobTitle">Frontend Developer</p>
    <p itemprop="email">nhuamani@gmail.com</p>
    <p itemprop="address">Cusco, Perú</p>
</article>

<article itemscope itemtype="https://schema.org/Book">
    <img itemprop="image" src="book.jpg" alt="Libro" />
    <h2 itemprop="name">Don Quijote de la Mancha</h2>
    <p itemprop="about">La historia de Don Quijote y sus aventuras</p>
    <p itemprop="author">Miguel de Cervantes Saavedra</p>
    <p itemprop="copyrightYear">1532</p>
</article>
```

### Facebook

-   [Open Graph Protocol - Facebook](https://schema.org/)
-   [Testing Tools Open Graph](https://developers.facebook.com/tools/debug/)

```html
<!-- Url de la página -->
<!-- Título de la página -->
<!-- Descripción de la página -->
<!-- Imagen para compartir -->

<meta property="og:url" content="https://nhuamani.github.io/blog" />
<meta property="og:title" content="Optimiza tu web con Twitter cards" />
<meta property="og:description" content="Con poco código puedes personalizar como Twitter muestra tu página al compartirla" />
<meta property="og:image" content="https://nhuamani.github.io/images/blog/twitter-cards.jpg" />

<!-- Extras -->
<meta property="og:type" content="website" />
<meta property="og:locale" content="es_PE" />
<meta property="og:site_name" content="nhuamani - Frontend Developer" />
```

Twitter

-   [Twitter for Websites with Cards](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)
-   [Twitter Card Validator](https://cards-dev.twitter.com/validator)

```html
<!-- Url de la página -->
<!-- Título de la página -->
<!-- Descripción de la página -->
<!-- Imagen para compartir -->

<meta name="twitter:url" content="https://nhuamani.github.io/blog" />
<meta name="twitter:title" content="Optimiza tu web con Twitter cards" />
<meta name="twitter:description" content="Con poco código puedes personalizar como Twitter muestra tu página al compartirla" />
<meta name="twitter:image" content="https://nhuamani.github.io/blog/twitter-cards.jpg" />

<!-- Extras-->
<meta property="twitter:card" content="summary_large_image" />
<meta property="twitter:site" content="@nhuamanic" />
```

## Temas de Interes

-   [Unicode UTF-8](https://unicode-table.com)
-   [ASCII Code](https://elcodigoascii.com.ar)

## Source

-   [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
-   [W3C Recommendation (2017)](https://www.w3.org/TR/html52/)
-   [Living Standard (2020))](https://html.spec.whatwg.org/)
-   [Mozilla Developer Network](https://developer.mozilla.org/es/docs/Web/HTML)

## Libraries

-   [Scroll Reveal](https://scrollrevealjs.org/)
-   [Smooth Scroll](https://github.com/iamdustan/smoothscroll)

**[☝ back to top](#table-of-contents)**
