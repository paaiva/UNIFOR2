
# UNIFOR
**DICIPLINA:** raciocinio logico algoritimo
**Orientador:** Prof. Ricardo Carubbi
## Lista 1 exercicio
### exercicio 3
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um número inteiro e positivo é par ou impar.
#### Fluxograma

```mermaid
flowchart TD
A([INICIO])-->B{{Digite um numero:}}
B --> C[/numero/]
C --> D{numero>0}
D --NAO--> E{{O numero deve ser positivo!}}
E --> J([FIM])
D --SIM--> F[resto = numero % 2]
F --> G{resto == 0}
G --NAO--> H{{O numero e impar}}
G --SIM--> I{{O numero e par}}
H --> J
I --> J
```

```
ALGORITIMO verifica_par_impar
DECLARE numero, resto INTEIRO
ESCREVA "Digite um numero"
LEIA numero
SE numero > 0 ENTAO
	resto = numero % 2
	SE resto == 0 ENTAO
		ESCREVA "O numero e par!"
	SENAO
		ESCREVA "O numero e impar!"
SENAO
	ESCREVA "O numero deve ser positivo"
FIM_ALGORITIMO
	
```
