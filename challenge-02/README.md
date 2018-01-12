# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function example(a, b) {
  return a + b;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var getResult = example(5, 10) + 5;

// Qual o valor atualizado dessa variável?
20

// Declare uma nova variável, sem valor.
var num;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function example() {
  num = 10;
  return "O valor da variável agora é 10."
}

// Invoque a função criada acima.
example();

// Qual o retorno da função? (Use comentários de bloco).
/*
  'O valor da variável agora é 10.'
*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function example(a, b, c) {
    if(a == '' || b == '' || c == '') {
       return "Preencha todos os valores corretamente!";
    }
    else {
       return (a * b * c) + 2;
    }
}

// Invoque a função criada acima, passando só dois números como argumento.
example(1, 2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
NaN

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
example(1, 2, 3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
8

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function example(a, b, c) {
    if(a == undefined && b == undefined && c != '')
        return c;
    else if(a == undefined && b != '' && c == undefined)
        return b;
    else if(a != '' && b == undefined && c == undefined)
          return a;
    else if (a != '' && b != '' && c == undefined)
        return a + b;
    else if(a != '' && b == undefined && c != '')
        return a + c;
    else if(a == undefined && b != '' && c != '')
        return b + c;
    else if(a != '' && b != '' && c != '')
        return (a + b) / c;
    else if(a == undefined && b == undefined && c == undefined)
        return false;
    else {
      return null;
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
example(); // Resultado = undefined;
example(5); // Resultado = 5;
example(5,10); // Resultado = 15;
example(5,10,2); // Resultado = 7,5;
```
