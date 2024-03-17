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
#### teste de mesa 
| valor em C | valor em Fahrenheit | saída |
| -- | -- | -- |
| 25 | 77 | "O valor convertido para fahrenheit é de 77 F " |
| 18 | 64.4 | "O valor convertido para fahrenheit é de 64.4 F" |
| 28| 82.4 | "O valor convertido para fahrenheit é de 82.4 F " | 
| 21 | 69.8 | "O valor convertido para fahrenheit é de 69.8 F" | 

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
E-->F{operador == +}

F--FALSE-->G{operador ==-}
G--FALSE-->H{operador ==%}
H--FALSE-->I{operador ==*}
I--FALSE-->W{{O operador não é valido}}
W-->M
I--TRUE-->T[r == n1*n2]
T-->U[/r/]
U==>V{{r é o seu resultado}}
V-->M


F--TRUE-->J[r == n1 + n2]
J-->K[/r/]
K-->L{{r é o seu resultado}}
L-->M([FIM])
G--TRUE-->N[r == n1 - n2]
N-->O[/r/]
O-->P{{r é o seu resultado}}
P-->M
H--TRUE-->Q[r== n1 % n2]
Q-->R[/r/]
R-->S{{r é o seu resultado}}
S-->M

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
#### teste de mesa 
| Insira n1, n2 | Insira o operador | operador é válido | resultado |
| -- | -- | -- | -- |
| 4, 6 | + | true | 10 | 
| 9, 3 | - | true | 6 | 
| 10, 5 | % | true | 2 | 
| 12, 2 | . | false | | 
### Exercício 4 atualizado
Elaborar um algoritmo que, dada a idade, classifique nas categorias: infantil A (5 - 7 anos),
infantil B (8 -10 anos), juvenil A (11 - 13 anos), juvenil B (14 -17 anos) e adulto (maiores que
18 anos)
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Digite sua idade}}
B-->C[/idade/]
C---->D{idade >= 5 and idade <= 7}

D--FALSE-->G{idade >= 8 and idade <= 10}

G--FALSE -->I{idade >= 11 and idade <= 13}

I--FALSE-->K{idade>= 14 and idade <=  17}

K--FALSE-->M{idade >= 18}

M--FALSE-->O{{O jovem nao possui grupo definido}}
O-->F
D--TRUE-->E{{O jovem pertence ao infantil A}}
E-->F([FIM])
G--TRUE-->H{{O jovem pertence ao infantil B}}
H-->F
I--TRUE-->J{{O jovem pertence ao juvenil A}}
J-->F

K--TRUE-->L{{O jovem pertence ao juvenil B}}
L-->F
M--TRUE-->N{{pertence ao grupo adulto}}
N-->F
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
#### teste de mesa
| Idade | idade < 5 | 5=<idade<=7 | 8<=idade<=10 | 11<=idade<=13 | 14<=idade<=17| idade>=18 | saída |
| -- | -- | -- | -- | -- | -- | -- | -- |
| 10 | false | false | true | false | false | false | "O jovempertence ao infantil B" | 
| 3 | true | false | false | false | false | false | "O jovem não possui grupo definido" | 
| 12 | false | false | false | true | false | false | "O jovem pertence ao grupo juvenil A" | 
| 25 | false | false | false | false | false | true | "Pertence ao grupo adulto" | 

