Função MultiplicacaoDeMatrizes(matrizA, matrizB):
    # Verifica se o número de colunas de matrizA é igual ao número de linhas de matrizB
    Se tamanho(matrizA[0]) ≠ tamanho(matrizB) então:
        Retornar "As matrizes não podem ser multiplicadas. O número de colunas de matrizA não é igual ao número de linhas de matrizB."
    Senão:
        linhasA <- tamanho(matrizA)
        colunasA <- tamanho(matrizA[0])
        colunasB <- tamanho(matrizB[0])
        
        matrizResultado <- novaMatriz(linhasA, colunasB)
        
        # Loop para percorrer cada elemento da matriz resultado
        Para i de 0 até linhasA-1 faça:
            Para j de 0 até colunasB-1 faça:
                elemento <- 0
                Para k de 0 até colunasA-1 faça:
                    elemento <- elemento + matrizA[i][k] * matrizB[k][j]
                matrizResultado[i][j] <- elemento
        
        Retornar matrizResultado

# Exemplo de uso da função
matrizA <- [[1, 2, 3], [4, 5, 6]]
matrizB <- [[7, 8], [9, 10], [11, 12]]

matrizMultiplicacao <- MultiplicacaoDeMatrizes(matrizA, matrizB)
Escrever("Resultado da multiplicação das matrizes:")
ImprimirMatriz(matrizMultiplicacao)
