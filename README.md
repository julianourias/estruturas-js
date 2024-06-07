# Estruturas de Controle em JavaScript

## Introdução
Este documento explora as estruturas de controle fundamentais em JavaScript: `if`, `else if`, `else`, `switch case`, `for loop` e `while loop`. Cada seção inclui uma breve explicação teórica e dois exemplos práticos para ilustrar o uso de cada estrutura.

## Estruturas de Controle

### If, Else If, e Else

#### Explicação
A estrutura `if` é usada para executar um bloco de código se uma condição especificada for verdadeira. O `else if` permite testar múltiplas condições, enquanto o `else` define um bloco de código a ser executado se nenhuma das condições anteriores for verdadeira. 

#### Quando usar
Use `if`, `else if`, e `else` quando precisar tomar decisões baseadas em condições diferentes. É ideal para situações onde há múltiplos caminhos possíveis que dependem de valores variáveis.

#### Exemplo 1
```javascript
let hour = 10;

if (hour < 12) {
    console.log("Bom dia!");
} else if (hour < 18) {
    console.log("Boa tarde!");
} else {
    console.log("Boa noite!");
}
```

#### Exemplo 2
```javascript
let score = 85;

if (score >= 90) {
    console.log("Nota A");
} else if (score >= 80) {
    console.log("Nota B");
} else if (score >= 70) {
    console.log("Nota C");
} else if (score >= 60) {
    console.log("Nota D");
} else {
    console.log("Nota F");
}
```

### Switch Case

#### Explicação
O `switch` é usado para executar um bloco de código entre várias opções possíveis com base na avaliação de uma expressão. Cada opção é definida por um `case`, e um `default` pode ser usado para capturar todos os outros casos não especificados.

#### Quando usar
Use `switch` quando tiver múltiplas condições possíveis que dependem do valor de uma única expressão. É especialmente útil quando há muitas condições que verificam a igualdade de uma expressão.

#### Exemplo 1
```javascript
let day = 3;

switch (day) {
    case 1:
        console.log("Segunda-feira");
        break;
    case 2:
        console.log("Terça-feira");
        break;
    case 3:
        console.log("Quarta-feira");
        break;
    case 4:
        console.log("Quinta-feira");
        break;
    case 5:
        console.log("Sexta-feira");
        break;
    default:
        console.log("Fim de semana");
}
```

#### Exemplo 2
```javascript
let fruit = "maçã";

switch (fruit) {
    case "banana":
        console.log("Bananas são amarelas");
        break;
    case "maçã":
        console.log("Maçãs podem ser vermelhas, verdes ou amarelas");
        break;
    case "laranja":
        console.log("Laranjas são laranjas");
        break;
    default:
        console.log("Fruta desconhecida");
}
```

### For Loop

#### Explicação
O `for` loop é usado para repetir um bloco de código um número específico de vezes. Ele é composto de três partes: a inicialização, a condição de continuação e a expressão de incremento.

#### Quando usar
Use o `for` loop quando souber de antemão quantas vezes deseja executar um bloco de código, especialmente quando precisar iterar sobre arrays ou coleções.

#### Exemplo 1
```javascript
for (let i = 0; i < 5; i++) {
    console.log("Número: " + i);
}
```

#### Exemplo 2
```javascript
let fruits = ["maçã", "banana", "laranja"];

for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}
```

### While Loop

#### Explicação
O `while` loop repete um bloco de código enquanto uma condição especificada for verdadeira. Diferente do `for` loop, a condição é verificada antes de cada iteração.

#### Quando usar
Use o `while` loop quando não souber de antemão quantas vezes o bloco de código deve ser executado e a repetição depender de uma condição que pode mudar durante a execução.

#### Exemplo 1
```javascript
let i = 0;

while (i < 5) {
    console.log("Número: " + i);
    i++;
}
```

#### Exemplo 2
```javascript
let password = "12345";
let userInput = "";

while (userInput !== password) {
    userInput = prompt("Digite a senha:");
}

console.log("Senha correta!");
```

## Conclusão
Cada uma dessas estruturas de controle tem seu uso específico em JavaScript. O `if`, `else if`, e `else` são ideais para decisões condicionais simples e complexas, o `switch case` é ótimo para múltiplas condições baseadas em uma única expressão, o `for loop` é perfeito para iterações com um número conhecido de repetições, e o `while loop` é adequado para situações onde a condição de parada não é conhecida de antemão. Entender quando e como usar cada uma dessas estruturas é fundamental para escrever código JavaScript eficiente e eficaz.
