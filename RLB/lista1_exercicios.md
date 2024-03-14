
# UNIFOR
**DICIPLINA:** raciocinio logico algoritimo
**Orientador:** Prof. Ricardo Carubbi
## Lista 1 exercicio
### exercicio 1
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um número inteiro e positivo é par ou impar.
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Digite um número: }}
B-->C[/número/]
C-->D{número > 0}
D--NÃO-->J{{O numero deve ser positivo}}
J--ENQUANTO-->K{{O número for < 0}}
K--FAÇA-->L{{Digite um número positivo: }}
L-->C
D--SIM-->E[resto == numero / 2]
E-->F{resto == 0}
F--SIM-->G{{O número é par}}
F--NÃO-->H{{O número é ímpar}}
G-->I([FIM])
H-->I
```
``` 
ALGORITIMO impar_par
DECLARE n, r: inteiro 
INICIO
	ESCREVA "Digite um número"
	LEIA n
	ENQUANTO n<0 FAÇA
		ESCREVA "Digite um número positivo: "
		LEIA n
	r == n / 2
		SE r == 0
			ESCREVA "O número é par"
		SENAO
			ESCREVA "O número é impar"
FIM
FIM_ALGORITIMO
```
|LISTA|LISTA|LISTA |teste|
 |teste|teset|teste|teste|


### exercicio 4
 Represente, em fluxograma e pseudocódigo, um algoritmo que, a partir da idade do
candidato(a), determinar se pode ou não tirar a CNH. Caso não atender a restrição de idade,
calcular quantos anos faltam para o candidato estar apto.
#### Fluxograma

```mermaid
flowchart TD
A([Inicio])-->B{{Digite sua Idade}}
B-->C{Idade >= 18}
C--SIM-->D{{Pode tirar CNH!}}
D-->E([FIM])
C--NAO-->F[18 - Idade == X]
F-->G{{Nao pode tirar CNH, faltam X anos!}}
G-->E
```

```
ALGORITIMO tirar_CNH
DECLARE idade NUMERICO
ESCREVA "Digite sua idade"
LEIA idade
SE idade >= 18
	ESCREVA "Pode tirar CNH!"

SENAO
	X = 18 - idade
	ESCREVA "Nao pode tirar CNH! Faltam X anos"

FIM_ALGORITIMO
	
```


### exercicio 1 
Represente, em fluxograma e pseudocódigo, um algoritmo para calcular a média aritmética
entre duas notas de um aluno e mostrar sua situação, que pode ser aprovado ou reprovado.
#### Fluxograma
``` mermaid
flowchart TD
A([inicio])-->B{{Digite N1, N2}}
B-->C[/N1, N2/]
C-->D[Media == N1 + N2 / 2]
D-->E{Media>=7}
E--SIM-->F{{Aprovado!}}
F-->H([FIM])
E--NAO-->G{{Reprovado}}
G-->H

``` 

```
ALGORITIMO media_aritimetica
DECLARE x NUMERICO
DECLARE y NUMERICO
ESCREVA "Escreva nota 1 "
ESCREVA "Escreva nota 2"
LEIA x
LEIA  y 
SE x + y / 2 >= 7
	ESCREVA "Aprovado!"

SENAO
	ESCREVA "Reprovado!"

FIM_ALGORITIMO
```
### exercicio 2
Represente, em fluxograma e pseudocódigo, um algoritmo para calcular o novo salário de um
funcionário. Sabe-se que os funcionários que recebem atualmente salário de até R$ 500 terão
aumento de 20%; os demais terão aumento de 10%.
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Digite seu salario}}
B-->C[/Salario/]
C-->D{Salario <= 500}
D--SIM-->E[Salario x 1,20]
E-->F[/Novo salario/]
F-->G([FIM])
D--NAO-->H[Salario x 1,10]
H-->I[/Novo Salario/]
I-->G
```

```
ALGORITIMO novo_salario
DECLARE salario NUMERICO
ESCREVA "Digite seu salario"
LEIA salario
SE salario <=500
	novo salario == salario x 1,20
	ESCREVA "Este e seu novo salario!"
	
SENAO
	novo salario == salario x 1,10
	ESCREVA "Este e seu novo salario!"

FIM_ALGORITIMO
```

