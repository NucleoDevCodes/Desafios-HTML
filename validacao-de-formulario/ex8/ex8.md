Você faz parte da equipe da organização de um festival de música e está responsável pelo formulário de compra de ingressos. Uma das regras que a organização colocou foi a de impedir que uma mesma pessoa compre mais de 2 ingressos. Portanto, você precisa:

● Criar uma validação que impeça que a pessoa adicione mais de 2 ingressos no campo indicado;

● Garantir que o campo seja preenchido obrigatoriamente;

● Exibir mensagens de erro para cada cenário de validação;

● Implementar uma indicação visual de que o input foi preenchido de forma incorreta.

Use o campo do CodePen abaixo e mostre como você faria as validações necessárias.

**Dicas:**

● O CSS para indicar que o input é inválido já foi adicionado aos estilos, você apenas deve implementar a lógica em JavaScript;

● Você pode consultar a [documentação do JustValidate](https://just-validate.dev/docs/intro) para te ajudar;

**Base do exercícios**

```html
<body>
    <div class="container">
			  <h1>Festival de música</h1>
        <form id="form" class="form">
            <fieldset class="campo-formulario">
                <label for="ingresso">Escolha a quantidade de ingressos:</label>
                <input id="ingresso" name="ingresso" type="number" />
                <span class="mensagem-erro"></span>
            </fieldset>
            <button type="submit">Enviar</button>
        </form>
    </div>
</body>
```

```css
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #EBD5E8;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.container {
    max-width: 500px;
    background: #FFF;
    padding: 2rem;
    border-radius: 16px;
    box-shadow: 0 0 16px rgba(0, 0, 0, 0.1);
    display:flex;
    flex-direction:column;
    align-items: center;
    gap:16px;
}

.titulo {
    font-size: 24px;
}

.form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 16px;
}

.campo-formulario {
    border: none;
}

input {
    width: 100%;
    padding: 0.5rem;
    border: 2px solid #CC92C2;
    border-radius: 24px;
}

button {
    width: 50%;
    padding: 1rem;
    background-color: #CC92C2;
    border: none;
    color: #FFF;
    font-weight: bold;
    border-radius: 24px;
    cursor: pointer;
    align-self: center;
}

button:hover {
    transform: scale(1.05);
}

.invalid {
    border: 2px solid #f7717d !important;
}
```



