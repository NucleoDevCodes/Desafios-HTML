# Formulário Interativo com HTML e JavaScript

## 📝 Descrição da Atividade

Nesta aula, os alunos aprenderão a criar um formulário interativo usando HTML e JavaScript. O projeto consiste em desenvolver uma página web que coleta informações do usuário e exibe uma mensagem personalizada sem recarregar a página.

## 🎯 Objetivos de Aprendizagem

- Criar formulários HTML com diferentes tipos de campos
- Manipular eventos do DOM com JavaScript
- Capturar e processar dados de formulários
- Implementar funcionalidades interativas sem recarregar a página
- Exibir dados dinamicamente na página

## 🛠️ Ferramentas e Tecnologias

- HTML5
- JavaScript
- Manipulação do DOM
- Eventos em JavaScript
- Prevenção de comportamento padrão de formulários

## ✨ Funcionalidades

- Campo para inserção de nome
- Campo para inserção de idade
- Validação de preenchimento obrigatório
- Exibição de mensagem personalizada após envio
- Prevenção de recarregamento da página

## 📋 Instruções para os Alunos

1. Crie um arquivo HTML chamado `index.html`
2. No corpo do HTML, crie um formulário com os seguintes campos:
   - Um campo de texto para o nome
   - Um campo numérico para a idade
   - Um botão de enviar
3. Adicione um script JavaScript que:
   - Intercepte o envio do formulário (usando `addEventListener`)
   - Capture os valores de nome e idade
   - Exiba a mensagem: "Olá [nome], você tem [idade] anos e está autorizado a continuar o cadastro."

## ⚠️ Requisitos Específicos

- A mensagem deve aparecer na página, não em alertas
- O formulário não deve recarregar a página
- Use `innerText` ou `innerHTML` para exibir a mensagem
- Use `event.preventDefault()` para evitar o reload

## 💡 Dicas

- Lembre-se de dar IDs aos elementos para facilitar a manipulação com JavaScript
- Utilize `document.getElementById()` para capturar elementos do DOM
- Adicione o evento de submit ao formulário, não ao botão
- Teste o formulário para garantir que a página não recarrega após o envio

## 🔍 Conceitos Importantes

- **DOM (Document Object Model)**: É a representação de documentos HTML/XML que permite que linguagens como JavaScript acessem e manipulem o conteúdo da página
- **Event Listeners**: Permitem que você execute uma função quando um evento específico ocorre em um elemento
- **preventDefault()**: Método que cancela o comportamento padrão de um evento, como o envio de um formulário que normalmente recarregaria a página

## 📚 Recursos Adicionais

- [MDN Web Docs: Formulários HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/form)
- [MDN Web Docs: Eventos em JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/API/Event)
- [MDN Web Docs: Método preventDefault()](https://developer.mozilla.org/pt-BR/docs/Web/API/Event/preventDefault)

## 🧩 Desafios Extras (Opcionais)

1. Adicione validação para garantir que a idade seja maior que 18 anos
2. Adicione um campo de seleção para o gênero e inclua essa informação na mensagem
3. Estilize o formulário usando CSS para melhorar a aparência
4. Adicione a funcionalidade de limpar o formulário após o envio

---

Desenvolvido como parte do curso de Desenvolvimento Web da NucleoDevCodes.