<details>
<summary> Introdução ao Python </summary>

## Introdução ao Python

Parte deste capítulo é baseado nos Tutoriais de Geek Girls Carrots (https://github.com/ggcarrots/django-carrots).

## Capítulo 1: Interpretador Python

Para começar a brincar com Python, precisamos abrir uma linha de comando no seu computador. Você já deve saber como fazer isso - você aprendeu isso no capítulo anterior. Assim que estiver pronto(a), siga as instruções abaixo.

### Interpretador Python

Abra o Python no terminal digitando `python3` e pressione Enter.

```shell
$ python3
Python 3.6.5 (...)
Type "copyright", "credits" or "license" for more information.
>>>
```

### Seu primeiro comando Python!

Depois de executar o comando Python, o prompt mudou para `>>>`. Isso significa que agora podemos digitar comandos em Python. Você não precisa digitar `>>>` - o Python fará isso por você. Se você deseja sair do console do Python, basta digitar `exit()` ou usar o atalho Ctrl + D no Mac/Linux. Agora, vamos explorar o interpretador Python.

Digite uma operação matemática simples, como `2 + 3`, e pressione Enter.

```python
>>> 2 + 3
5
```

> Incrível! A resposta é exibida imediatamente. O Python é capaz de realizar cálculos matemáticos. Experimente outras operações, como `4 * 5`, `5 - 1` e `40 / 2`. Divirta-se com isso por um tempo e depois continue.

</details>

<details>
<summary> Capítulo 2: Strings </summary>

## Capítulo 2: Strings

Vamos trabalhar com strings, que são sequências de caracteres processadas pelo computador.

### Criando strings

Digite seu primeiro nome entre aspas para criar uma string.

```python
>>> "Olá"
'Olá'
```

Parabéns! Você criou sua primeira string. As strings são delimitadas por aspas duplas ("") ou simples (''), e indicam ao Python que o conteúdo entre as aspas é uma string.

### Manipulando strings

As strings podem ser concatenadas usando o operador `+`.

```python
>>> "Oi " + "Olá"
'Oi Olá'
```

Você também pode multiplicar strings por um número.

```python
>>> "Olá" * 3
'OláOláOlá'
```

Para incluir um apóstrofo dentro de uma string, você pode usar aspas duplas ou escapar o apóstrofo com uma barra invertida (\).

```python
>>> "Foi a gota d'água"
'Foi a gota d'água'

>>> 'Foi a gota d\'água'
'Foi a gota d'água'
```

### Funções de string

Existem várias funções disponíveis para manipular strings. Por exemplo, a função `upper()` converte uma string em letras maiúsculas.

```python
>>> "Olá".upper()
'OLÁ'
```

A função `len()` retorna o comprimento de uma string.

```python
>>> len("Olá")
3
```

Observe que algumas vezes você chama funções com um ponto no final da string, como `"Olá".upper()`, enquanto outras vezes você coloca a string entre parênteses antes de chamar a função, como `len("Olá")`. Isso ocorre porque algumas funções são métodos de

 objetos específicos, como `upper()`, que só pode ser usada em strings. Em outros casos, as funções podem ser aplicadas a diferentes tipos de objetos, como `len()`, que pode ser usada em várias situações. Agora que você aprendeu o básico sobre strings, vamos recapitular:

</details>

<details>
<summary> Capítulo 3: Erros </summary>

## Capítulo 3: Erros

Vamos explorar erros em Python e como lidar com eles.

### Lidando com erros

Vamos tentar encontrar o tamanho de um número usando a função `len()`, da mesma forma que fizemos com uma string. Digite `len(304023)` e pressione Enter.

```python
>>> len(304023)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: object of type 'int' has no len()
```

Obtemos nosso primeiro erro! O erro indica que objetos do tipo 'int' (números inteiros) não possuem um comprimento. O que podemos fazer agora? Podemos converter o número em uma string usando a função `str()`.

```python
>>> len(str(304023))
6
```

Funcionou! Ao usar a função `str()`, convertemos o número em uma string antes de chamar a função `len()`.

### Importante

Lembre-se de que é possível converter números em texto, mas nem sempre é possível converter texto em números. Por exemplo, `int('hello')` não faz sentido, pois a string "hello" não representa um número. No entanto, é possível converter a string '300' em um número inteiro usando `int('300')`.

Agora que você aprendeu sobre erros em Python, vamos continuar com mais um tópico importante:

</details>

<details>
<summary> Capítulo 4: Variáveis </summary>

## Capítulo 4: Variáveis

As variáveis são usadas para armazenar dados e dar-lhes um nome significativo. Elas são úteis para tornar o código mais legível e evitar a necessidade de lembrar constantemente o que as coisas significam.

### Criando variáveis

Vamos criar uma variável chamada `nome`.

```python
>>> nome = "Olá"
```

Ótimo! Agora você possui uma variável chamada `nome` com o valor "Olá". Para verificar o conteúdo da variável, basta digitar o nome da variável.

```python
>>> nome
'Olá'
```

Você também pode alterar o valor da variável atribuindo um novo valor a ela.

```python
>>> nome = "Sonja"
>>> nome
'Sonja'
```

As variáveis podem ser usadas em funções também. Por exemplo, podemos obter o comprimento do nome usando a função `len()`.

```python
>>> len(nome)
5
```

As variáveis podem armazenar não apenas strings, mas também números. Experimente atribuir valores numéricos às variáveis e realizar operações com elas.

```python
>>> a = 4
>>> b = 6
>>> a * b
24
```

Caso você digite o nome de uma variável incorretamente, você receberá um erro de "NameError". Verifique se digitou corretamente o nome da variável.

Agora que você aprendeu sobre variáveis, strings, erros e outras noções básicas de Python, você está pronto(a) para avançar para os próximos capítulos. Divirta-se explorando e praticando mais conceitos de programação em Python!
</details>

<details>
<summary> Capítulo 4: Variáveis </summary>

## Capítulo 5: A função print

A função `print` é utilizada para exibir informações na saída do programa. Ela permite mostrar o conteúdo de variáveis, mensagens personalizadas e outros dados. Vamos ver como utilizá-la.

**Tente isso:**

```python
>>> nome = 'Maria'
>>> nome
'Maria'
>>> print(nome)
Maria
```

Quando você digita apenas `nome`, o interpretador Python exibe a representação em forma de string da variável `nome`, que são as letras M-a-r-i-a, entre aspas simples. Porém, quando você usa `print(nome)`, o Python imprime o conteúdo da variável na tela, sem as aspas, o que resulta em uma exibição mais pura.

A função `print()` também é útil quando desejamos exibir algo dentro de funções ou quando queremos mostrar informações em várias linhas.

</details>

<details>
<summary> Capítulo 6: Listas </summary>

## Capítulo 6: Listas

Além de strings e números inteiros, o Python oferece outros tipos de objetos. Um deles é a lista. As listas são estruturas de dados que permitem armazenar coleções de itens de forma ordenada. Vamos aprender como criar e manipular listas em Python.

**Criando uma lista:**

```python
>>> lista_vazia = []
>>> lista_vazia
[]
```

Acabamos de criar uma lista vazia. Não é muito empolgante, não é mesmo? Vamos criar uma lista dos números da loteria. Para evitar repetir o código o tempo todo, vamos armazenar essa lista em uma variável.

```python
>>> numeros_loteria = [3, 42, 12, 19, 30, 59]
```

Pronto! Agora temos uma lista com números da loteria. O que podemos fazer com ela? Vamos verificar quantos números há nessa lista. Você sabe qual função deve usar para isso. Acho que já aprendemos sobre ela!

```python
>>> len(numeros_loteria)
6
```

Sim! A função `len()` retorna o número de objetos em uma lista. É muito útil, não acha? Vamos organizar essa lista em ordem crescente.

```python
>>> numeros_loteria.sort()
```

Isso não retorna nada, apenas altera a ordem dos números na lista. Vamos imprimir a lista novamente e ver o que acontece.

```python
>>> print(numeros_loteria)
[3, 12, 19, 30, 42, 59]
```

Como você pode ver, os números na nossa lista estão agora em ordem crescente, do menor para o maior. Parabéns! E se quisermos inverter essa ordem? Vamos fazer isso!

```python
>>> numeros_loteria.reverse()
>>> print(numeros_loteria)
[59, 42, 30, 19, 12, 3]
```

Fácil, não é mesmo? Se quisermos adicionar algo à nossa lista, podemos fazer isso usando o método `append()`.

```python
>>> numeros_loteria.append(199)
>>> print(numeros_loteria)
[59, 42, 30, 19, 12, 3, 199]
```

Se quisermos mostrar apenas o primeiro número da lista, podemos usar índices. Um índice é um número que indica a posição de um item na lista. No Python, a contagem começa em 0, então o primeiro

 objeto tem índice 0, o segundo tem índice 1 e assim por diante. Experimente:

```python
>>> print(numeros_loteria[0])
59
>>> print(numeros_loteria[1])
42
```

Como você pode ver, podemos acessar diferentes objetos em nossa lista usando o nome da lista seguido pelo índice do objeto entre colchetes.

Por diversão extra, experimente outros índices, como 6, 7, 1000, -1, -6 ou -1000. Veja se consegue prever o resultado antes de executar o comando. Os resultados fazem sentido?

Você pode encontrar uma lista de todos os métodos disponíveis para listas na documentação do Python: [https://docs.python.org/3/tutorial/datastructures.html](https://docs.python.org/3/tutorial/datastructures.html)

</details>

<details>
<summary> Capítulo 7: Dicionários </summary>

## Capítulo 7: Dicionários

Um dicionário é semelhante a uma lista, mas em vez de acessar os valores através de um índice, você pode acessá-los por meio de uma chave. Uma chave pode ser uma string ou um número. Vamos aprender como criar e usar dicionários em Python.

**Criando um dicionário vazio:**

```python
>>> dicionario_vazio = {}
>>> dicionario_vazio
{}
```

Acabamos de criar um dicionário vazio. Uau!

Agora, vamos criar um dicionário com algumas informações pessoais (fique à vontade para substituir com suas próprias informações).

```python
>>> participante = {'nome': 'Ola', 'pais': 'Polonia', 'numeros_favoritos': [7, 42, 92]}
```

Com esse comando, criamos uma variável chamada `participante` que contém três pares de chave-valor:

- A chave `'nome'` aponta para o valor `'Ola'` (uma string).
- A chave `'pais'` aponta para o valor `'Polonia'` (outra string).
- A chave `'numeros_favoritos'` aponta para o valor `[7, 42, 92]` (uma lista com três números).

Podemos verificar o conteúdo de chaves individuais usando o comando:

```python
>>> print(participante['nome'])
Ola
```

Como você pode ver, é semelhante a acessar elementos em uma lista. No entanto, em vez de lembrar o índice, usamos o nome da chave.

O que acontece se pedirmos ao Python o valor de uma chave que não existe? Você consegue adivinhar? Vamos tentar e descobrir!

```python
>>> participante['idade']
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
KeyError: 'idade'
```

Olha só, outro erro! Desta vez é um `KeyError`. O Python é muito prestativo e nos informa que a chave `'idade'` não existe nesse dicionário.

Quando devemos usar uma lista e quando devemos usar um dicionário? Bem, é um bom ponto para refletir. Pense em uma solução antes de ver a resposta na próxima linha.

- Se precisamos de uma sequência ordenada de itens, usamos uma lista.
- Se precisamos associar valores a chaves e queremos pesquisar esses valores de forma eficiente (por meio das chaves), usamos um dicionário.

Assim como

 as listas, os dicionários são mutáveis, o que significa que podemos modificá-los depois de criados. Podemos adicionar novos pares de chave-valor ao dicionário após sua criação. Por exemplo:

```python
>>> participante['linguagem_favorita'] = 'Python'
```

Assim como com as listas, podemos usar a função `len()` para obter o número de pares chave-valor no dicionário. Vamos experimentar:

```python
>>> len(participante)
4
```

Espero que tudo esteja fazendo sentido até agora. :)

Pronto para mais diversão com dicionários? Continue lendo para descobrir coisas incríveis!

Podemos usar o método `pop()` para excluir um item do dicionário. Por exemplo, se quisermos excluir a entrada correspondente à chave `'numeros_favoritos'`, podemos usar o seguinte comando:

```python
>>> participante.pop('numeros_favoritos')
>>> participante
{'pais': 'Polonia', 'linguagem_favorita': 'Python', 'nome': 'Ola'}
```

Como você pode ver no resultado, o par chave-valor correspondente à chave `'numeros_favoritos'` foi removido.

Além disso, podemos alterar o valor associado a uma chave já existente no dicionário. Experimente:

```python
>>> participante['pais'] = 'Alemanha'
>>> participante
{'pais': 'Alemanha', 'linguagem_favorita': 'Python', 'nome': 'Ola'}
```

Como você pode ver, o valor da chave `'pais'` foi alterado de `'Polonia'` para `'Alemanha'`. Emocionante, não é?

Uau! Você acabou de aprender mais uma coisa incrível.

**Resumo até agora**

Incrível! Agora você sabe muito sobre programação. Nesta última parte, você aprendeu sobre:

- Erros: agora você sabe como ler e entender erros que aparecem quando o Python não entende um comando que você digitou.
- Variáveis: nomes para objetos que facilitam a programação e tornam o código mais legível.
- Listas: coleções de objetos armazenados em uma ordem específica.
- Dicionários: objetos armazenados como pares chave-valor.

Está empolgado para o próximo passo? :)

