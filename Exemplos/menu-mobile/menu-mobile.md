# 📱 Exercício Prático: Criando um Menu Mobile Responsivo com HTML, CSS e JavaScript

Quer aprender a construir um menu mobile moderno e funcional? Este exercício vai te guiar passo a passo na criação de um **menu responsivo**, com animação de abertura e fechamento, usando apenas **HTML, CSS e JavaScript puro**!

---

## 🎯 Objetivo

Desenvolver um menu mobile que:
- Apareça ao clicar em um botão (ícone "hambúrguer");
- Exiba os links de navegação de forma clara e responsiva;
- Inclua efeitos visuais com transições suaves;
- Seja funcional tanto em dispositivos móveis quanto em desktop.

---

## 🧰 Tecnologias Utilizadas

- HTML5
- CSS3 (Flexbox, Media Queries, Transições)
- JavaScript (DOM, Eventos)

---

## 📂 O que você vai praticar

- Criação de layout responsivo
- Manipulação do DOM com JavaScript
- Estruturação semântica com HTML
- Estilização com CSS moderno

---

## 🚀 Desafio Extra (opcional)

Adicione um **efeito de escurecimento no fundo** quando o menu estiver aberto, simulando um modal.

---

## 📎 Recursos

Você pode começar com este esqueleto base:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu Mobile</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <button id="menu-toggle">☰</button>
    <nav id="mobile-menu" class="hidden">
      <ul>
        <li><a href="#">Início</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Serviços</a></li>
        <li><a href="#">Contato</a></li>
      </ul>
    </nav>
  </header>
  <script src="script.js"></script>
</body>
</html>
```

💡 Dica: Use @media (max-width: 768px) para aplicar estilos apenas em telas menores.

Bora codar? 💻🚀
