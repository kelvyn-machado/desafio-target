# desafio-target
## Respostas aos desafios da vaga de estágio na Target - Ribeirão Preto

### Pergunta 1
```
1) Observe o trecho de código abaixo:

int INDICE = 13, SOMA = 0, K = 0;

enquanto K < INDICE faça

{

K = K + 1;

SOMA = SOMA + K;

}
imprimir(SOMA);

Ao final do processamento, qual será o valor da variável SOMA?
```
 Resposta 1: O valor da variável SOMA será 91 no fim do processamento.

### Pergunta 2
```
2) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

IMPORTANTE:

Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;
```

Resposta 2: 
```
 const isFibonacci = number => {
        if(number === 0 || number ===1) {
          return 'O número pertence a sequência Fibonacci.';
        }

        let prev = 1;
        let count = 2;
        let temp = 0;
        while(count <= number) {
          if(prev + count === number){
            return 'O número pertence a sequência Fibonacci.';
          };
          temp = prev;
          prev = count;
          count = count + temp;
        };
        return 'O número não pertence a sequência Fibonacci.'
         
      }

      console.log(fib(7));
      console.log(fib(8));
```
### Pergunta 3 
```
3) Descubra a lógica e complete o próximo elemento:

a) 1, 3, 5, 7, ____

b) 2, 4, 8, 16, 32, 64, ____

c) 0, 1, 4, 9, 16, 25, 36, ____

d) 4, 16, 36, 64, ____

e) 1, 1, 2, 3, 5, 8, ____

f) 2,10, 12, 16, 17, 18, 19, ____
```
Resposta 3: 
  a = 9; 
  b = 128; 
  c = 49; 
  d = 100; 
  e = 13; 
  f = 200;

### Pergunta 4 
```
4) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada.

Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?
```
Resposta 4: 
    Eu ligaria o primeiro interruptor e esperaria alguns minutos, após isso desligaria o primeiro e ligaria o segundo. Em seguida, iria até uma das salas. 
    Se a lâmpada da sala estiver acesa, então o segundo interruptor é o correto. Se a lâmpada estiver apagada e quenta, então o primeiro é o correto. Se  a lâmpada estiver apagada e fria, então o terceiro interruptor é o correto.

### Pergunta 5 
```
5) Escreva um programa que inverta os caracteres de um string.

IMPORTANTE:

a) Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;

b) Evite usar funções prontas, como, por exemplo, reverse;
```

Resposta 5: 
```
function reverseString(str){
  let r = "";
  for(let i = str.length-1; i >= 0; i--){
    r += str[i];
  }
  return r;
}
  
console.log(reverseString("Target"))
```