</details>

<details>
<summary> Capítulo 8: Listas </summary>

## Capítulo 8: Fazendo comparações

Grande parte da programação consiste em comparar coisas. O que é mais fácil de comparar? Números, é claro. Vamos ver como isso funciona:

```python
>>> 5 > 2
True
>>> 3 < 1
False
>>> 5 > 2 * 2
True
>>> 1 == 1
True
>>> 5 != 2
True
```

Demos ao Python alguns números para comparar. Legal, hein?

Você está se perguntando por que colocamos dois sinais de igual `==` lado a lado para comparar se os números são iguais? Nós usamos um único `=` para atribuir valores a variáveis.

Você sempre, sempre precisa colocar dois `==` se quiser verificar se as coisas são iguais. Também é possível afirmar que as coisas são diferentes entre si. Para isso, usamos o símbolo `!=`, conforme mostrado no exemplo acima.

Dê ao Python mais duas tarefas:

```python
>>> 6 >= 12 / 2
True
>>> 3 <= 2
False
```

`>` e `<` são fáceis, mas o que `>=` e `<=` significam?

Leia eles da seguinte forma:
- `x > y` significa: x é maior que y
- `x < y` significa: x é menor que y
- `x <= y` significa: x é menor ou igual a y
- `x >= y` significa: x é maior ou igual a y

