#  Linguagem de Programação

## Introdução à Linguagem Python

### Prof.ª Elisa Antolli (Mestre em Ciência da Computação)

---

## Principais conceitos de programação em Python

- A linguagem Python
- Ferramentas
- Estruturas lógicas, condicionais e de repetição
- Funções
- Exemplos de códigos

> Conceitos

## Introdução linguagem de Programação Python

O que é Linguagem de Programação?

- As linguagens de programação foram criadas para solucionar qualquer tipo de problema na área tecnológica computacional.
- Cada linguagem possui suas particularidades.
- Permite que um programador crie programas a partir de um conjunto de ordens, ações consecutivas, dados e algorítimos.
- Python é uma linguagem de script de alto nível, de tipagem forte e dinâmica.

## Primeiros passos em Python

- Vamos criar nosso primeiro programa em Python.

  ```python
  print("Hello, World!")
  ```

  ```tex
  Hello, World!
  ```

## A Linguagem Python

- Criado no início dos anos 1990 por Guido van Rossum no Stichting Mathematisch Centrum (CWI), na Holanda, foi sucessor de uma linguagem chamada ABC.
- Em 2001, a Python Software Foundation (PSF) foi formada, uma organização sem fins lucrativos criada especificamente para possuir a propriedade intelectual relacionada ao Python.

### Porque Python?

- Python é uma linguagem de programação clara e poderosa.
- usa sintaxe clara, facilitando a leitura dos programas que você escreve;
- Linguagem fácil, ideal para o desenvolvedor de protótipos e outras tarefas de programação;
- Grande biblioteca padrão, suporta muitas tarefas de programação;
- Possui inúmeras bibliotecas que estendem seu poder de atuação.
- Linguagem interpretada, ou seja, uma vez escrito o código, este não precisa ser convertido em linguagem de máquina por um processo de compilação;
- Permite atribuição múltipla;
- O interpretador Python 3 utiliza unicode por padrão, o que torna possível usar nomes de variáveis com acento e até outros caracteres especiais, porém não é uma boa prática.
- Códigos em Python pode ser feito tanto em local quanto em nuvem.

## Instalação do interpretador Python:

