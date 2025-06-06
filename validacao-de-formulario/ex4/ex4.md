Você está desenvolvendo um sistema de inscrições para os treinamentos internos da TechWizard, uma empresa que cria soluções mágicas para o mundo da tecnologia. Para garantir que apenas as pessoas que trabalham na TechWizard se inscrevam, você precisa:

● Criar uma validação em JavaScript para verificar se o e-mail informado termina com @techwizard.io;
● Garantir que todos os campos sejam preenchidos obrigatoriamente;

● Exibir mensagens de erro personalizadas para cada cenário de validação;

● Implementar uma indicação visual de que o input foi preenchido de forma incorreta.

Use o campo do CodePen abaixo e mostre como você faria as validações necessárias.

**Dicas:**

● O CSS para indicar que o input é inválido já foi adicionado aos estilos, você apenas deve implementar a lógica em JavaScript;

● Você pode consultar a [documentação do JustValidate](https://just-validate.dev/docs/intro) para te ajudar;

**Base do exercícios**

```html
<body>
    <div class="container">
        <h1>TechWizard</h1>
        <form id="form" class="form">
            <fieldset class="campo-formulario">
                <label for="email">Digite seu e-mail corporativo:</label>
                <input id="email" name="email" type="email" />
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
    background-color: #EEDFF6;
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
    border: 2px solid #8332AC;
    border-radius: 24px;
}

button {
    width: 50%;
    padding: 1rem;
    background-color: #8332AC;
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