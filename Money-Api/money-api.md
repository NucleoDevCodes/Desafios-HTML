# Desafio conversão das moedas

Você deve criar uma aplicação ,asi avençada agpra usando uma Api que converta valores de dólares americanos (USD) para reais brasileiros (BRL).

✅ Requisitos:

● O usuário deve inserir um valor em dólar (USD) no campo de entrada.

● O valor convertido em real (BRL) deve aparecer automaticamente no segundo campo.

● A cotação do dólar pode ser fixa (por exemplo, R$ 6,00).

● Use HTML e JavaScript para implementar a lógica.

● Dica: use eventos e manipulação do DOM. 

***Dica**

```js
const apiKey = 'sua chave api'; 
const url = `https://v6.exchangerate-api.com/v6/${apiKey}/latest/USD`;

```

use também imput no HTML 

```html
    <section>
            <span class="cur">US$</span>
            <input id="usd" type="text" />
        </section>
        <section>
            <span class="cur">R$</span>
            <input id="brl" type="text" />
        </section>
```