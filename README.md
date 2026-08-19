import numpy as np  # Importa a biblioteca NumPy e a apelida de 'np'

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  # Cria uma lista com números de 1 a 10

soma = 0  # Inicializa a variável 'soma' com valor zero

for n in numeros:  # Inicia um loop que percorre cada elemento da lista 'numeros'
    soma += n  # Adiciona o número atual (n) ao valor acumulado na variável 'soma'

media = soma / len(
    numeros
)  # Calcula a média dividindo a soma total pela quantidade de elementos (len)
print("Média feita na mão:", media)  # Exibe o resultado do cálculo manual

array_numeros = np.array(
    numeros
)  # Converte a lista do Python para um array do NumPy
media = np.mean(array_numeros)  # Usa a função nativa do NumPy para calcular a média
print("Média com Numpy:", media)  # Exibe o resultado obtido pelo NumPy
