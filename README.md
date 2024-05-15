# ebac_talks

**Comandos**
`npm init -y`
`npm i --save-dev parcel`

**link Animação**

[Link AOS](https://michalsnik.github.io/aos/)


**Data do JavaScript**

Podemos criar uma data utilizando o comando new Date(). A partir disso, teremos acesso a funções para recuperar o dia, mês, ano e obter a data em timestamp.

``const minhaData = new Date();``

Considerando a constante minhaData, temos:

```
minhaData.getTime() // retorna a data atual em timestamp
minhaData.getDate() // retorna o dia - número
minhaData.getDay() // retorna o dia, como índice, onde domingo = 0, segunda = 1
minhaData.getFullYear() // retorna o ano completo, ex: 2022
minhaData.getYear() // Retorna o ano porém considera o ano
2000 como 100, logo 2022 seria 122
minhaData.getHour() // retorna a hora atual em 24hrs
minhaData.getMinute() // retorna o minuto atual
minhaData.getSeconds() // retorna o segundo atual
```

Também podemos utilizar o new Date() para criar uma data específica, no passado ou futuro:

```
minhaData.getTime() // retorna a data atual em timestamp const dataNoPassado = new Date(“April 24, 2000 19:00:00”) const dataNoFuturo = new Date(“December 20, 2030 19:00:00”) // Seguimos a estrutura // (mês em inglês dia, ano horário 24hrs)

```

**SetInterval**

Com essa função, podemos executar uma função após determinado intervalo: setInterval(FUNCAO, intervalo); No primeiro argumento inserimos o código que será executado a cada intervalo e no segundo argumento passamos o tempo em milissegundos.

``` 
setInterval(function() { console.log(“olá”); }, 1000); // A cada 1 segundo teremos a mensagem olá no console

```

Para parar um intervalo, utilizamos a função clearInterval, passando o intervalo como argumento. Para isso precisamos armazenar o setInterval em uma varíavel: 

``` 
const contador = setInterval(function() { console.log(“olá”); }, 1000); // .... clearInterval(contador); // o contador será paralisado, para retomar será necessário criar um novo setInterval.

```

