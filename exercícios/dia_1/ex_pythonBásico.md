## Lista de exercícios de Python

1. **Exercício sobre variáveis e operadores lógicos**

Crie uma função chamada `verifica_vogal` que recebe um caractere como parâmetro e retorna True se o caractere for uma vogal e False caso contrário.

2. **Exercício sobre variáveis e operadores lógicos**

Crie uma função chamada `verifica_par_impar` que recebe um número inteiro como parâmetro e retorna "par" se o número for par e "ímpar" caso contrário.

3. **Exercício sobre listas e strings**

Crie uma função chamada `concatena_listas` que recebe duas listas como parâmetros e retorna uma nova lista que contém a concatenação das duas listas.

4. **Exercício sobre listas e strings**

Crie uma função chamada `inverte_palavra` que recebe uma palavra como parâmetro e retorna a palavra invertida.

5. **Exercício sobre listas e strings**

Crie uma função chamada `verifica_palindromo` que recebe uma palavra como parâmetro e retorna True se a palavra for um palíndromo (lida da mesma forma de trás para frente) e False caso contrário.

6. **Exercício sobre dicionários**

Crie uma função chamada `conta_palavras` que recebe uma frase como parâmetro e retorna um dicionário contendo a contagem de cada palavra na frase.

7. **Exercício sobre dicionários**

Crie uma função chamada `calcula_media` que recebe um dicionário contendo as notas de um aluno em diferentes disciplinas e retorna a média das notas.

8. **Exercício sobre if, elif e else**

Crie uma função chamada `verifica_idade` que recebe a idade de uma pessoa como parâmetro e retorna "Maior de idade" se a idade for maior ou igual a 18 e "Menor de idade" caso contrário.

9. **Exercício sobre if, elif e else**

Crie uma função chamada `classifica_triangulo` que recebe três valores inteiros representando os lados de um triângulo e retorna "Equilátero" se todos os lados forem iguais, "Isósceles" se dois lados forem iguais e "Escaleno" caso contrário.

10. **Exercício sobre laço de repetição**

Crie uma função chamada `calcula_fatorial` que recebe um número inteiro positivo como parâmetro e retorna o fatorial desse número.

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>


### Soluções dos exercícios

1. **Exercício sobre variáveis e operadores lógicos**
```python
def verifica_vogal(caractere):
    vogais = ['a', 'e', 'i', 'o', 'u']
    if caractere.lower() in vogais:
        return True
    else:
        return False
```

2. **Exercício sobre variáveis e operadores lógicos**
```python
def verifica_par_impar(numero):
    if numero % 2 == 0:
        return "par"
    else:
        return "ímpar"
```

3. **Exercício sobre listas e strings**
```python
def concatena_listas(lista1, lista2):
    nova_lista = lista1 + lista2
    return nova_lista
```

4. **Exercício sobre listas e strings**
```python
def inverte_palavra(palavra):
    palavra_invertida = palavra[::-1]
    return palavra_invertida
```

5. **Exercício sobre listas e strings**
```python
def verifica_palindromo(palavra):
    palavra = palavra.lower()
    if palavra == palavra[::-1]:
        return True
    else:
        return False
```

6. **Exercício sobre dicionários**
```python
def conta_palavras(frase):
    palavras = frase.split()
    contagem = {}
    for palavra in palavras:
        if palavra in contagem:
            contagem[palavra] += 1
        else:
            contagem[palavra] = 1
    return contagem
```

7. **Exercício sobre dicionários**
```python
def calcula_media(notas):
    total_notas = len(notas)
    soma = sum(notas.values())
    media = soma / total_notas
    return media
```

8. **Exercício sobre if, elif e else**
```python
def verifica_idade(idade):
    if idade >= 18:
        return "Maior de idade"
    else:
        return "Menor de idade"
```

9. **Exercício sobre if, elif e else**
```python
def classifica_triangulo(lado1, lado2, lado3):
    if lado1 == lado2 == lado3:
        return "Equilátero"
    elif lado1 == lado2 or lado1 == lado3 or lado2 == lado3:
        return "Isósceles"
    else:
        return "Escaleno"
```

10. **Exercício sobre laço de repetição**
```python
def calcula_fatorial(numero):
    fatorial = 1
    for i in range(1, numero+1):
        fatorial *= i
    return fatorial
```
