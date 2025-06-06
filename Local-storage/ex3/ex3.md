Você está criando um gerenciador de tarefas onde os(as) usuários(as) podem adicionar e remover tarefas. No entanto, como o localStorage só aceita strings, precisamos converter os dados antes de salvar e recuperar.

Crie um script que:

● Tenha um input e um botão para adicionar tarefas.

● Salve as tarefas no localStorage como um array de strings usando JSON.stringify().

● Ao recarregar a página, recupere e exiba as tarefas salvas usando JSON.parse().

**Exemplo de entrada:**

O(a) usuário(a) adiciona as tarefas:

```js
["Comprar leite", "Fazer academia"]
```

**Saída Esperada (Ao recarregar a página):**


```js
Tarefas salvas: Comprar leite, Fazer academia
```

**Base do exercícios**

```html

<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lista de Tarefas</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Lista de Tarefas</h1>
    <input type="text" id="task-input" placeholder="Digite uma tarefa">
    <button id="add-task">Adicionar</button>
    <h2>Tarefas Salvas:</h2>
    <ul id="task-list"></ul>
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
}

```

