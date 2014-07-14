..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 4: Primeiras Funcionalidades
=================================

Objetivos
+++++++++

- Entender o que são funções e seus argumentos.
- Aprender a utilizar o comando ``import``.
- Compreender o conceito e acesso a módulos.
- Trabalhar com números aleatórios.
 

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.

Atividades
++++++++++

**Conceitos computacionais**

Até o momento nos familiarizamos com as `idéias e conceitos <../Aula1/Plano.html>`__ para construir programas, começamos a conhecer 
o `ambiente <../Apoio/idle.html>`__ IDLE, brincamos com `operadores matemáticos <../Aula2/Plano.html#atividades>`__ e finalmente aprendemos a `definir variáveis <../Aula3/Plano.html>`__. 

.. admonition:: Funções

  Funções são uma espécie de "*mini*-programa" dentro do código que permite executá-lo facilmente. Para acessá-las 
  basta saber o seu *nome* e *argumentos*. 
  
  No Python elas seguem a estrutura: ``nome`` ``(`` ``argumentos`` ``)`` e podem retornar valores ou não. 
  
  Nas aulas anteriores utilizamos duas funções print() e input()
  
  - Quando fazemos ``print(u"Olá Mundo")`` estamos invocando a função ``print()`` com o **argumento** ``u"Olá Mundo"``.
  - Já ao utilizar a função ``input()`` temos a opção de passar um parâmetro (ex. ``input(u"qual o seu nome?")`` sendo que ela **retorna**
    o valor inserido pelo usuário. Nos exemplos anteriores atribuimos esta entrada a uma variável.

1. Além das funções de **entrada/saída** (print/input) apresente outras funções, algumas sugestões:

+------------+---------------------------------------------------+-----------------+--------------------+---------------------+
| Função     | O que ela faz?                                    | Argumentos      |      Retorno       | Exemplo             |
+============+===================================================+=================+====================+=====================+
| ``type()`` | descobre o tipo da variável                       | objeto          |  tipo  do objeto   |  ``type(4)``        |
+------------+---------------------------------------------------+-----------------+--------------------+---------------------+
| ``len()``  | retorna o número de caracteres de uma sequência   | string ou lista |  número inteiro    | ``len("programaê")``|
+------------+---------------------------------------------------+-----------------+--------------------+---------------------+
| ``help()`` | retorna detalhes de acesso/retorno de uma função  | nome da função  | descrição da função| ``help(print)``     | 
+------------+---------------------------------------------------+-----------------+--------------------+---------------------+


Trabalhe no `console interativo <../Apoio/idle.html#console-iterativo>`__ estas funções.

2. A linguagem Python contém muitas funções pré-definidas, as citadas acima são chamadas de funções *built-in* ou seja, estão "embutidas" e não dependem 
de nenhum passo extra para serem acessadas: veja uma `lista de funções <../Apoio/builtin.html>`__ embutidas e trabalhe algumas com os alunos. 

3. Para acessarmos um conjunto maior de funções precisamos definir explicitamente sua localização, é preciso importá-la acessarmos dentro do programa. Para tal
utilizamos a palavra-reservada ``import``, nesta aula iremos apresentar o pacote **random** que contem funções para trabalhar com números aleatórios.

Por definição as instruções para importar módulos são definidas no inicio do programa.

.. sourcecode:: python

  """
  definições
  """
  
  import random
  
  # resto do programa.
  
Para exemplificar esta aula utilizaremos funções definidas no módulo (*pacote*) random: ``randint()`` e ``choice``. 
Proponha as seguintes atividades:

4. Gerar um número aleatório inteiro entre ``-5`` e ``5``

.. activecode:: random1

	import random # nossa "caixa" de funcionalidades
	numero = random.randint(-5,5)
	print(numero)

Para acessar precisamos primeiro definir o módulo e depois a função em questão, o ``.`` faz esta "ligação" entre módulo e função. 
Execute mais algumas vezes para ver os números se alternando.
	
	
- Escolher um número na lista de cores.

.. activecode:: random2

  import random
  cores = ('azul', 'amarelo', 'verde', 'azul', 'branco' )
  print(random.choice(cores))
  
Note que a função ``choice()`` recebe uma lista de itens (cores) e retorna apenas uma. Neste exemplo não utilizamos variável,
pegamos o retorno da função *choice* e passamos como parâmetro para a função *print*, conhecida comumente como funções aninhadas.


.. admonition:: Funções aninhadas

  É importante nesta aula destacar conceito de *retorno* de uma função como parâmetro de outra, a leitura deve ser de dentro para fora. No exemplo abaixo usamos três funções:
  *input*, *len* e *print*. Com o ``input()`` obtemos a funcionalidade do usuário poder inserir um valor, seguimos com a função ``len()`` que pega o retorno do *input*
  e calcula o número de caracteres, por fim utilizamos o resultado como argumento função ``print()``.

  .. sourcecode:: python
  
    print(len(input("qual o seu nome: ")))

- Simular a jogada de um dado de 6 lados. 

.. activecode:: dado

  import random
  print(random.randint(1,6))
   

.. admonition:: Acesso a funções

  Tente invocar uma função sem fazer um ``import``. Mostre que quando esquecemos de importar uma biblioteca 
  geramos um erro de falta de definição.
  
    ``NameError: name 'random' is not defined``


**Proposta** 

- Utilize o ``randint`` e a função ``choice`` para criar um programa de sorteios.

Exemplos:

- MegaSena - construir um número para sortear os números.
- AmigoSecreto - Escolher uma pessoa (semelhante ao problema com cores)

Comandos sugeridos:

* ``randint()``
* ``choice()`` 
	

Reflexão
++++++++




