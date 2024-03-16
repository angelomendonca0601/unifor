# unifor 
**Disciplina:** raciocínio lógico algoritmico
**EXERCÍCIO 1**
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

