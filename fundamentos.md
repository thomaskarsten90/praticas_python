# 📘 Material de Estudo - Python Básico

## 1. Estruturas de Dados

### 🔹 Listas
- Estruturas **mutáveis** (podem ser alteradas).
- Usadas para armazenar coleções ordenadas.

```python
# Criando uma lista
frutas = ["maçã", "banana", "laranja"]

# Acessando elementos
print(frutas[0])  # maçã
print(frutas[-1]) # laranja

# Alterando
frutas[1] = "uva"

# Adicionando
frutas.append("pera")

# Removendo
frutas.remove("maçã")

print(frutas)
```

### 🔹 Tuplas

- Estruturas imutáveis (não podem ser alteradas).
- Mais rápidas que listas.

```python
# Criando uma tupla
cores = ("vermelho", "azul", "verde")

# Acessando
print(cores[0])  # vermelho

# Não é possível alterar
# cores[0] = "amarelo" -> ERRO
```

### 🔹 Dicionários

- Estrutura chave: valor.
- Muito usada em datasets e JSON.

```python
aluno = {
    "nome": "Maria",
    "idade": 21,
    "curso": "Ciência de Dados"
}

print(aluno["nome"])   # Maria
aluno["idade"] = 22    # Atualiza valor
aluno["nota"] = 9.5    # Adiciona nova chave

print(aluno)
```

### 🔹 Sets (Conjuntos)

- Estrutura não ordenada e sem elementos repetidos.
- Muito útil para eliminar duplicatas.

```python
numeros = {1, 2, 3, 3, 4, 5}
print(numeros)  # {1, 2, 3, 4, 5}

# Operações de conjuntos
a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))        # União -> {1, 2, 3, 4, 5}
print(a.intersection(b)) # Interseção -> {3}
print(a.difference(b))   # Diferença -> {1, 2}
```

## 2. Loops e Condicionais

### 🔹 Condicionais
```python
idade = 18

if idade >= 18:
    print("Maior de idade")
elif idade == 17:
    print("Quase lá!")
else:
    print("Menor de idade")
```

### 🔹 Loops (for e while)

```python
# FOR
for i in range(5):
    print(i)

# WHILE
n = 0
while n < 5:
    print(n)
    n += 1
```

## 3. Funções

- Reutilizam código.
- Podem receber parâmetros e retornar valores.

```python
def soma(a, b):
    return a + b

print(soma(10, 5))  # 15

# Função com valor padrão
def saudacao(nome="visitante"):
    print(f"Olá, {nome}!")

saudacao("Maria")
saudacao()
```

## 4. Compreensão de Listas e Dicionários

### 🔹 List Comprehension

- Forma rápida de criar listas.

```python
# Lista de quadrados
quadrados = [x**2 for x in range(5)]
print(quadrados)  # [0, 1, 4, 9, 16]

# Apenas pares
pares = [x for x in range(10) if x % 2 == 0]
print(pares)  # [0, 2, 4, 6, 8]
```

### 🔹 Dict Comprehension

- Forma rápida de criar dicionários.

```python
# Dicionário {n: n²}
quadrados_dict = {x: x**2 for x in range(5)}
print(quadrados_dict)  # {0:0, 1:1, 2:4, 3:9, 4:16}
```

# ✅ Resumo

- **Listas** = mutáveis, ordenadas.
- **Tuplas** = imutáveis, ordenadas.
- **Dicionários** = pares chave:valor.
- **Sets** = únicos, não ordenados.
- **Loops** controlam repetição.
- **Condicionais** controlam fluxo.
- **Funções** organizam e reutilizam código.
- **Comprehension** = sintaxe curta e eficiente para listas e dicionários.
