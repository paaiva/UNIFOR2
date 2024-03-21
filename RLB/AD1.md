# UNIFOR
## AD1 de exercicios

### exercício 1 
Dadas duas variáveis, a e b, implemente e teste um algoritmo para trocar os valores atribuídos a elas.
#### peseudocódigo
``` 
ALGORITIMO troca_de_valores
DECLARE a, b, aux: inteiro
INICIO
ESCREVA "Digite o valor de a"			// ler os valores das variaveis
LEIA a
ESCREVA "Digite o valor de b"
LEIA b
ESCREVA "valores iniciais a e b"
a = aux 					// trocando os valor das variáveis 
a = b
b = temp
ESCREVA "Valor após a troca de A é a"		// novos valores das variaveis
ESCREVA "Valor após a troca de B é B"
FIM_ALGORITIMO
```
### exercício 2 
Dado um conjunto n de notas de alunos em um exame, implemente e teste um algoritmo para fazer uma contagem cont do número de alunos que foram aprovados no exame. Será considerado aprovado o aluno que tirar nota 50 ou maior (no intervalo de 0 a 100).
#### pseudocódigo
```
ALGORITIMO contador_de_notas
DECLARE nota : real
	n,  cont_aprovados : inteiro
INICIO
ESCREVA "Digite o numero de alunos"
LEIA n
cont_aprovados = 0
i = 1
ENQUANTO i <= n
	ESCREVA "Obter nota"
	LEIA nota
		SE nota >= 50 and nota <= 10												
			cont_aprovados = cont_aprovados + 1
			ESCREVA "A contagem de aprovados é igual a cont_aprovados"
		SENAO
			i = +1
FIM_ALGORITIMO
```
### exercício 3
Dado um conjunto de n números, implemente e teste um algoritmo para calcular a soma desses números.
Aceite apenas n maior ou igual a zero.
#### pseudocódigo
```
ALGORITIMO soma_numeros
DECLARE soma, num : real
	      n, i : inteiro
INICIO
ESCREVA "Digite a quantidade de números: "
LEIA n
SE n >= 0
	soma = 0
	i = 1
	ENQUANTO i <= n FAÇA
		ESCREVA "Digite um número"
		LEIA num
		soma = soma + num
		i = + 1 
	ESCREVA "soma dos números é soma"
SENAO
	ESCREVA "O valor deve ser maior ou igual a 0"
FIM_SE
FIM_ALGORITIMO
```
### exercício 4
Dado um conjunto de n termos da série, implemente e teste um algoritmo para calcular o valor de S

#### pseudocódigo 
``` 
ALGORITIMO calculo_s
DECLARE numerador
	denominador
	n : inteiro
	s, termo = real
INICIO
ESCREVA "Escreva o numero de termos da série s"
LEIA n
S = 0
PARA i ATE n PASSO 1 FAÇA
	numerador = 2 * i + 1
	denominador = 2 * i + 2
	termo = numerador / denominador
	S += termo
FIM_PARA
ESCREVA "Soma da série s é S
FIM_ALGORITIMO
