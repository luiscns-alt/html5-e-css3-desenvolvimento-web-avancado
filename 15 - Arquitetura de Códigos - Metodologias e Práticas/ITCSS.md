Settings
É onde declaramos as configurações do nosso projeto, como variáveis de medidas, cores, etc.

```css
$my-color: #0057fb;
$footer-height: 120px;
```

Tools
É onde colocamos funções, mixings, placeholders, etc presentes nos Pré Processadores. Se não estiver utilizando algum Pré Processador, esta camada não será utilizada.

```css
@mixin my-box() {
  width: 200px;
  height: 100px;
}
```

Generics
Essa camada é para as propriedades com a menor especificidade. Por isso, o mais comum aqui é o seletor "\*".

```css
* {
  box-sizing: border-box;
}
```

Base
Essa camada é voltada para estilizações mais básicas dos elementos. Então, nada de IDs ou Classes, apenas o seletor de tags.

```css
div {
  padding: 10px;
}
```

Objects
Aqui utilizamos apenas classes. É onde declaramos a estilização da estrutura dos nossos elementos.

```css
.my-button {
  width: 200px;
  padding: 10px;
}
```

Components
Na camada anterior nós tentamos ser mais genéricos. Agora na camada Components nós podemos ser mais específicos quanto a estilização do elemento. Também só são permitidas classes.

```css
.my-red-button {
  background-color: red;
  color: white;
  border: 2px solid black;
}
```

Trumps
Esta camada tem as regras com a maior especificidade de todas, ou seja, se uma classe daqui for colocada em um elemento, as propriedades de uma classe da camada Trumps irá sobrescrever as propriedades declaradas em outras camadas.

Aqui é permitido o uso de !important.

A maioria das propriedades aqui são apenas pequenos ajustes que precisamos em certos elementos ou então definição de estado de um elemento.

```css
.hidden {
  display: none !important;
}
```
