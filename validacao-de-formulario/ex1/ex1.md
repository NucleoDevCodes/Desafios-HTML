Você está trabalhando no time de desenvolvimento da MoveHouse, uma plataforma digital para compra, venda e aluguel de imóveis. Os usuários podem anunciar seus imóveis diretamente pelo site, preenchendo um formulário com todas as informações do imóvel.

Um dos campos mais importantes é o título do anúncio, que será exibido em destaque na busca. Para garantir clareza e padronização, você precisa:

● Cria uma validação em JavaScript para verificar se o campo contém no mínimo 10 caracteres e no máximo 200 caracteres;

● Garantir que todos os campos sejam preenchidos obrigatoriamente;

● Exibir mensagens de erro personalizadas para cada cenário de validação;

● Implementar uma indicação visual de que o input foi preenchido de forma incorreta.

Use o campo do CodePen abaixo e mostre como você faria as validações necessárias.

**Dicas:**

O CSS para indicar que o input é inválido já foi adicionado aos estilos, você apenas deve implementar a lógica em JavaScript;
Você pode consultar a [documentação do JustValidate](https://just-validate.dev/docs/intro) para te ajudar;

**Base do exercícios**

```html
<body>
    <div class="container">
        <h1>MoveHouse</h1>
        <form id="form" class="form">
            <fieldset class="campo-formulario">
                <label for="texto">Faça a descrição do imóvel:</label>
                <textarea id="texto" name="texto" rows="4"></textarea>
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
    background-color: #E2E4F3;
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

textarea {
    width: 100%;
    padding: 0.5rem;
    border: 2px solid #06070E;
    border-radius: 24px;
    font-family: inherit;
    resize: vertical;
}


button {
    width: 50%;
    padding: 1rem;
    background-color: #06070E;
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