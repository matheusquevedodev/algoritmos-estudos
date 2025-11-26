🖥️ **Introdução a Arrays**

Os arrays são uma das estruturas de dados mais fundamentais na computação. Eles representam uma coleção ordenada de elementos, geralmente do mesmo tipo, armazenados em posições contíguas de memória. Por serem simples e eficientes, aparecem constantemente em entrevistas, concursos, competições e no LeetCode.

Embora Python não tenha um array clássico como em C ou Java (com tamanho fixo e armazenamento estritamente contínuo), a estrutura mais próxima e amplamente utilizada é a lista (list), que funciona como um array dinâmico — ajustando seu tamanho automaticamente conforme novos elementos são inseridos.

🔹**Por que Arrays são importantes?**

Arrays são a base para diversos algoritmos e técnicas, como:

Two Pointers

Binary Search

Sliding Window

Busca Linear

Prefix Sum

Manipulação de strings

Hashing básico

Além disso, muitos problemas complexos são resolvidos a partir de operações eficientes em arrays.

🔹**Operações comuns em Arrays**

✔ Acessar elementos

Acesso é O(1):
```python
nums = [10, 20, 30, 40]
print(nums[2])  # 30
```

✔ Atualizar valores
```python
nums[1] = 50
print(nums)  # [10, 50, 30, 40]
```
✔ Inserir elementos
```python
nums.append(99)      # adiciona no final
nums.insert(1, 15)   # insere na posição 1
```

✔ Remover elementos
```python
nums.pop()       # remove o último
nums.pop(0)      # remove o primeiro
nums.remove(30)  # remove o valor 30
```

✔ Percorrer um array
```python
for num in nums:
    print(num)
```

🔹 **Criando Arrays em Python**
```python
Array simples
numbers = [1, 2, 3, 4, 5]
```
```python
Array vazio
arr = []
```
```python
Criar array preenchido
zeros = [0] * 5   # [0, 0, 0, 0, 0]
```
```python
Compreensão de listas
squares = [x * x for x in range(1, 6)]
```
🔹 **Como Python armazena Arrays?**

Python utiliza uma estrutura chamada Dynamic Array, que:

mantém elementos contíguos na memória

aumenta de tamanho automaticamente quando necessário

permite inserções rápidas no final (append() é muito eficiente)

Embora exista o módulo array, para algoritmos e problemas de entrevistas usamos listas.

🔹 **Exemplo clássico de problema com arrays (LeetCode)**
```python
Two Sum
def two_sum(nums, target):
    mapa = {}
    for i, n in enumerate(nums):
        complement = target - n
        if complement in mapa:
            return [mapa[complement], i]
        mapa[n] = i

print(two_sum([2, 7, 11, 15], 9))
Saída: [0, 1]
```
🔹**O que estudar nesta seção**

Iteração eficiente

Two Pointers

Sliding Window

Binary Search

Uso combinado de arrays + hash maps

Problemas de soma, diferenças, subarrays

Manipulação de intervalos
