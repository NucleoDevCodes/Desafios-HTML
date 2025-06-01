Seu site agora precisa de um botão de "Limpar Tudo", permitindo que o(a) usuário(a) apague todos os dados armazenados no localStorage.

Crie um script que:

● Armazene alguns dados no Local Storage (como nome e idade).

● Exiba os dados na tela.

● Tenha um botão que, ao ser clicado, use clear() para apagar tudo.

**Exemplo de saída:**

```js
Nome: Alice
Idade: 25
```
Após clicar em "Limpar Tudo":

```js
Nenhum dado encontrado.
```

```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gerenciar Dados</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Armazenamento de Dados</h1>
    <input type="text" id="name-input" placeholder="Digite seu nome">
    <input type="number" id="age-input" placeholder="Digite sua idade">
    <button id="save-data">Salvar Dados</button>
    <button id="clear-data" class="clear">Limpar Tudo</button>
    <h2>Dados Salvos:</h2>
    <p id="data-display">Nenhum dado encontrado.</p>
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
  display: block;
  margin: 5px auto;
}

button {
  padding: 8px;
  margin-top: 10px;
  cursor: pointer;
}

button.clear {
  background: red;
  color: white;
  border: none;
}

```