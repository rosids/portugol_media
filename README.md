# portugol_media
Pequeno programa de cálculo de média

programa
{
	
	funcao inicio()
	{
		real nota1,nota2,nota3,nota4,media,total
		inteiro opcao
		cadeia nome
		escreva("Digite seu nome: ")
		leia(nome)
		escreva("Digite a nota 1: ")
		leia(nota1)
		escreva("Digite a nota 2: ")
		leia(nota2)
		escreva("Digite a nota 3: ")
		leia(nota3)
		escreva("Digite a nota 4: ")
		leia(nota4)

		escreva("Aperte: \n1 - total \n2 - media \n")
		escreva("Sua opção: ")
		leia(opcao)
		
		escolha(opcao){
		caso 1:
		total = nota1+nota2+nota3+nota4
		escreva("O total de suas notas é: " + total + " pontos.")
		pare
		caso 2:
		media = (nota1+nota2+nota3+nota4)/4
		escreva("Sua média é: " + media + " pontos. \n")
		se(media>=7){
			escreva(nome + ", parabéns! Você foi aprovado(a)!")
		}
		senao{
			escreva(nome + ", infelizmente, você foi reprovado(a). ")
		}
		pare
		caso contrario:
		escreva("Escolha uma das opções: \n1 - total \n2 - media \n ")
		}
	}
}
