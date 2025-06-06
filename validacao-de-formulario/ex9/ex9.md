A Code Connect, uma rede social para programadores, está aperfeiçoando seu formulário de cadastro. Agora o formulário possui um novo campo para confirmar o e-mail digitado. Seu desafio é:

● Criar uma validação para permitir que apenas senhas fortes (no mínimo 8 dígitos, letras maiúsculas e minúsculas, números e caracteres especiais) sejam utilizadas no campo “Digite uma senha”;

● Garantir que senha digitada no campo “Confirme sua senha” seja igual a senha digitada no campo “Digite uma senha”;

● Garantir que todos os campos sejam preenchidos obrigatoriamente;

● Exibir mensagens para cada cenário de validação;
Implementar uma indicação visual de que o input foi preenchido de forma incorreta.

Use o campo do CodePen abaixo e mostre como você faria as validações necessárias.

**Dicas:**

● O CSS para indicar que o input é inválido já foi adicionado aos estilos, você apenas deve implementar a lógica em JavaScript;

● Você pode consultar a [documentação do JustValidate](https://just-validate.dev/docs/intro) para te ajudar;

**Base do exercícios**

```html
<body>
    <div class="container">
        <h1>Code Connect</h1>
        <form id="form" class="form">
            <fieldset class="campo-formulario">
                <label for="senha">Digite uma senha:</label>
                <input id="senha" name="senha" type="text" />
                <span class="mensagem-erro"></span>
            </fieldset>
            <fieldset class="campo-formulario">
                <label for="confirmacao">Confirme sua senha:</label>
                <input id="confirmacao" name="confirmacao" type="text" />
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
    background-color: #E2D5CA;
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
    border: 2px solid #533E2D;
    border-radius: 24px;
}

button {
    width: 50%;
    padding: 1rem;
    background-color: #533E2D;
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