Agora, você precisa criar um sistema que registre quantas vezes o usuário visitou a página. Para isso, claro, você deve usar o localStorage. Você já deve ter visto algo assim principalmente em blogs, onde o número de visitas importa muito para quem quer monetizar na internet.

●  Toda vez que a pessoa usuária acessar a página, o contador de visitas aumenta.

● O número de visitas é exibido na tela.

● A pessoa usuária pode clicar em um botão para zerar o contador.

**Exemplo de saída:**

```js
Você visitou esta página 5 vezes.
```

Se o usuário clicar em "Zerar contador":

```js
Você visitou esta página 0 vezes.
```

**Base do exercícios**

```html
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contador de Visitas</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <div class="container">
    <h1 id="visit-count">Você visitou esta página 0 vezes.</h1>
    <button id="reset-btn">Zerar contador</button>
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
}

button {
  padding: 8px;
  margin-top: 10px;
  cursor: pointer;
}

```