Fantástico! Vamos brincar mais um pouco? Tente isto:

```python
>>> 6 > 2 and 2 < 3
True
>>> 3 > 2 and 2 < 1
False
>>> 3 > 2 or 2 < 1
True
```

Você pode dar ao Python quantos números para comparar quanto você quiser, e ele vai te dar uma resposta! Espertinho, certo?

- `and`: se você usar o operador `and`, ambas as comparações terão que ser verdadeiras para que todo o comando seja verdadeiro.
- `or`: se você usar o operador `or`, apenas uma das comparações precisa ser verdadeira para que o comando todo seja verdadeiro.

Já ouviu a expressão "comparar maçãs com laranjas"? Vamos tentar o equivalente em Python:

```python
>>> 1 > 'django'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unorderable types: int() > str()
```

Aqui vemos que assim como na expressão, Python não é capaz de comparar um número (`int`) e uma string (`str`). Em vez disso, ele mostrou um `TypeError` e nos disse que os dois tipos não podem ser comparados juntos.

Mas como o Python entende verdadeiro e falso? Vamos para a próxima parte! :)

</details>

<details>
<summary> Capítulo 9: Booleanos </summary>

## Capítulo 9: Booleanos

Acidentalmente, você aprendeu sobre um novo tipo de objeto em Python. É chamado de booleano -- e provavelmente o tipo mais fácil que existe.

