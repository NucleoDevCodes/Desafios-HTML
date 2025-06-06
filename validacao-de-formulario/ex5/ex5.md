A PetZen é uma clínica de bem-estar animal que oferece consultas presenciais com terapeutas para pets ansiosos, estressados ou hiperativos. Como a equipe só atende durante o horário comercial, os agendamentos só podem ser feitos entre 08:00 e 18:00. Sua tarefa é:

● Criar uma validação personalizada com JavaScript para que o(a) tutor(a) do pet escolha um horário válido entre 8h e 18h;

● Garantir que todos os campos sejam preenchidos obrigatoriamente;

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
        <h1>PetZen</h1>
        <form id="form" class="form">
            <fieldset class="campo-formulario">
                <label for="horario">Escolha um horário para atendimento:</label>
                <input id="horario" name="horario" type="time" />
                <span class="mensagem-erro"></span>
            </fieldset>
            <button type="submit">Enviar</button>
        </form>
    </div>
    <script src="https://unpkg.com/just-validate@latest/dist/just-validate.production.min.js"></script>
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
    background-color: #EBF3E3;
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
    border: 2px solid #698F3F;
    border-radius: 24px;
}

button {
    width: 50%;
    padding: 1rem;
    background-color: #698F3F;
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