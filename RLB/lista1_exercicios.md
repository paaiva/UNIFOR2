
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

