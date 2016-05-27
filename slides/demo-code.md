<!-- .slide: data-background="#b82c7f" -->

# Demo kódu

---

# Externí načítání kódu

<pre class="c-text-xs"><code class="sample" sample="slides/sample.html#html"></code></pre>

>>>
* načítá kód z vnějších souborů, soubor může být delší a tímto z něj ukázat jen snippet(y)
* zároveň je nutno obalit komentáři alespoň jeden snippet (nejde načíst celý soubor)

---

## s ukázkou výsledku v iframe

<pre class="c-text-xs"><code class="sample" sample="slides/demo-sample.html#html"></code></pre>
<pre class="c-text-xs"><code class="sample" sample="slides/demo-sample.html#css" sample-type="css"></code></pre>
<pre class="c-text-xs"><code class="sample" sample="slides/demo-sample.css#css"></code></pre>
<pre class="c-text-xs"><code class="sample" sample="slides/demo-sample.html#script" sample-type="js"></code></pre>

<div class="stretch">
<iframe width="100%" height="100%" src="slides/demo-sample.html"></iframe>
</div>

>>>
* kód se automaticky reloaduje
* u inline css/js v html je potřeba nastavit typ kódu ručně