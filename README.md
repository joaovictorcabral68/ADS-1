# Par ou ímpar
## Objetivo
O objetivo desse **projeto** era criar um **programa** para informar se um número inteiro escolhido pelo usuario é **par ou ímpar**.

---
### Logica Utilizada:

Par ou ímpar é uma lógica bem conhecida:

1. Pedir que usuario informe um número
2. O programa lê esse número e me da a resposta
3. Se o número for divisível por 2 e o resto dessa divisão for 0 o programa vai informar ao usuario que o número é par
4. Caso contrario o programa vai informar que esse número é ímpar
5. Fim de programa
---

### Programa

Então depois de ter essa lógica em mente eu passei para o Portugol.

- **Variaveis usadas**:(`Inteiro Número`) os números que o usuario vai pedir são números inteiros por isso o uso dessa **variavel**
- **Dados de entrada**:(`Escreva/Leia`) O comando **escreva** para informar ao usuario para escrever um número, e o comando **leia** para selecionar a variavel número, e assim que o úsuario escrever o número ele automaticamente entra nessa variavel.
- **Operadores**: (`%`) Para indicar que o número tem que ser uma divisão por 2 e o resultado tem que ser 0.
- **Etrutura condicional**:(`SE/SENAO`) Usei esses comandos para dar dois caminhos para esse programa, **se** o número atender as condições é par, **senao** ímpar
---

### Resultado

```Portugol

programa {
  //Programa que indica se o número é par ou ímpar
  //Variaveis
inteiro numero
  funcao inicio() {
    //Processamento

    escreva("Par ou ímpar")
    escreva("\nDigite um número:")
    leia(numero)
    se(numero %2==0)
    escreva("PAR")
    senao
    escreva("ímpar")
    //Fim de programa
    
  }
}


```
---
# Maior de Dois
## Objetivo
O objetivo desse **projeto** era criar um **programa** para ler dois números inteiros e no final comparar os dois e mostrar se é maior ou igual.

---
### Logica Utilizada:

1. Pedir que usuario informe dois números separadamente 
2. O programa lê esses números e faz a comparação
3. Se for maior ou igual ele vai me dar a resposta de "Positivo"
4. Caso contrario o programa vai me dar a resposta de "Negativo"
5. Fim de programa
---

### Programa

Então depois de ter essa lógica em mente eu passei para o Portugol.

- **Variaveis usadas**:(`Inteiro Num 1/Num 2`) duas variaveis pois o usuario vai precisar digitar dois números e o inteiro pois vai ser utilizado números inteiros
- **Dados de entrada**:(`Escreva/Leia`) O comando **escreva** para informar ao usuario para escrever os números, e o comando **leia** para selecionar as duas variaveis, e assim que o úsuario escrever os números eles automaticamente entram nas variaveis.
- **Operadores**: (`>=`) Para indicar que os números tem que ser maior ou igual
- **Etrutura condicional**:(`SE/SENAO`) Usei esses comandos para dar dois caminhos para esse programa, **se** os números atenderem as condições é resposta positiva, **senao** resposta negativa
---

### Resultado
```Portugol

programa {
  //A funçao desse programa é ler dois números e fazer a comparação dos dois para saber se é maior ou igual.
  //Variaveis
  inteiro num1, num2
  funcao inicio() {
    //Processamento
    escreva("Informe um número:")
    leia(num1)
    escreva("Informe outro número:")
    leia(num2)
    se(num1>=num2)
    escreva("Positivo\n", num1 , " é maior ou igual à " , num2)
    senao
    escreva(" Negativo\n ", num1, " Não é maior ou igual à ", num2)
    
    //Fim de programa

    
  }
}
```
---
# Calculadora com Menu 
## Objetivo
O objetivo desse **projeto** era criar um **programa** para simular um funcionamento de uma calculadora, com as opções de Adição, subtração, multiplicação e divisão.

---
### Logica Utilizada:

1. Pedir que usuario informe qual das quatro operações ele quer fazer
2. Cada operação tem que pedir ao usuario dois números
3. Assim que o usuario informa os dois números o programa aplica a operação selecionada
4. E entrega o resultado para o usuario "O resultado da operação é:"
5. Fim de programa
---

### Programa

Então depois de ter essa lógica em mente eu passei para o Portugol.

- **Variaveis usadas**:(`Real Global Num 1/Num 2  Inteiro opcao`) duas variaveis globais pois o usuario vai precisar digitar dois números em todos os casos e o real pois o resultado das operações pode dar um número inteiro ou um número real, assim eu dou mais opções ao usuario e a **variavel** Inteiro para dar ao usuario as opções
- **Dados de entrada**:(`Escreva/Leia/Escolha`) O comando **escreva** para informar ao usuario para escrever os números, o comando **leia** para selecionar as três variaveis, e assim que o úsuario escrever os números e opções eles automaticamente entram nas variaveis e o comando **escolha** para dar ao usuario acesso às opções.
- **Operadores**: (`+ - * /`) Os quatro operadores que precisou para a calculadora
- **Etrutura condicional**:(`Caso`) Usei **Caso** pois para 4 operações nós temos 4 caminhos diferentes e este comando serve para separar cada operação no programa, dependendo da sua escolha no inicio, ele segue o caminho desejado.
### Exemplo:
1. Adição
2. Subtração

- Caso 1: `escreva(num 1 + num 2)`
- Caso 2: `escreava(num 1 - num2)`

>Se o usuario escolher Adição automaticamente o programa vai ler o **caso 1**
>Se o usuario escolher Subtração automaticamente o programa vai ler o **caso 2**

---

### Resultado
```Portugol
programa {
  //Variaveis globais
  real num1, num2
  funcao inicio() {
    //Variaveis
inteiro opcao
//Processamento
    escreva("\n1 Adição \n2.Subtração \n3.Multiplicação\n4.Divisão\nEscolha uma operação:")
    leia(opcao)
    escolha(opcao){
      
      //Soma
      
      caso 1:
      escreva("Adição:\nQuais números deseja somar?:")
      escreva("\nDigite um número:")
      leia(num1)
      escreva("digite outro número:")
      leia(num2)
      escreva("O resultado da soma é:" , num1+num2)

      //Subtração

      caso 2:
      escreva("Subtração: \nQuais números deseja subtrair?:")
      escreva("\nDigite um número:")
      leia(num1)
      escreva("Digite outro número:")
      leia(num2)
      escreva("O resultado da subtração é:", num1-num2)

      //Multiplicação

      caso 3:
      escreva("Multiplicação:\nQuais números deseja multiplicar?:")
      escreva("\nDigite um número:")
      leia(num1)
      escreva("Digite outro número:")
      leia(num2)
      escreva("O resultado da multiplicação é:", num1*num2)

      //Divisão

      caso 4:

      escreva("Divisão:\nQuais números deseja dividir?:")
      escreva("\nDigite um número:")
      leia(num1)
      escreva("Digite outro número:")
      leia(num2)
      escreva("O resultado da divisão é:", num1/num2)
      
      //Fim de programa

 }
    
  }
}
```
---

### Data do projeto: 04/03/2026



