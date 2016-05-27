<!-- .slide: data-background="#b82c7f" -->

# Demo kódu

===

# CSS

```css
/* Extra small devices (phones, less than 768px) */
/* No media query since this is the default in Bootstrap */

/* Small devices (tablets, 768px and up) */
@media (min-width: @screen-sm-min) { ... }

/* Medium devices (desktops, 992px and up) */
@media (min-width: @screen-md-min) { ... }

/* Large devices (large desktops, 1200px and up) */
@media (min-width: @screen-lg-min) { ... }
```
<!-- .element: class="c-text-sm stretch" -->

---

# HTML

```html
<!-- Stack the columns on mobile by making one full-width and the other half-width -->
<div class="row">
  <div class="col-xs-12 col-md-8">.col-xs-12 .col-md-8</div>
  <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
</div>

<!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
<div class="row">
  <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
  <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
  <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
</div>

<!-- Columns are always 50% wide, on mobile and desktop -->
<div class="row">
  <div class="col-xs-6">.col-xs-6</div>
  <div class="col-xs-6">.col-xs-6</div>
</div>
```
<!-- .element: class="c-text-xs stretch" -->

===

# Externí načítání kódu

<pre class="c-text-xs"><code class="sample" sample="slides/sample.html#foo"></code></pre>
<pre class="c-text-xs"><code class="sample" sample="slides/sample.css#foo"></code></pre>

>>>
* načítá kód z vnějších souborů, soubor může být delší a tímto z něj ukázat jen snippet(y)
* zároveň je nutno obalit komentáři alespoň jeden snippet (nejde načíst celý soubor)

---

## s ukázkou výsledku… v iframe

<pre class="c-text-xs"><code class="sample" sample="slides/sample.html#foo"></code></pre>

<div class="stretch">
<iframe class="" width="1500" height="100%" src="slides/sample.html">
</div>


