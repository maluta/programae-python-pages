..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 5: Controles (I)
=======================

Objetivos
+++++++++

- Utilizar operadores comparações.
- Utilizar operadores Booleanos (True e False)
- Aprender sentenças com ``if``


Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.


Atividades
++++++++++

**Conceitos computacionais** 

Até o momento, utilizamos instruções sequenciais para dar ordens ao computador. Agora iremos entrar em um mundo novo, onde teremos 
de definir **decisões**. Contudo, antes de apresentar os mecanismos da linguagem para tomada de decisões vamos aprender como 
efetuar comparações.

Abra o `console <../Apoio/idle.html#console-iterativo>`__ e trabalhe alguns exemplos:

.. sourcecode:: python

  >>> -1 > 1
  False
  >>> 10 < 9
  False
  >>> 2+2 == 5
  False

Repare que sempre obtemos como resposta ``False`` (falso) ou ``True`` (verdadeiro). 

Também podemos aplicar estes operadores em outros tipos de dados, por exemplo, não-numéricos:

.. sourcecode:: python

  >>> "a" == "b"
  False
  >>> "a" < "b"
  True

É importante destacar para os alunos dois pontos, quando utilizamos o operador de comparação de igualdade (``==``) estamos nos referindo o **conteúdo** das variáveis, estamos
vendo se "a" *é igual a* "b". Entretando quando utilizamos o operador ``>`` ou ``<`` a lógica é outra. Para entedermos é preciso demonstrar a função (`built-in <../Apoio/builtin.html>`__) 
``ord()``.

.. activecode:: ord

  print("a",ord("a"))
  print("b",ord("b"))
  
 
Repare que quando efetuamos a operação ``<`` na verdade estamos comparando se o código referente a letra ``a`` (97) é menor que o da letra ``b`` (98).

De posse dos conceitos de comparação podemos seguir e aprender a primeira instrução para efetuar decisões no Python, a palavra-reservada ``if``.

Começemos com um exemplo:

.. activecode:: if

  idade = input(u"Qual é a sua idade?") 
  idade = int(idade)
  if idade > 14 == True:
    print(u"Bem-vindo ao curso de Python!")
    print(u"Sua idade é " + str(idade) + " anos.")
  
Vamos analisar cada linha individualmente:

- ``#1`` → Chama a função input() passando como parâmetro a pergunta *'Qual é a sua idade?'* e armazena a resposta na variável idade.
- ``#2`` → Neste momento utilizamos a função (*built-in*) ``str()`` para converter o tipo string para o tipo inteiro. 
- ``#3`` → **Se** o conteúdo da variável idade for maior que 14 executa a próxima linha.
- ``#4`` → Caso a sentença da linha 3 seja verdadeira a função ``print`` com a mensagem de boas vindas é executada. 
- ``#5`` → Novamente utilizamos a função (built-in) ``str()`` que faz o oposto da função *int()* e converte um tipo numérico em string.

**Fluxograma**

Apresente os fluxogramas como ferramentas de apoio para estruturar o raciocínio. Desenhe no papel (ou lousa) como seria o 
trecho de execução de parte do programa.  Abaixo temos a condição ``if`` que dependendo da reposta sim/não executa um bloco de 
código diferente. 

.. image:: ../../_static/fluxograma.png
  :height: 640px
  :width: 480px
  :scale: 50%
  :align: center
  
Não há regras fixas para a construção do fluxograma, a proposta aqui é apenas esboçar o fluxo do programa.

.. admonition:: Indentação

  Repare que as instruções das linhas 4 e 5 estão um pouco deslocados para a direita. A este recuo dá-se o nome de **indentação**
  ou seja, é um bloco de código que é executado dentro de um *contexto*. No exemplo acima, as duas linhas ``print`` só são executadas 
  se confirmarem a condição definida no ``if``. 
  
  **Para a separação de blocos de código, a linguagem Python usa espaços em branco.**
  
  Veja mais exemplos `aqui <../Apoio/boaspraticas.html#indentacao>`__.
  
Para exemplificar vamos definir um protótipo do comando ``if`` que não faz absolutamente nada. 
    
.. sourcecode:: python
  
  if True:
    pass
  
Veja que a condição é **sempre** verdadeira (True) e a palavra-reservada ``pass`` faz com que o código seja validado sem que ainda precisemos pensar na 
*implementação* caso a condição do *if* seja confirmada.

Mais exemplos com ``if``.

.. activecode:: ex_if

  nome = u"José"
  if nome == u"José":
    print(u"Seu nome é: " + nome)


Por fim, apresente a necessidade de ter o segundo caminho, caso a condição da sentença não seja confirmada, para tal apenas complementamos com a palavra ``else``.

    
**Proposta**

- Utilize as funções para números aleatórios para fazer um jogo de adivinhação.
- Sugestão: Utilize o ``if`` para introduzir a idéia probabilidades, por exemplo, a instrução ``random.randint(1,3)`` tem 33,3% de chances (em média) de occorer
  cada uma das possibilidades. Exemplo:
  
.. activecode:: prob 

  import random
  print(u"Você caminha em direção a sala...")
  if random.randint(1,2) == 1: 
      print(u"Um monstro aparece")
  else:
      print(u"Tudo esta calmo e tranquilo")
  

Quando fazemos ``randint(1,2)`` podemos ter como resposta ``1`` ou ``2`` logo, cada uma das resposta, em média, aparecerá em 50% dos casos. 

- Comece a trabalhar com os alunos o "enredo" da história. Como esta pode ser construída?

.. admonition:: RPG

  Pergunte na sala se algum dos alunos conhece jogos de `RPG <http://pt.wikipedia.org/wiki/Role-playing_game>`__ (*Role-playing Game*), eles podem dar dicas de como estrutura uma aventura. 


Reflexão
++++++++

