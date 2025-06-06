Imagine que você está desenvolvendo um sistema de carrinho de compras para um site. O(a) usuário(a) pode adicionar e remover produtos, e os itens devem permanecer armazenados mesmo após recarregar a página.

Crie um script que:

● Permita adicionar produtos ao carrinho e armazená-los no localStorage.

●  Exiba os produtos salvos na tela.

●   Dê a opção de remover produtos específicos.

**Exemplo de entrada:**

O usuário(a) adiciona:

```js
{ nome: "Notebook", preco: 3500 }
{ nome: "Mouse", preco: 150 }
```
**Saída Esperada:**

```js
Carrinho: 
1. Notebook - R$3500
2. Mouse - R$150
```

Se o usuário(a) remover o "Mouse":

```js
Carrinho: 
1. Notebook - R$3500
```

**Base do exercícios**

```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Carrinho de Compras</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Carrinho de Compras</h1>
    <input type="text" id="product-name" placeholder="Nome do produto">
    <input type="number" id="product-price" placeholder="Preço do produto">
    <button id="add-product">Adicionar ao Carrinho</button>
    <h2>Produtos no Carrinho:</h2>
    <ul id="cart-list"></ul>
  </div>

  <script src="script.js"></script>
</body>

</html>
```

```js
body {
  font-family: Arial, sans-serif;
  text-align: center;
  padding: 50px;
}

.container {
  max-width: 400px;
  margin: auto;
}

input {
  padding: 8px;
  width: 90%;
  display: block;
  margin: 5px auto;
}

button {
  padding: 8px;
  margin-top: 10px;
  cursor: pointer;
}

h2 {
  margin-top: 16px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  background: #f0f0f0;
  padding: 8px;
  margin: 5px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

button.remove {
  background: red;
  color: white;
  border: none;
  padding: 5px;
  cursor: pointer;
  margin-top: 0px;
}

```
