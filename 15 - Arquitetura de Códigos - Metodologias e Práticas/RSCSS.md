Reasonable System for CSS. Ele foi feito pensando em escrever um CSS que tenha mais sentido e significado.

```html
<div class="search-form">
  <input type="search" class="input" />
  <button class="button">Buscar</button>
</div>
```

```css
.search-form{ . . . }
.search-form > .input{ . . . }
.search-form > .button { . . . }
```
