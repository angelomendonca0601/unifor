### Exercício 01
Atualize o algoritmo para determinar se um número inteiro e positivo é par ou ímpar, usando uma laço condicional para aceitar apenas números maiores ou iguais a zero. 


```mermaid
flowchart TD
id1([INICIO]) --> id2>"Digite um número"]
id2 --> id3[/n/]
id3 --> id4{n<0}
id4 -- V --> id5>"Digite um número maior ou igual a zero:"]
id5 --> id6[/n/]
id6 --Loop-->id4
id4 -- F --> id7{n%1 =0}
id7 -- F--> id8>Por favor, digite um número inteiro:]
id7 -- V --> id9{n%2=0}
id9 -- V --> id10>O número n é par]
id9 -- F --> id11>O número n é ímpar]
id11 --> id
id10 --> id
id8-->id


id([FIM])
```


```
Algoritmo "ClassificaCategoria"
Var
  n
Inicio
   Escreva("Digite um número")
   Leia(n)
   Enquanto n<0 faca
       Escreva("Digite um número")
       Leia(n)
   FimEnquanto
   Se n%1 = 0 entao
      Se n%2=0 entao
        Escreva("O número",n,"é par")
      Senao
        Escreva("O número",n,"é impar")
      FimSe
   Senao 
    Escreva("Por favor, digite um número inteiro")
   Fimse
FIM_ALGORITMO
```

### Exercício 02
Faça um algoritmo que exiba na tela uma contagem de 0 até 30, exibindo apenas os múltiplos de 3.


```mermaid
flowchart TD
id1([INICIO]) --> id2[i=1]
id2 --> id3[[i de 0 até 30 passo 1]]
id3 --> id4[/i/] 
id4 --> id5{i%3=0}
id5 -- V --> id6>i é múltiplo de 3]
id6 -- LOOP-->id3
id6 -->id([FIM])
```



```
Algoritmo "Questão2"
Var
  i:inteiro
Inicio
  i<-1
  Para i de 0 até 30 passo 1
    Leia(i)
    Se i%3=0 entao
       Escreva(i,"é múltiplo de 3")
    Fim_Se
  Fim_Para
Fim_Algoritmo  
```
### Exercício 03
Dada uma sequência de números inteiros, calcular a sua soma. 
Por exemplo, para a sequência {12, 17, 4, -6, 8, 0}, o seu programa deve escrever o número 35.

```mermaid
flowchart TD
id1([INICIO]) -->id2>Digite quantos números você quer:]
id2 -->id3[/n/]
id3 -->id4[rep<-0]
id4-->id5[soma<-0]
id5-->id6>Digite um número:]
id6-->id7[/num/]
id7-->id8[soma<-soma+num]
id8-->id9[rep<-rep+1]
id9 -->id10{rep=n}
id10 --LOOP-->id6
id10 --V-->id11>soma é o resultado da soma dos números digitados]
id11-->id([FIM])
```








```
Algoritmo "Lista3_Soma"
// Função :Dada uma sequência de números inteiros, calcular a sua soma
// Autor : Ângelo Mendonça Rodrigues
// Data : 21/03/2024
// Seção de Declarações 
var
  n,num,rep,soma       :inteiro
inicio
  Escreva("Digite quantos números você quer:")
   Leia(n)   //n:quantidade de números 
   rep<-0    //rep:contador de repetições
   soma<-0   //soma:soma dos números digitados
   Repita
      Escreva("Digite um número:")
      Leia(num)  //num:números digitados
      soma<-soma+num
      rep<-rep+1
   ate rep=n
   Escreva(soma, "é o resultado da soma dos números digitados")
// Seção de Comandos
FIM_ALGORITMO
```
    
### Exercício 04
Escreva um programa que leia a nota de diversos alunos, até que seja digitada uma nota negativa. 
Nesse momento, ele mostra a média aritmética de todas as notas lidas e quantas notas foram lidas. 
Ex. Foram lidas 14 notas. A média aritmética é 6.75!

#### Fluxograma

```mermaid
flowchart TD
A([INICIO]) --> B([FIM])
```

#### Pseudocódigo

```
algoritmo "semnome"
Declare nota, media:real quant🇦🇷
INICIO
 media<-0
 quant<-0
 nota<-0
 Escreva("Digite uma nota:")
 Leia(nota)
 Enquanto nota>=0
   quant<--quant+1
   media<-- (media+nota)/quant
 FimEnquanto
 Escreva("A média das notas foi:",media,"e quantidade de notas escritas foi",quant) 
fimalgoritmo
```


```
Algoritmo ClassificaCategoria
FIM_ALGORITMO
```