Existem apenas dois objetos booleanos:

- `True` (verdadeiro)
- `False` (falso)

Mas para o Python entender isso, você precisa sempre escrever `True` (primeira letra maiúscula, com o resto das letras em min

úsculo). `true`, `TRUE`, `tRUE` não vai funcionar -- só `True` é correto. (O mesmo se aplica ao `False`, claro.)

Booleanos podem ser variáveis também! Veja:

```python
>>> a = True
>>> a
True
```

Você também pode fazer desse jeito:

```python
>>> a = 2 > 5
>>> a
False
```

Pratique e divirta-se com os valores booleanos, tentando executar os seguintes comandos:

```python
True and True
False and True
True or 1 == 1
1 != 2
```

Parabéns! Booleanos são um dos recursos mais interessantes na programação, e você acabou de aprender como usá-los!

</details>

<details>
<summary> Capítulo 10: Salve o código </summary>

## Capítulo 10: Salve o código

Até agora nós escrevemos todo nosso código em um interpretador Python, que nos limita a uma linha de código em um momento. Programas normais são salvos em arquivos e executados pelo nosso interpretador de linguagem de programação ou compilador.

Até agora só executamos nossos programas de uma linha de cada vez no interpretador Python. Nós vamos precisar de mais de uma linha de código para as próximas tarefas, então precisaremos rapidamente:

1. Sair do interpretador Python
2. Abrir o editor de código
3. Salvar algum código em um novo arquivo Python
4. Executá-lo!

