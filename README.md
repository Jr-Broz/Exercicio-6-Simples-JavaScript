# Exercicio-6-Simples-JavaScript

02 Exemplos de função em JavaScript que verifica se um número é primo.
***
* **EXEMPLO 1:**

A função "ehPrimo" recebe um parâmetro "num" e segue os seguintes passos:

Verifica se "num" é menor que 2. Se for, retorna false, já que números menores que 2 não são considerados primos.

Percorre um laço for de 2 até a raiz quadrada de "num" (Math.sqrt(num)), verificando se o resto da divisão entre `num` e o valor atual de `i` é igual a zero. 

Se for, significa que `num` é divisível por `i` e portanto não é primo. A função retorna `false`.

Se o laço for percorrido sem encontrar nenhum valor de `i` que divida `num`, significa que "num" é primo e a função retorna `true`.

A função `ehPrimo` é chamada com o valor 7 como argumento. Como 7 é um número primo, a função retorna true e esse valor é exibido no console pelo método `console.log`.

***

* **EXEMPLO 2:**
  
Com a mesma lógica do código anterior, porém percorre um laço for de 2 até "num - 1". 

Se o resto da divisão de `"num"` por algum número entre 2 e "num - 1" for igual a zero, a função retorna false, pois o número não é primo. 

Caso contrário, a função retorna true, indicando que o número é primo.

Uma observação importante é que essa implementação pode ser menos eficiente para números grandes, 

já que percorre um laço for com mais iterações do que a implementação anterior, que percorre apenas até a raiz quadrada de "num". 

Porém, para números pequenos, a diferença de desempenho é negligível.
