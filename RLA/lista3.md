### Exercício 01
Atualize o algoritmo para determinar se um número inteiro e positivo é par ou ímpar, usando uma laço condicional para aceitar apenas números maiores ou iguais a zero. 





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
   Se n%1 != 0 entao
       Escreva("Por favor, digite um número inteiro")
   Fimse
   Se n%2=0 entao
      Escreva("O número",n,"é par")
   Senao
      Escreva("O número",n,"é impar")
   FimSe
FIM_ALGORITMO
```

