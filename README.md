# Prezentace pro _Tvořím web 2_

## Instalace

```
> npm install
```

## Prezentování/editování

```
> grunt serve
```

Spustí na localhost:8000 server, kde to běží. Je tam hlídání změn, takže jak obsah slajdů, tak index.html a soubory s SCSS se kompilují obnovuje se samo v prohlížeči.

## Editování

### Nastavení

Pro editaci je obvykle dobré s zapnout (v index.html), resp. zakomentovat pro prezentování

* fragments: false,   // vypnout postupné zobrazování prvků s třídou fragment
* transition: 'none', // vypnout efekty na přechodu mezi slajdy
* showNotes: true,    // zapnout viditelné poznámky

### Slajdy

* píšeme v primárně v Markdownu, ale tak jako v Markdownu jde použít i HTML
* jsou ve `slides` jako jednotlivé soubory (viz demo.md)
* aby se objevily v prezentaci, je potřeba je nalinkovat v `index.html`
* hlavní (horizontální) slajdy děláme obvykle jako samostatný soubor (ale lze je dělat i v rámci jednoho souboru pomocí odělovače `\n===\n`) a vertikální jsou pomocí oddělovače `\n---\n` v tom samém (pokud je třeba udělat `<hr>`, tak pomocí více než tří `-`)

### Poznámky pro přednášejícího

* Píšou se na konec slajdu za `\n>>>`
* Pokud možno by měly být srozumitelné pro každého (např. viditelné s vystavenou prezentací na internetu)

## Kompatibilita

* Dle Reveal.js, ale naše úpravy jsou testovány jen v nejnovějším Chrome.