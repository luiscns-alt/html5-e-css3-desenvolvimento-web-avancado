#### Block

É uma abstração de um elemento, um novo componente. Ele é visto como um elemento pai.

```CSS
.botao{ . . . }
```

#### Elements

Filhos do Block, ou seja, elementos que serão colocados dentro de um elemento considerado Block. O nome de suas classes devem ser escritos com dois "\_" após o nome do Block.

```CSS
.botao__label{ . . . }
```

####Modifiers
Podem modificar o estilo do Block. O nome das classes dos Modifiers devem ser escritos com dois "-" após o nome do Block.

```CSS
.botao--azul{ . . . }
```

####Elementos HTML
Com as classes que criamos acima, nosso HTML poderia ficar assim:

```HTML
<button class="botao botao--azul" >
   <span class="botao__label" >Click Me</span>
</button>
```
