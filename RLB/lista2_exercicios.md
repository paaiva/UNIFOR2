# Unifor
## Lista 2 de exercicios 
### exercicio 1 
Calcule a média de quatro números inteiros dados.
#### Fluxograma 

```mermaid
flowchart TD
A([Inicio])-->B{{Digite N1, N2, N3, N4}}
B-->C[/N1,N2,N3,N4/]
C-->D[M == N1 + N2 + N3 + N4]
D-->E[MT == M / 4 ]
E-->H[/MT/]
H-->F{{MT é sua media total}}
F-->G([FIM])
```
#### pseudocódigo
```
ALGORITIMO media_4_numeros
DECLARE n1, n2, n3. n4, : inteiro
	m : real
INICIO
ESCREVA "Digite n1"
LEIA n1
ESCREVA "Digite n2"
LEIA n2
ESCREVA "Digite n3"
LEIA n3
ESCREVA "Digite n4"
LEIA n4
m == (n1 + n2 + n3 + n4) / 4 
ESCREVA " media dos números é igual à m"
FIM
FIM_ALGORITIMO
```
#### teste de mesa
| numeros | media | saida |
| -- | -- | -- |
| 10, 8, 4 , 2| 6 | "A media é igual a 6" | 
| 3, 1, 6 , 12| 5.5 |"A media é igual a 5.5" | 
|6, 4, 8, 6 | 6 | "A media é igual a 6" |
|10, 20, 10 , 0| 10 | "A media é igual a 10" |

### exercicio 2 
Leia uma temperatura dada na escala Celsius (C) e imprima o equivalente em Fahrenheit
#### Fluxograma 
``` mermaid 
flowchart TD 
A([Inicio])-->B{{Digite o valor em C}}
B-->C[/C/] 
C-->D[F== 9/5 * C + 32 ]
D-->G[/F/]
G-->E{{F é o valor convertido a fahrenheit}}
E-->F([FIM])
``` 
``` 
ALGORITIMO transformar_celsius_em_fahrenheit
DECLARE c, f: real
INICIO
ESCREVA "Digite o valor em c"
LEIA c
f== (9/5) * c + 32 
ESCREVA " f é o novo valor em fahrenheit"
FIM
FIM_ALGORITIMO
``` 


```

```
### exercício 3 atualizado
Receba dois números reais e um operador e efetue a operação correspondente com os
valores recebidos (operandos). O algoritmo deve retornar o resultado da operação
selecionada simulando todas as operações de uma calculadora simples
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Digite n1, n2}}
B-->C[/n1, n2/]
C-->D{{Digite o operador}}
D-->E[/operador/]
E--ESCOLHA-->F{operador}
F--CASO-->G[operador== +]
G-->H[r== n1 + n2]
H-->I[/r/]
I-->J{{r é o resultado}}
J-->K([FIM])
F--CASO-->L[operador== -]
L-->M[r== n1- n2]
M-->N[/r/]
N-->O{{r é o resultado}}
O-->K
F--CASO-->P[operador== *]
P-->Q[r== m1 * n2]
Q-->R[/r/]
R-->S{{r é o resultado}}
S-->K
F--CASO-->T[operador== %]
T-->U[r==n1 % n2]
U-->V[/r/]
V-->W{{r é o resultado}}
W-->K
```
```
ALGORITIMO calculadora
DECLARE n1, n2, r: real
	operador: caractere 
INICIO
ESCREVA "Digite o primeiro numero"
LEIA n1
ESCREVA "Digite o segundo número"
LEIA n2
ESCREVA "Digite o operador"
LEIA operador
ESCOLHA
	CASO operador == +
             r== n1+n2
	     ESCREVA " r é o resultado"
	CASO operador == *
             r== n1*n2
	     ESCREVA " r é o resultado"
	CASO operador == %
             r== n1%n2
	     ESCREVA " r é o resultado"
	CASO operador == -
             r== n1-n2
	     ESCREVA " r é o resultado"
	SENAO
	     ESCREVA "O operador não é valido"
FIM
FIM_ALGORITIMO
```
### Exercício 4 atualizado
Elaborar um algoritmo que, dada a idade, classifique nas categorias: infantil A (5 - 7 anos),
infantil B (8 -10 anos), juvenil A (11 - 13 anos), juvenil B (14 -17 anos) e adulto (maiores que
18 anos)
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Digite sua idade}}
B-->C[/idade/]
C--ESCOLHA-->D{idade}
D--SENAO-->P{{O jovem não possui grupo definido}}
P-->G
D--CASO-->E[idade >= 5 and idade <= 7]
E-->F{{O jovem pertence ao infantl A}}
F-->G([FIM])
D--CASO-->H[idade >= 8 and idade <= 10]
H-->I{{O jovem pertence ao ifantil B}}
I-->G
D--CASO-->J[idade >= 11 and idade <= 13]
J-->K{{O jovem pertence ao juvenil A}}
K-->G
D--CASO-->L[idade >= 14 and idade <= 17]
L-->M{{O jovem pertence ao juvenil B}}
M-->G
D--CASO-->N[idade >= 18]
N-->O{{pertence ao grupo adulto}}
O-->G
```
```
ALGORÌTIMO grupo_idade
DECLARE idade: inteiro
INICIO
ESCREVA "Digite sua idade"
LEIA idade
ESCOLHA
	CASO idade >= 5 and idade <= 7
	     ESCREVA "O jovem pertence ao ifantil A"
	CASO idade >= 8 and idade <= 10
  	     ESCREVA "O jovem pertence ao infantil B"
	CASO idade >= 11 and idade <= 13
	     ESCREVA "O jovem pertence ao juvenil A"
	CASO idade >= 14 amd idade <= 17
	     ESCREVA "O jovem pertence ao juvenil B"
	CASO idade >= 18
             ESCREVA "pertence ao grupo adulto"
	SENAO
	     ESCREVA "O jovem nao possui grupo definido"
FIM
FIM_ALGORITIMO
```


