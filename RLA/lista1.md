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
Algoritmo "ContaAprovacoes"
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




 
