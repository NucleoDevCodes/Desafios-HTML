Agora você vai criar um sistema de login que armazena a sessão do(a) usuário(a) no localStorage.

O(a) usuário(a) insere um nome de usuário e senha e clica em "Entrar". O nome do usuário(a) e senha fica armazenado no localStorage, e uma mensagem de "Bem-vindo" aparece.

Se a pessoa usuária sair da página e voltar, ele continua logado. Um botão "Sair" permite remover a pessoa usuária do Local Storage e redirecioná-lo para a tela de login.

**Exemplo de entrada:**

```js
Usuário: joao123
Senha: ser3523ft!#


Saída Esperada:

```bash
Bem-vindo, joao123!
```

**Base do exercícios**

```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login com Local Storage</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1 id="title">Login</h1>

    <div id="login-form">
      <input type="text" id="username" placeholder="Usuário">
      <input type="password" id="password" placeholder="Senha">
      <button id="login-btn">Entrar</button>
    </div>

    <div id="welcome-message" class="hidden">
      <h2 id="user-welcome"></h2>
      <button id="logout-btn">Sair</button>
    </div>
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
  max-width: 300px;
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

.hidden {
  display: none;
}

```