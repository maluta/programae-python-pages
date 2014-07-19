..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 6: Repetições (I)
==============================

Objetivos
+++++++++

- Aprender a utilizar laços ``for``

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.

Atividades
++++++++++

**Conceitos computacionais** 

O título desta aula é simples e direto: **repetições**. Introduza o conceito através de exemplos e comece por algo simples como imprimir 
uma lista de números na tela. Uma solução seria utilizar uma sequência de ``print()``, ``print()`` , ``print()`` ..., levante algumas questões:

- Se esta lista for muito longa? 
- Existe algo que podemos fazer para melhorar? 

.. sourcecode:: python

  print("1")
  print("2")
  print("3")
  print("4")
  print("5")
  # ...
  print("50")
  # ...
  print("99")

Continue e apresente um exemplo mais completo, como seria um programa para perguntar a idade de todos os alunos da sala? 

.. activecode:: cad

  print("Cadastro de idades")
  
  nome_1 =  input("Digite seu nome:  ")
  idade_1 = input("Digite sua idade: ")
    
  nome_2 =  input("Digite seu nome:  ")
  idade_2 = input("Digite sua idade: ")
    
  nome_3 =  input("Digite seu nome:  ")
  idade_3 = input("Digite sua idade: ")
  
  print("Cadastrado: " + nome_1 + " (" + idade_1 + " anos) ")
  print("Cadastrado: " + nome_2 + " (" + idade_2 + " anos) ")
  print("Cadastrado: " + nome_3 + " (" + idade_3 + " anos) ")
  
  #...
  
Mostre o impacto na quantidade de linhas de código se quiséssemos cadastrar todos os alunos da sala. 

Aprendemos até então apenas como dar instruções sequênciais ao programa, para resolver este problemas precisamos aprender 
mais algumas palavras-reservadas.

A primeira é a dupla de comandos ``for`` e ``in``, veja o funcionamento para imprimir 5 itens na tela.

.. activecode:: for 

  for item in range(5):
    print(item)

   
Comentários linha-a-linha:

- A linha 1 pode ser lida como: 
  
  *para cada "valor" dentro da "faixa" faça* 
    
- A linha dois é o bloco de código que será executado a cada interação (lembre-se da `indentação <../Apoio/boaspraticas.html#indentacao>`__ )  
  
  
.. admonition:: A função ``range()``

  Na linha 1 utilizamos uma função chamada ``range`` que pertence ao grupo de funções `embutidas <../Apoio/builtin.html>`__ do 
  Python. É importante dar uma atenção especial a ela, destacando alguns pontos:
  
  - A função ``range()`` que gera um lista de valores de acordo com os argumentos passados para ela.
  - Ao passarmos somente um parâmetro, a função ``range()`` retorna uma lista de números. Diferente do que imaginamos, ela não 
    retorna uma lista até o número especificado (nesse caso, de 0 a 5) mas sim um intervalo que se inicia no **zero** e termina 
    no número inteiro que **antecede** o número especificado. 
    
    Na notação matemática para intervalos, a função range do exemplo anterior criaria o seguinte intervalo: [0,5). 
    Isto é, um intervalo fechado à esquerda e aberto à direita.
    
    .. image:: ../../_static/intervalo.png


    
**Atividades para a empresa**

- 
    
    
Reflexão
++++++++

É importante que todos aprendam a pensar nos objetivos e resultados.
    
    
  


  