[https://www.python.org/downloads/](https://www.python.org/downloads/)

Na instalação, marcar a opção "Add Python 3.x to PATH".

O Python instalado, já podemos digitar comandos python:

> No terminal

```bash
print("Olá mundo!")
```

> Resultado

```bash
Olá mundo!
```

## Ferramentas

- Para implementação de soluções, normalmente utiliza-se uma IDE, (Integrated Development Environment) ou Ambiente de Desenvolvimento Integrado.

- Duas IDE's disputam a preferência dos desenvolvedores Python, o PyCharm e o Visual Studio Code (VSCode).

  - PyCharm: Profissional e Community, sendo a primeira paga e a segunda gratuita.
  - VSCode: Gratuito.

- Python Anaconda ([https://www.anaconda.com/distribution/](https://www.anaconda.com/distribution/)).

  Consiste na unição de ferramentas Python, composta por bibliotecas e IDE's.

- Possui tanto o interpretador Python quanto bibliotecas, duas interfaces de desenvolvimento: a IDE spyder e o projeto Jupyter.

- Grande diferencial do projeto Anaconda é ter o Jupyter Notebook ([https://jupyter.org/](https://jupyter.org/)) integrado na instalação, principalmente para o uso sistemas de controle de versão (como o Git / GitHub).

- Google Colaboratory (Colab)

  [https://colab.research.google.com/notebooks/](https://colab.research.google.com/notebooks/)

- Especialmente adequado para aprendizado de máquina, análise de dados e educação. Colab é um serviço de notebook Jupyter hospedado que não requer configuração para ser usado.

---

> Conceitos

## Variáveis e tipos básicos de dados em Python

### Variáveis

- Variáveis são espaços alocados na memória RAM para guardar valores temporariamente.
- Em Python, esses espaços não precisam ser tipados, a variável pode ser alocada sem especificar o tipo de dado que ela aguardará.
- As variáveis são tipadas dinamicamente nessa linguagem.

Exemplos:

- Para saber o tipo de dado que uma variável guarda, podemos imprimir seu tipo usando a função type(), veja como:

  ```python
  x = 10
  name = "Teste"
  nota = 8.5
  flag = True
  
  print(type(x))
  print(type(name))
  print(type(nota))
  print(type(flag))
  ```

  > Resultado

  ```bash
  <class 'int'>
  <class 'str'>
  <class 'float'>
  <class 'bool'>
  ```

  Em Python, tudo é objeto! Por isso os tipos de dados aparecem com a palavra "class".

  Função input() faz a leitura de um valor digitado.

  Veja como usar:

  ```py
  name = input("Digite um nome: ")
  print(name)
  ```

  > Resultado

  ```bash
  Digite um nome: Marcos
  Marcos
  ```

  Temos uma variedade de formas de imprimir texto e variável em Python.

  Vejamos algumas:

  - podemos usar formatadores de caracteres (igual em C)
  - podemos usar a função format() e
  - podemos criar uma string formatada.

  **Modlo 1: usando Formatadores de caracteres (igual na linguagem C):**

  *print("Oá %s, bem vindo a disciplina de programação. Parabéns pelo seu primeiro hello world" % (name))*

  ```py
  name = input("Digite um nome: ")
  print("Olá %s, bem vindo a disciplina de programação. Parabéns pelo seu primeiro hello world" % (name))
  ```

  > Resultado

  ```bash
  Digite um nome: Marcos
  Olá Marcos, bem vindo a disciplina de programação. Parabéns pelo seu primeiro hello world
  ```

  **Modo 2: usando a função format() para imprimir variável e texto:**

  ```py
  print("Olá {}, bem vindo a disciplina de programação. Parabéns pelo seu primeiro hello world".format(name))
  ```

  **Modo 3: usando strings formatadas**

  ```py
  print(f"Olá {name}, bem vindo a disciplina de programação. Parabéns pelo seu primeiro hello world")
  ```

- Usamos o hash # para criar comentários de uma linha.

- Nessa PEP, a 498, o autor destaca o uso do "modo 3" como a melhor opção, chamando-a de "f-strings".

- As strings formatadas com "f-strings" só podem ser usadas com o interpretador Python na versão 3.6.

---

## Operações matemáticas suportadas por Python

Com exceção das funções abs() e pow() e da notação de potência **, as outras operações e sintaxe são similares a diversas linguagens de programação.

| Operation       | Result                                                       |
| --------------- | ------------------------------------------------------------ |
| x + y           | sum of x and y                                               |
| x - y           | difference of x and y                                        |
| x * y           | product of x and y                                           |
| x / y           | quotient of x and y                                          |
| x // y          | floored quotient of x and y                                  |
| x % y           | remainder of x / y                                           |
| -x              | x negated                                                    |
| abs(x)          | absolute value or magnitude of x                             |
| int(x)          | x converted to integer                                       |
| float(x)        | x converted to floating point                                |
| complex(re, im) | a complex number with real part / imaginary part *im. im* defaults to ... |
| c.conjugate()   | conjugate of the complex number...                           |
| divmod(x, y)    | the pair (x // y, x % y)                                     |
| pow(x, y)       | x to the power y                                             |
| x ** y          | x to the power y                                             |

Repare como é fundamental conhecer a ordem de procedências das operações para não criar cálculos errados durante a implementação de uma solução.

1. Primeiro resolvem-se os parênteses, do mais interno para o mais externo.
2. Exponenciação.
3. Multiplicação e divisão.
4. Soma e subtração.

```py
# Qual o resultado armazenado na variável operacao_1: 25 ou 17?
operacao_1 = 2 + 3 * 5
# Qual o resultado armazenado na variável operacao_2: 25 ou 17?
operacao_2 = (2 + 3) * 5
# Qual o resultado armazenado na variável operacao_3: 4 ou 1?
operacao_3 = 4 / 2 ** 2
# Qual o resultado armazenado na variável operacao_4: 1 ou 5?
operacao_4 = 13 % 3 +4
```

> Resultado

```bash
Resutlado em operacao_1 = 17
Resutlado em operacao_2 = 25
Resutlado em operacao_3 = 1.0
Resutlado em operacao_4 = 5
```

---

## Estruturas Lógicas, Condicionais e de Repetição em Python

Em geral, em um programa você tem opções de caminhos ou lista de comandos que nada mais são que trechos de códigos que podem ser executados, devendo-se tomar decisões sobre qual trecho de código será executado em um determinado momento.

![](./images/EstruturasLogicasCondicionaisEDerepeticaoEmPython.png)
