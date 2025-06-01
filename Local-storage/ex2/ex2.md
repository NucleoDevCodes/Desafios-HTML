Agora, imagine que você está desenvolvendo um site onde os(as) usuários(as) podem escolher entre o modo claro e o modo escuro. Quando um(a) usuário(a) escolhe um tema, essa escolha deve ser salva para que, ao voltar ao site, o tema selecionado permaneça ativo.

**Crie um programa que:**

1- Exiba dois botões: "Modo Claro" e "Modo Escuro".
2- Quando o(a) usuário(o) clicar em um dos botões, salve a escolha no localStorage.
3- Ao recarregar a página, aplique automaticamente o tema salvo.

**Exemplo de Interação:**

● O(a) usuário(a) clica em "Modo Escuro", a cor de fundo muda e a escolha é salva.

● Ao recarregar a página, o site continua em modo escuro.

```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alternar Tema</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1>Escolha um tema</h1>
    <button id="light-mode">Modo Claro</button>
    <button id="dark-mode">Modo Escuro</button>
  </div>

  <script src="script.js"></script>
</body>

</html>

```

```css
body {
  font-family: Arial, sans-serif;
  transition: background 0.3s, color 0.3s;
  text-align: center;
  padding: 50px;
}

.container {
  max-width: 300px;
  margin: auto;
}

button {
  padding: 10px;
  margin: 10px;
  cursor: pointer;
  border: none;
  font-size: 16px;
}

#light-mode {
  background: #f0f0f0;
  color: #000;
}

#dark-mode {
  background: #333;
  color: #fff;
}

/* Tema escuro */
.dark {
  background: #222;
  color: #fff;
}
```

