# unifor 
**Disciplina:** raciocínio lógico algoritmico





**EXERCÍCIO 1**
Calcule a média de quatro números inteiros dados.


```mermaid
flowchart TD
id1([INICIO]) --> id2>Digite quatro números inteiros:]
id2 --> id3[/n1,n2,n3,n4/]
id3 --> id4[m= n1/4+n2/4+n3/4+n4/4]
id4 --> id5>A média aritmética dos quatro números digitados é: m]
id5 --> id([FIM])
```
```
Algoritmo "Media"
Var
  n1,n2, n3, n4 :real
Inicio
   Escreva ("Digite quatro números inteiros:")
   Leia (n1,n2,n3,n4)
   m<- n1/4+ n2/4+ n3/4+ n4/4
   Escreva ("A média aritmética dos quatro números digitados é:", m)
FIM_ALGORITMO
```






**EXERCÍCIO 2**
Leia uma temperatura dada em Celsius (C) e imprima o equivalente em Fahrenheit (F). (Fórmula de conversão: F = (9/5) * C + 32)
```mermaid
flowchart TD
id1([INICIO]) --> id2>Digite uma temperatura em celsius:]
id2 --> id3[/C/]
id3 --> id4[   F <- 9/5 * C + 32]
id4 --> id5>A temperatura que você digitou em Fahrenheit é: F]
id5 --> id([FIM])
```

```
Algoritmo "ConverteCelsiusFarenheit"
Var
  F, C : inteiro
Inicio
  Escreva("Digite uma temperatura em celsius:)
  Leia (C)
   F <- (9/5) * C + 32)
   Escreva("A temperatura que você digitou em Fahrenheit é:", F)   
FIM_ALGORITMO
```

**EXERCÍCIO 3**
Receba dois números reais e um operador e efetue a operação correspondente com os valores recebidos (operandos). O algoritmo deve retornar o resultado da operação selecionada simulando todas as operações de uma calculadora simples.

```mermaid
flowchart TD
id1([INICIO]) --> id2>Digite um número]
id2 -->  id3[/n1/]
id3 --> id4>Digite outro número:]
id4 --> id5[/n2/]
id5 --> id6>opções:]
id6 --> id7>1 - Soma]
id7 --> id8>2 - Subtração]
id8 --> id9>3 - Multiplicação]
id9 --> id10>4 - Divisão]
id10 --> id11{Caso 1}
id11 -- V --> id12>A soma dos dois números deu: n1+n2]
id11 -- F --> id13{Caso 2}
id13 -- V --> id14>A subtração dos dois números deu: n1-n2]
id13 -- F --> id15{Caso 3}
id15 -- V --> id16>A multiplicação dos dois números deu: n1*n2]
id15 -- F --> id17{Caso 4}
id17 -- V --> id18>A divisão dos dois números deu: n1/n2]
id18 -- F --> id19>Por favor, escolha uma opção de 1 a 4]
id12 --> id
id14 --> id
id16 --> id
id18 --> id
id19 --> id

 
id([FIM])
```

```
Algoritmo "Calculadora"
var
  n1,n2, opcao :inteiro
inicio
   escreva ("Digite um número")
   leia(n1)
   escreva ("Digite outro número")
   leia(2)
    escreva("opções:")
    escreval (")
    escreval ("(1) - Soma")
    escreval ("(2) - subtração")
    escreval ("(3) - multiplicação")
    escreval ("(4) - divisão")
    escreval ("")
    escreva("Escolha uma opção:")
    leia (opcao)
    escolha (opcao)
      caso 1
         escreva("A soma dos dois números deu:", n1+n2)
      caso 2 
          escreva("A subtração dos dois números deu:", n1-n2)
      caso 3
          escreva("A multiplicação dos dois números deu:", n1*n2)
      caso 4
           escreva("A divisão dos dois números deu:", n1/n2)
      caso contrario
           escreva ("Por favor, escolha uma opção de 1 a 4")
      fimcaso
FIM_ALGORITMO
```



### Exercício 04 (2.5 pontos)
Elaborar um algoritmo que, dada a idade, classifique nas categorias: infantil A (5 - 7 anos), infantil B (8 -10 anos), juvenil A (11 - 13 anos), juvenil B (14 -17 anos) e adulto (maiores que 18 anos).
```mermaid
flowchart TD
id1([INICIO]) --> id2>Digite a sua idade:]
id2 --> id3[/n/]
id3 --> id4{ caso 5<=n<=7}
id4 -- V --> id5>Você está na categoria infantil A]
id4 -- F --> id6{8<=n<=10}
id6 -- V --> id7>você está na categoria infantil B]
id6 -- F -->id8{11<=n<=13}
id8 -- V --> id9>você está na categoria juvenil A]
id8 -- F -->id10{14<=n<=17}
id10 -- V -->id11>você está na categoria juvenil B]
id10 -- F --> id12{caso n>=18}
id12 -- V --> id13>você está na categoria adulto]
id12 -- F --> id14{caso contrário}
id14-- V --> id15>esse algoritmo só trabalha com pessoas a partir de 5 anos]
id5 -->id
id7 --> id
id9 --> id
id11 -->id
id13 --> id
id15 --> id
id14 --> id
id([FIM])
```



```
Algoritmo "ClassificaCategoria"
var
  n: inteiro
inicio
  escreva ("Digite a sua idade:")
  leia (n)
  escolha(n)
    caso 5<=n<=7
      escreva ("Você está na categoria infantil A")
    caso 8<=n<=10
       escreva ("você está na categoria infantil B")
    caso 11<=n<=13
        escreva("você está na categoria juvenil A")
    caso 14<=n<=17
        escreva("você está na categoria juvenil B")
    caso n>=18
         escreva("você está na categoria adulto")
     Senao
         escreva("esse algoritmo só trabalha com pessoas a partir de 5 anos")
     fimcaso   
FIM_ALGORITMO
```

