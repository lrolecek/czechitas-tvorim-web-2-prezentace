# czechitas-tvorim-web-2-prezentace

## Instalace

```
> npm install
```

## Prezentování/editování

```
> npm install
```

a na localhost:8000 to běží

## Editování

### Nastavení

Pro editaci je obvykle dobré s zapnout (v index.html), resp. zakomentovat pro prezentování

* fragments: false,   // vypnout postupné zobrazování prvků s třídou fragment
* transition: 'none', // vypnout efekty na přechodu mezi slajdy
* showNotes: true,    // zapnout viditelné poznámky

### Slajdy

* jsou ve `slides` jako jednotlivé soubory (viz demo.md)
* aby se objevily v prezentaci, je potřeba je nalinkovat v `index.html`
* hlavní (horizontální) slajdy děláme obvykle jako samostatný soubor a vertikální jsou pomocí oddělovače `---` v tom samém
