# Interseção de dois conjuntos-A-e-B
# Verificar a interseção de dois conjuntos A e B

import os
os.system('cls')

print('Vamos trabalhar com a interseção de dois conjuntos, A e B.')
tamanho_a = int(input('Quantos elementos tem o conjunto A? '))
contador = 0

while contador < tamanho_a:
    conjunto_a = []
    for lista_a in range(tamanho_a):
        lista_a = int(input('Forneça um elemento para o conjunto A: '))
        conjunto_a.append(lista_a)
        contador = contador + 1
        print(conjunto_a)

tamanho_b = int(input('Quantos elementos tem o conjunto B? '))
contador_b = 0

while contador_b < tamanho_a:
    conjunto_b = []
    for lista_b in range(tamanho_b):
        lista_b = int(input('Forneça um elemento para o conjunto B: '))
        conjunto_b.append(lista_b)
        contador_b = contador_b + 1
        print(conjunto_b)


print('='*80)
print('O conjunto A é:', conjunto_a, 'e o conjunto B é:', conjunto_b)
print('='*80)

inter = set(conjunto_a).intersection(set(conjunto_b))
print('='*80)

if len(inter) == 0:
    print('Não há interseção entre os conjuntos apresentados! ')
else:
    print('A interseção dos cojuntos A e B é:', inter)
print('='*80)    
print()
