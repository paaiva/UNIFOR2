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
```
### exercício 5
Dado um número n, implemente e teste um algoritmo para calcular o fatorial de n (escrito como n!), onde n >= 0.
#### pseudocódigo
```
ALGORITIMO n_fatorial
DECLARE n, i, fator: inteiro
INICIO 
ESCREVA "Digite um numero inteiro não-negativo: "
LEIA n
SE n >= 0
	fator = 1
	i = 1
	PARA i ATE n PASSO 1 FAÇA
		fator = fator * i
	FIM_PARA
	ESCREVA "O fatorial de n é fator"
SENAO 
	ESCREVA "O valor deve ser maior igual a 0!"
FIM_SE
FIM_ALGORITIMO
```
### exercício 6
Gerar e imprimir os n primeiros termos da sequência de Fibonacci, onde n >= 1.
#### pseudocódigo
```
ALGORITIMO fibonacci
DECLARE n, a, b, i, termo_atual : inteiro
INICIO
ESCREVA "Numero de termos da sequência fibonacci"
LEIA n
a = 0
b = 1
i= 1
PARA i ATE n PASSO 1 FAÇA
	termo_atual = a + b
	a = b
	b = termo_atual
FIM_PARA
ESCREVA "termo_atual é o termo atual"
FIM_ALGORITIMO
```
### exercício 7
Implemente e teste um algoritmo para inverter a ordem dos dígitos de um número inteiro positi
#### pseudocódigo
```
DECLARE num, num_inv, digito : inteiro
INICIO
ESCREVA "Digite um número inteiro: "
LEIA num
SE  num >= 0
	num_inv = 0
	ENQUANTO num >= 0 FAÇA
		digito = num % 10
		num_inv = num_inv * 10 + digito
		num = num // 10
	ESCREVA "Numero invertido é num_inv"
SENAO
	ESCREVA "O numero deve ser positivo!"
FIM_SE
FIM_ALGORITIMO
	
