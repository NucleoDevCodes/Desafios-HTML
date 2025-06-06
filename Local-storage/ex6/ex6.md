Você precisa criar um sistema onde, ao modificar um dado no Local Storage em uma aba, ele também seja atualizado automaticamente em outra aba aberta do navegador.

Crie um script que:

●  Permita que o(a) usuário(a) digite um nome e salve no localStorage.

● Atualize o nome em tempo real em todas as abas abertas do site usando storage event.

●  Abra o editor do codepen em uma nova aba e duplique ela.

● Escreva sua solução e salve. Depois faça o teste.

**Exemplo de interação:**

O(a) usuário(a) altera o nome para "Carlos" em uma aba.
Outra aba aberta recebe essa alteração automaticamente.

**Base do exercícios**


```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sincronização entre Abas</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Sincronizar Nome entre Abas</h1>
    <input type="text" id="name-input" placeholder="Digite seu nome">
    <button id="save-name">Salvar Nome</button>
    <h2>Nome Salvo:</h2>
    <p id="name-display">Nenhum nome salvo.</p>
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

```