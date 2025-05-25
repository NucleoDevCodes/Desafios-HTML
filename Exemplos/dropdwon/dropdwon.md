# ⬇️ Desafio de Programação: Crie um Dropdown com HTML, CSS e JavaScript!

Vamos colocar em prática um dos componentes mais usados na web: o **menu dropdown**! Seja para navegação, filtros ou opções ocultas, aprender a criar um dropdown interativo é essencial para qualquer desenvolvedor front-end. 🚀

## 🎯 Objetivo

Você vai desenvolver um menu suspenso que:

- Exibe uma lista de opções ao clicar em um botão
- Esconde as opções ao clicar fora ou selecionar uma delas
- Tem um design limpo e responsivo

## 🧰 Tecnologias Usadas

- **HTML** para estruturar
- **CSS** para estilizar o menu e os efeitos de transição
- **JavaScript** para lidar com os eventos de clique e alternar a visibilidade

## 📦 O que você precisa entregar

Um pequeno projeto com:

- Um botão que abre e fecha o menu
- Estilização básica do dropdown
- Funcionalidade interativa com JavaScript

### Exemplo de estrutura inicial:

```html
<div class="dropdown">
  <button id="dropdownButton">Menu ▼</button>
  <ul id="dropdownMenu" class="dropdown-content">
    <li><a href="#">Opção 1</a></li>
    <li><a href="#">Opção 2</a></li>
    <li><a href="#">Opção 3</a></li>
  </ul>
</div>
```

E no JavaScript:

```js
const button = document.getElementById('dropdownButton');
const menu = document.getElementById('dropdownMenu');

button.addEventListener('click', () => {
  menu.classList.toggle('show');
});
```

🧠 Desafios Extras (opcional)
Fechar o menu ao clicar fora dele

Adicionar animação na abertura/fechamento

Tornar o menu acessível com teclado

💡 Dica: Use position: absolute; no CSS para posicionar o menu, e display: none/block ou opacity/visibility para os efeitos de transição.

Pronto para colocar seu dropdown no ar? Bora codar! 💻🔥