Para sair do interpretador Python que estamos usando, simplesmente digite a função `exit()`:

```python
>>> exit()
$
```

Isso vai colocá-la(o) no prompt de comando.

Agora vá até a pasta de exercícios e clique no arquivo `python_intro.py` e salvá-lo. Podemos nomear o arquivo de tudo o que quisermos, o importante aqui é ter certeza que o arquivo termina com `.py`, isto diz ao nosso computador que é um arquivo executável de Python e Python pode executá-lo.

Agora você pode escrever seu programa:

```python
print('Olá, AfroPython!')
```

Nota: Você deve observar que uma das coisas mais legais sobre editores de código: cores! No console do Python, tudo era da mesma cor, mas agora você deve ver que a função de `print` é uma cor diferente da sequência de caracteres no seu interior. Isso é chamado de "realce de sintaxe", e é uma ajuda muito útil quando está programando. Perceba a cor das coisas e você vai obter uma dica para quando você esquecer de fechar uma sequência de caracteres, ou fazer um erro de digitação em um nome de palavra-chave (como `def` em uma função, que veremos abaixo). Esta é uma das razões pelas quais nós usamos um editor de código :)

Obviamente, você é um(a) desenvolvedor(a) Python bastante experiente agora, então sinta-se livre para escrever um código que você aprendeu hoje.

Não esqueça de salvar as modificações no seu arquivo (Save File, ou utilize o atalho Ctrl + S). Com o arquivo salvo, é hora de executá-lo! Usando as habilidades que você aprendeu na seção de linha de comando, use o terminal para chegar na pasta em que seu arquivo foi salvo.

Se você ficar preso(a), peça ajuda.

Em seguida, use o Python para executar o código no

 arquivo assim:

```
$ python3 python_intro.py
Olá, AfroPython!
```

Tudo bem! Você acabou de executar seu primeiro programa em Python que foi salvo em um arquivo.

Se sente bem?

Vamos descobrir mais coisas que podemos fazer com Python então! :D

</details>

<details>
<summary>Capítulo 11: if...elif...else</summary>

## Capítulo 11: if...elif...else

Muitas coisas no código só podem ser executadas se determinadas condições forem atendidas. É por isso que o Python tem algo chamado declaração `if`.

Substitua o código no arquivo `python_intro.py` por isto:

```python
if 3 > 2:
    print('Isso funciona!')
```

Se você salvar e executar este código, verá a seguinte saída:

```
$ python3 python_intro.py
Isso funciona!
```

O Python espera que forneçamos mais instruções que serão executadas caso a condição `3 > 2` seja verdadeira (ou `True`). Vamos tentar fazer o Python imprimir "Isso funciona!".

Você percebeu que indentamos a próxima linha com 4 espaços? Precisamos fazer isso para que o Python saiba qual código será executado se o resultado for `True`. Você pode usar 1 espaço, mas a convenção é usar 4 espaços para manter as coisas organizadas.

Agora, vamos adicionar uma condição `else` para tratar o caso em que a condição não é verdadeira. Substitua o código no arquivo `python_intro.py` por isto:

```python
if 5 > 2:
    print('5 é realmente maior que 2')
else:
    print('5 não é maior que 2')
```

Ao executar o código, você verá a seguinte saída:

```
$ python3 python_intro.py
5 é realmente maior que 2
```

Se o número 2 fosse maior do que 5, o segundo comando seria executado.

Agora, vamos adicionar uma condição `elif` para tratar mais casos. Substitua o código no arquivo `python_intro.py` por isto:

```python
nome = 'Sonja'
if nome == 'Ola':
    print('Oi Ola!')
elif nome == 'Sonja':
    print('Oi Sonja!')
else:
    print('Oi anônimo!')
```

Ao executar o código, você verá a seguinte saída:

```
$ python3 python_intro.py
Oi Sonja!
```

O Python comparou o valor da variável `nome` e caiu na condição do `elif` onde compara `nome == 'Sonja'`, assim imprimindo "Oi Sonja!".

Resumindo, nos últimos exemplos você aprendeu:

- Comparar coisas: em Python, você pode comparar as coisas usando os operadores `>`, `>=`, `==`, `<=`, `<` e os operadores lógicos `and` e `or`.
- Booleanos: um tipo de objeto que tem apenas dois valores: `True` ou `False`.
- Salvando arquivos: armazenando código em arquivos para poder executar programas maiores.
- `if...elif...else`: instruções que permitem executar código somente se determinadas condições forem atendidas.

