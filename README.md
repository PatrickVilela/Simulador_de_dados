# Simulador de Dados em Python

## Introdução
O Simulador de Dados é um projeto simples em Python que simula o lançamento de dados. Neste projeto, usamos a biblioteca `random` para gerar números aleatórios que representam os resultados dos lançamentos.

## Como funciona
1. O usuário insere o número de faces do dado.
2. O usuário insere o número de lançamentos desejados.
3. O programa gera resultados aleatórios para os lançamentos.
4. Os resultados são exibidos ao usuário.

## Código
```python
import random

def dice_roller(num_faces, num_rolls):
    results = []
    for _ in range(num_rolls):
        roll_result = random.randint(1, num_faces)
        results.append(roll_result)
    return results

def main():
    num_faces = int(input("Digite o número de faces do dado: "))
    num_rolls = int(input("Digite o número de lançamentos: "))

    results = dice_roller(num_faces, num_rolls)
    print("Resultados dos lançamentos:", results)

if __name__ == "__main__":
    main()

````python

**Exemplo de Uso**

Digite o número de faces do dado: 6
Digite o número de lançamentos: 10
Resultados dos lançamentos: [3, 5, 2, 6, 4, 1, 3, 2, 6, 1]

**Conclusão** 

O Simulador de Dados é um projeto divertido e educativo que mostra como podemos usar Python para criar aplicativos simples, mas úteis. É um ótimo projeto para iniciantes praticarem seus conhecimentos em Python e lógica de programação.


