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
a = aux 								// trocando os valor das variáveis 
a = b
b = temp
ESCREVA "Valor após a troca de A é a"	// novos valores das variaveis
ESCREVA "Valor após a troca de B é B"
FIM_ALGORITIMO
```
### exercício 2 
Dado um conjunto n de notas de alunos em um exame, implemente e teste um algoritmo para fazer uma contagem cont do número de alunos que foram aprovados no exame. Será considerado aprovado o aluno que tirar nota 50 ou maior (no intervalo de 0 a 100).
### pseudocódigo
```
ALGORITIMO contador_de_notas
DECLARE nota, notas: real
	          cont_aprovados : inteiro
INICIO
cont_aprovados = 0
ESCREVA "Obter nota"
LEIA nota 
PARA nota ATE notas PASSO 1 FAÇA
	SE nota >= 50 and nota <= 100
		cont_aprovados = cont_aprovados + 1
		ESCREVA "A contagem de aprovados é igual a cont_aprovados"
	FIM_SE
FIM_ALGORITIMO
```