Parabéns! Agora vamos para a próxima parte.

</details>

<details>
<summary>Capítulo 12: Suas próprias funções</summary>

## Capítulo 12: Suas próprias funções

Se lembra das funções como `len()` que você pode executar no Python? Bem, boas notícias, agora você vai aprender a escrever suas próprias funções!

Uma função é uma sequência de instruções que o Python deve executar. Cada função em Python começa com a palavra

-chave `def`, seguida por um nome para a função e, opcionalmente, uma lista de parâmetros.

Vamos começar com uma função simples. Substitua o código no arquivo `python_intro.py` por isto:

```python
def oi():
    print('Olá!')
    print('Como vai você?')

oi()
```

Aqui está nossa primeira função! 

Você pode se perguntar por que escrevemos o nome da função na parte inferior do arquivo. Isso ocorre porque o Python lê o arquivo e executa de cima para baixo. Portanto, para usar nossa função, precisamos chamá-la na parte inferior.

Ao executar o código, você verá a seguinte saída:

```
Olá!
Como vai você?
```

Vamos criar uma função com parâmetros. Usaremos o exemplo anterior - uma função que diz "oi" para quem a executa - com um parâmetro `nome`. Substitua o código no arquivo `python_intro.py` por isto:

```python
def oi(nome):
    if nome == 'Ola':
        print('Oi Ola!')
    elif nome == 'Sonja':
        print('Oi Sonja!')
    else:
        print('Oi anônimo!')

oi("Ola")
```

Ao executar o código, você verá a seguinte saída:

```
Oi Ola!
```

Se mudarmos o nome, a função será executada de acordo com o novo nome. Substitua o código no arquivo `python_intro.py` por isto:

```python
oi("Sonja")
```

Ao executar o código, você verá a seguinte saída:

```
Oi Sonja!
```

Se você escrever outro nome que não seja "Ola" ou "Sonja", a função imprimirá "Oi anônimo!".

Dessa forma, você não precisa se repetir a cada vez que quiser mudar o nome da pessoa que a função cumprimenta. E é exatamente por isso que precisamos de funções - você não quer repetir seu código!

Parabéns! Agora você sabe como criar suas próprias funções :)

</details>

<details>
<summary>Capítulo 13: Laços de repetição</summary>

## Capítulo 13: Laços de repetição

Chegamos à última parte. Foi rápido, não foi? :)

Como mencionamos, as pessoas que programam são preguiçosas e não gostam de repetir as mesmas coisas. Programação é sobre automatizar coisas, então não queremos cumprimentar cada pessoa pelo seu nome manualmente, certo? É aí que os laços entram em jogo.

Vamos criar uma lista de garotas:

```python
garotas = ['Rachel', 'Monica', 'Phoebe', 'Ola', 'You']
```

Agora, queremos cumprimentar todas elas pelos seus nomes. Temos a função `oi` para fazer isso, então vamos usá-la em um loop:

```python
for nome in garotas:
    oi(nome)
    print('Próxima!')
```

Aqui está o código completo que será salvo no arquivo `python_intro.py`:

```python
def oi(nome):
    print('Oi ' + nome + '!')

garotas = ['Rachel', 'Monica', 'Phoebe', 'Ola', 'You']
for nome in garotas:
    oi(nome)
    print('Próxima!')
```

Ao executar o código, você verá a seguinte saída:

```
Oi Rachel!
Próxima!
Oi Monica!


Próxima!
Oi Phoebe!
Próxima!
Oi Ola!
Próxima!
Oi You!
Próxima!
```

Como você pode ver, tudo o que você colocar dentro do loop `for` será repetido para cada elemento da lista `garotas`.

Você também pode usar o `for` com números usando a função `range`:

```python
for i in range(1, 6):
    print(i)
```

Isso imprimirá:

```
1
2
3
4
5
```

`range` é uma função que cria uma lista de números que seguem um após o outro (esses números são fornecidos por você como parâmetros).

Observe que o segundo número não está incluído na lista. No exemplo `range(1, 6)`, conta-se de 1 a 5, mas o 6 não é incluído.

Resumo
----------
Parabéns! Você concluiu este capítulo!

Agora você sabe como usar instruções condicionais (`if`, `elif`, `else`) para executar código com base em condições, como criar suas próprias funções e como usar loops de repetição (`for`) para automatizar tarefas.

Dê uma pausa, faça um alongamento, dê uma volta ou descanse os olhos antes de prosseguir para o próximo capítulo. Você está indo muito bem! :)