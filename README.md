# Desafio-Final-Portugol-NExt-C.E.S.A.R
Quesões elaboradas para o desafio final da fase preparátoria do NExt C.E.S.A.R
================================================================================
Questão 6
programa
{
	inclua biblioteca Matematica -->mat
	
	funcao inicio()
	{
		real ini
		real meio	
		real fim		
		escreva("Digite o salário: ")
		leia(ini)
		meio = mat.arredondar(ini*1.15, 2)
		fim = mat.arredondar(meio*0.92, 2)
		escreva("Salário inicial:     R$ ",ini, "\n")
		escreva("Salário com aumento: R$ ",meio, "\n")
		escreva("Salário final:       R$ ",fim, "\n")
	}
}
=============================================================================
Questão 7
programa
{

	funcao inicio()
	{

		inteiro vetor_idade[10]
		cadeia  matriz_dados[10][3]
		inteiro maior_letra_a = 0
		inteiro id_letra_a = 0
		inteiro id_letra_b = 0
		vetor_idade[0] = 10
		vetor_idade[1] = 11
		vetor_idade[2] = 12
		vetor_idade[3] = 13
		vetor_idade[4] = 14
		vetor_idade[5] = 15
		vetor_idade[6] = 16
		vetor_idade[7] = 17
		vetor_idade[8] = 18
		vetor_idade[9] = 19
		para (inteiro j = 0; j<=3; j++)
		{
			matriz_dados[j][0] = "masculino"
		}
		para (inteiro j = 4; j<=7; j++)
		{
			matriz_dados[j][0] = "outros"
		}
		para (inteiro j = 8; j<=9; j++)
		{
			matriz_dados[j][0] = "feminino"
		}
		para (inteiro j = 0; j<=3; j++)
		{
			matriz_dados[j][1] = "azuis"
		}
		para (inteiro j = 4; j<=7; j++)
		{
			matriz_dados[j][1] = "verdes"
		}
		para (inteiro j = 8; j<=9; j++)
		{
			matriz_dados[j][1] = "castanhos"
		}
		para (inteiro j = 0; j<=3; j++)
		{
			matriz_dados[j][2] = "loiros"
		}
		para (inteiro j = 4; j<=7; j++)
		{
			matriz_dados[j][2] = "castanhos"
		}
		para (inteiro j = 8; j<=9; j++)
		{
			matriz_dados[j][2] = "pretos"
		}
	para (inteiro r=0; r<=9; r++)
	{
		se (maior_letra_a <= vetor_idade[r])
		{
			maior_letra_a = vetor_idade[r]
			id_letra_a = r+1
		}
		
	}
	escreva("A maior idade entre as pessoas da amostra é ",maior_letra_a," referente ao aluno ",id_letra_a,"\n")
	para (inteiro s=0; s<=9; s++)
	{
		se(matriz_dados[s][0] == "feminino" e matriz_dados[s][1] == "castanhos" e matriz_dados[s][2] == "pretos" e vetor_idade[s] >= 18 e vetor_idade[s] <=35)
		{
			id_letra_b = id_letra_b + 1
		}
	}
  	escreva("A quantidade de feminimos entre 18 e 35 anos com olhos castanhos e cabelos pretos é igual a ", id_letra_b,"\n")
	}
}
=========================================================================================
Questão 8
programa
{
	
	funcao inicio()
	{
		inteiro qestudante
		inteiro i = 1
		cadeia nomes[99]
		inteiro idades[99]
		escreva("Insira a quantidade de estudantes: ")
		leia(qestudante)
		enquanto (i <= qestudante)
		{
			escreva("Digite o nome do ",i,"° estudante:")
			leia(nomes[i])
			escreva("Digite a idade do ",i,"° estudante:")
			leia(idades[i])
			i++
		}
		para (inteiro j=1; j<=qestudante; j++)
		{
			se (idades[j] >= 18)
			{
				escreva("\n",nomes[j],", você está apto(a) a tirar a carteira de motorista.","\n")
			}
			senao
			{
				escreva("\n",nomes[j],", você não está apto(a) a tirar a carteira de motorista.","\n")
			}
		}
	}
}
==================================================================================================
Questão 9
programa
{

	funcao inicio()
	{
		inteiro i = 0
		real soma_idades = 0.0
		real q_estudan = 0.0
		real med
		escreva("Digite as idades dos estudantes do ensino fundamental","\n")
		enquanto (i != -1)
		{
			leia(i)
			se (i == -1)
			{
				pare
			}
			soma_idades = soma_idades + i
			q_estudan = q_estudan + 1
		}
		med = soma_idades/q_estudan
		escreva("Quantidade de estudantes: ",q_estudan,"\n")
		escreva("Média das idades: ",med," anos")
	}
}
=================================================================================
Questao 10
programa
{
	
	funcao inicio()
	{	
		cadeia nomes[5]
		real notas[5]
		real med
		cadeia alunos_aci_media = ""
		real teste
		inteiro cont = 0
		real medi = 0.0
		para (inteiro i = 0; i<5; i++)
		{
			escreva("Escreva o nome do ",i+1,"° estudante: ")
			leia(nomes[i])
			escreva("Escreva a nota do ",i+1,"° estudante: ")
			leia(notas[i])
		}
		para (inteiro i = 0; i < 5; i++)
		{
			medi = medi + notas[i]
		}	
		med = medi/5	
		para (inteiro i = 0; i<5; i++)
		{
 			teste = notas[i] - med
			se (teste >= 0)
			{
				alunos_aci_media = alunos_aci_media + nomes[i] + ", "
				cont = cont + 1
			}
		}
		escreva("Média da turma: ",med,"\n")
		escreva("Estudantes com nota acima da média da turma: ", cont,", nomes: ", alunos_aci_media)
	}
}
==========================================================================================
Questão 11
programa
{
		
	funcao inicio()
	{
		inteiro valorant_1 = 0
		inteiro amongus_2 = 0
		inteiro freefire_3 = 0
		inteiro rust_4 = 0
		inteiro pixelripped1995_5 = 0
		inteiro celeste_6 = 0
		inteiro i = 7
		real total_votos
		real valorant_1_per
		real amongus_2_per
		real freefire_3_per
		real rust_4_per
		real pixelripped1995_5_per
		real celeste_6_per	
		escreva("Digite os votos, conforme o quadro a seguir:")
		enquanto (i != 0)
		{
			leia(i)
			escolha (i)
			{
				caso (1):
					valorant_1 = valorant_1 + 1
					pare
				caso (2):
					amongus_2 = amongus_2 + 1
					pare
				caso (3):
					freefire_3 = freefire_3 + 1
					pare
				caso (4):
					rust_4 = rust_4 + 1
					pare
				caso (5):
					pixelripped1995_5 = pixelripped1995_5 + 1
					pare
				caso(6):
					celeste_6 = celeste_6 + 1
					pare
			}
		}
		total_votos = valorant_1+amongus_2+freefire_3+rust_4+pixelripped1995_5+celeste_6
		valorant_1_per = valorant_1/total_votos*100
		amongus_2_per = amongus_2/total_votos*100
		freefire_3_per = freefire_3/total_votos*100
		rust_4_per = rust_4/total_votos*100
		pixelripped1995_5_per = pixelripped1995_5/total_votos*100
		celeste_6_per = celeste_6/total_votos*100
		escreva("Valorant - votos: ",valorant_1,", ",valorant_1_per,"%","\n")
		escreva("Among Us - votos: ",amongus_2,", ",amongus_2_per,"%","\n")
		escreva("Free Fire - votos: ",freefire_3,", ",freefire_3_per,"%","\n")
		escreva("Rust - votos: ",rust_4,", ",rust_4_per,"%","\n")
		escreva("Pixel Ripped 1995 - votos: ",pixelripped1995_5,", ",pixelripped1995_5_per,"%","\n")
		escreva("Celeste - votos: ",celeste_6,", ",celeste_6_per,"%","\n")
		escreva("Total de votos: ",total_votos,"\n")
    =====================================================================================
    Questão 12
    programa
{
	
	funcao inicio()
	{
		cadeia sintoma
		inteiro selecao
		escreva("Digite o sintoma:")
		leia(sintoma)
		se (sintoma == "azia")
		{
			escreva("sugerimos o medicamento Buxim pelo valor de R$ 2,40","\n")
		}
		senao se (sintoma == "dor de cabeça")
		{
			escreva("sugerimos os medicamentos Cabeçã e Leuza","\n")
			escreva("Digite 1 para selecionar o medicamento Cabeçã e 2 para selecionar Leuza","\n")
			leia(selecao)
			se (selecao == 1)
			{
				escreva("O valor do Cabeçã é R$ 10,50","\n")
			}
			senao se (selecao == 2)
			{
				escreva("O valor do Leuza é R$ 8,20","\n")
			}
			senao
			{
				escreva("A opção escolhida não é válida")
			}	
		}
		senao se (sintoma == "dor muscular")
		{
			escreva("sugerimos os medicamentos - Relashow e Geslado","\n")
			escreva("Digite 1 para selecionar o medicamento Relashow e 2 para selecionar Geslado","\n")
			leia(selecao)
			se (selecao == 1)
			{
				escreva("O valor do Relashow é R$ 8,25","\n")
			}
			senao se (selecao == 2)
			{
				escreva("O valor do  Geslado é R$ 12,80","\n")
			}
			senao
			{
				escreva("A opção escolhida não é válida")
			}	
		}		
		senao se (sintoma == "enjoo")
		{
			escreva("sugerimos os medicamentos - Dramatic e Padentrum","\n")
			escreva("Digite 1 para selecionar o medicamento Dramatic e 2 para selecionar Padentrum","\n")
			leia(selecao)
			se (selecao == 1)
			{
				escreva("O valor do Dramatic é R$ 11,10","\n")
			}
			senao se (selecao == 2)
			{
				escreva("O valor do Padentrum é R$ 15,30","\n")
			}
			senao
			{
				escreva("A opção escolhida não é válida")
			}	
		}
		senao se (sintoma == "gases")
		{
			escreva("sugerimos o medicamento Catapum pelo valor de R$ 5,50","\n")
		}
		senao
		{
			escreva("Para o sintoma apresentado sugerimos que entre em contato com o farmacêutico")
		}
	}
}
