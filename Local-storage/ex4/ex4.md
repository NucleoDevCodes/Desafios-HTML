Você está desenvolvendo um sistema onde os(as) usuários(as) podem armazenar suas cores favoritas. No entanto, agora precisa permitir que eles(as) removam uma cor específica.

Crie um script que:

● Permita que o(a) usuário(a) adicione cores ao localStorage.

● Exiba todas as cores salvas.

● Tenha um botão para remover uma cor específica usando removeItem().

**Exemplo de entrada:**

O(a) usuário(a) adiciona as cores:

```js
["Azul", "Vermelho", "Verde"]
```

Saída Esperada (Após remover "Vermelho"):

```js
Cores salvas: Azul, Verde
```

**Base do exercícios**

```html

<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cores Favoritas</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Cores Favoritas</h1>
    <input type="text" id="color-input" placeholder="Digite uma cor">
    <button id="add-color">Adicionar Cor</button>
    <h2>Cores Salvas:</h2>
    <ul id="color-list"></ul>
  </div>

  <script src="script.js"></script>
</body>

</html>
```

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  padding: 50px;
}

.container {
  max-width: 300px;
  margin: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 16px;
}

input {
  padding: 8px;
  width: 80%;
}

button {
  padding: 8px;
  margin-top: 10px;
  cursor: pointer;
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
  gap: 5px;
}

button.remove {
  background: red;
  color: white;
  border: none;
  padding: 5px;
  cursor: pointer;
  margin-top: 0px
}

```





