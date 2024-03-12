# UNIFOR
## Lista 3 de exercicios
### exercicio 1
Faça um algoritmo para determinar se um número inteiro e positivo é par ou ímpar
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
