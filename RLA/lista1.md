# unifor 
**Disciplina:** raciocínio lógico algoritmico


**EXERCÍCIO 2**


FLUXOGRAMA
```mermaid
flowchart TD
 id1([Inicio]) --> id2>Digite o valor do salário:]
 id2 --> id3[/Si/]
 id3 --> id4{Si<= 500}
 id4 -- NÃO --> id5[Sf= 1.1*Si]
 id4 -- SIM --> id6[Sf= 1.2*Si]
 id5 --> id7>O seu novo salário é: Sf]
 id6 --> id7
 id7 -->id8([Inicio])
```

PSEUDOCÓDIGO
```
Algoritmo "AlgoritmoSalário"
var
      Si, Sf :numérico               //Si: salário inicial e Sf: salário final
inicio
     escreva ("Digite o valor do salário":)
     leia (Si)
     se Si <= 500 entao
        Sf<-- 1.2* Si             // 1.2* Si significa o aumento de 20% do salário inicial        
        escreva ("seu novo salário é:", Sf)
     senao
        Sf<-- 1.1* Si              //1.1* Si significa o aumento de 10% do salário inicial   
        escreva ("seu novo salário é:", Sf)
     fimse
FIM_ALGORITMO
```


**EXERCÍCIO 3**

FLUXOGRAMA
```mermaid
flowchart TD
id1([INICIO]) -->id2>Digite o valor das duas notas:]
id2 --> id3[/n1,n2/]
id3 --> id4[M=n1/2+ n2/2]
id4 --> id5{M>=7}
id5 -- NÃO --> id6>infelizmente, você está reprovado]
id5 -- SIM --> id7>parabéns, você está aprovado]
id6 --> id([FIM])
id7 --> id([FIM])
```

```
Algoritmo "AlgoritmoMédia"
var
  n1,n2, M :numérico
inicio
     escreva ("Digite o valor das duas notas:")
     leia (n1,n2)
     M<--n1/2 + n2/2
     se M>=7 entao
        escreva("parabéns, você está aprovado")
     senão
         escreva("infelizmenre, você está reprovado")
     fimse
 FIM_ALGORITMO
```

**EXERCÍCIO 4**

```mermaid
flowchart TD
id1([INICIO]) --> id2>Digite quantos anos você tem:]
id2 --> id3[/i/]
id3 -- Sim--> id4>Parabéns, você tem idade suficiente para tirar sua CNH]
id3 -- Nao--> id5[I =18-i]
id5 --> id6>Quantos anos faltam para que você possa tirar a sua CNH:I]
id6-->id([FIM])
id4 -->id([FIM])

```




 
