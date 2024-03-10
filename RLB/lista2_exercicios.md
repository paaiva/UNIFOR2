# Unifor
## Lista 2 de exercicios 
### exercicio 1 
Calcule a média de quatro números inteiros dados.
#### Fluxograma 

```mermaid
flowchart TD
A([Inicio])-->B{{Digite N1, N2, N3, N4}}
B-->C[/N1,N2,N3,N4/]
C-->D[N1 + N2 + N3 + N4 == M]
D-->E[M / 4 == MT]
E-->F{{MT é sua media total}}
F-->G([FIM])
```
```
ALGORITIMO media_4_numeros
DECLARE n1, n2, n3. n4, media NUMERICOS 
INICIO
	ESCREVA "Digite n1"
	LEIA n1
	ESCREVA "Digite n2"
	LEIA n2
	ESCREVA "Digite n3"
	LEIA n3
	ESCREVA "Digite n4"
	LEIA n4
	media == (n1 + n2 + n3 + n4) / 4 
	ESCREVA " media dos números ==M"
FIM
FIM_ALGORITIMO
```
### exercicio 2 
Leia uma temperatura dada na escala Celsius (C) e imprima o equivalente em Fahrenheit
#### Fluxograma 
``` mermaid 
flowchart TD 
A([Inicio])-->B{{Digite o valor em C}}
B-->C[/C/] 
C-->D[F== 9/5 * C + 32 ]
D-->E{{F é o valor convertido a fahrenheit}}
E-->F([FIM])
``` 
``` 
ALGORITIMO transformar_celsius_em_fahrenheit
DECLARE c, f NUMERICO
INICIO
	ESCREVA "Digite o valor em c"
	LEIA c
	f== (9/5) * c + 32 
	ESCREVA " f é o novo valor em fahrenheit"
FIM
FIM_ALGORITIMO
``` 
### exercício 3
Leia uma quantidade de chuva dada em polegadas e imprima o equivalente em milímetros
#### Fluxograma 
```  mermaid
flowchart TD 
A([Inicio])-->B{{Insira a quantidade de chuva em polegadas }}
B-->C[polegadas == p]
C-->D[25.4 * P == mm]
D-->E{{mm é a quantidade em milimetros de chuva}}
E-->F([FIM])
```
```
ALGORITIMO polegadas_para_milimetros
DECLARE polegadas NUMERICO
INICIO 
	ESCREVA "insira a quantidade em polegadas"
	LEIA polegadas 
	polegadas * 25.4 == NQ
	ESCREVA "NQ é a quantidade de chuva em milimetros" 
FIM
FIM_ALGORITIMO
```
		
