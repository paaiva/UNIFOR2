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
#### teste de mesa 
| Número | Número >0 | resto | resto = 0 | saída |
| -- | -- | -- | -- | -- |
| -4 | false | | | "O número deve ser positivo" | 
| 12 | true | 0 | true | "O número é par!" | 
| 27 | true | 1 | false | "O número é ímpar!" | 
| 230 | true | 0 | true | "O número é par!" |
### exercicio 2 
 Faça um algoritmo que exiba na tela uma contagem de 0 até 30, exibindo apenas os
múltiplos de 3.
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B[n==30]
B-->C[soma== 0]
C-->D[i=1 ATÉ n PASSO 1]
D-->E[soma == soma + i]
E-->F{{A contagem é igual à soma}}
F-->G([FIM])
D-->F
E-->D

```
#### pseudocódigo
DECLARE soma, n, i: inteiro
INICIO
i== 3
n== 30
soma == 0
PARA i ATE n PASSO 1 FAÇA
	soma == soma + i
 	ESCREVA "contagem é igual a soma"
FIM_PARA
FIM_ALGORITIMO


### exercício 3
#### Fluxograma
```mermaid
flowchart TD
A([Inicio])-->B{{Insira uma sequência de números inteiros separados por vírgula}}
B-->C[/sequência/]
C-->D{numeros == inteiro}

F--FAÇA-->G{{Insira uma sequência inteira}}
E--ENQUANTO-->F[numeros != inteiro]
D--NAO-->E{{Os numeros devem ser inteiros}}

D--SIM-->H[s == numero + numero + numero...]
H-->I{{A soma é igual a s}}
I-->J([FIM])
G-->C
```
#### pseudocodigo
DECLARE sequencia, r: inteiro
INICIO
ESCREVA "Digite uma sequencia de numeros inteiros separados por virgula"
LEIA sequencia
	ENQUANTO sequência != inteiro FAÇA
 		ESCREVA "Digite uma sequência inteira"
   		LEIA sequência 
r == numero + numero + numero...
ESCREVA "Soma é igual a r"
FIM
FIM_ALGORITIMO

 	
 

