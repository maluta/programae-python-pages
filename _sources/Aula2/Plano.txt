..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 2: Conceitos & Ambiente
=============================

Objetivos
+++++++++

- Entender as partes que constituem a arquitetura básica de um computador.
- Entender o modelo de execução: pergunta -> resposta. 
- Ter o primeiro contato com a Linguagem Python.
- Explorar o ambiente de desenvolvimento.

Preparação
++++++++++

**Materiais**

- Ambiente IDLE (Veja na seção de ajuda: `Como instalar o Python <../Apoio/comoinstalar.html>`__)
- `Console <../Apoio/idle.html#console-interativo>`__ do IDLE


Atividades
+++++++++++

- Comece a aula relembrando a última pergunta da aula anterior: *"O que nós precisamos aprender para criar .....?"* 
- Trabalhe as questões a seguite, que envolvem os primeiros conceitos computacionais necessários. 

**Conceitos computacionais**

Como os computadores trabalham?

Levante alguns possíveis necessidades que os cientistas desenvolveram o computador, mostre que o computador é muito bom para executar rapidamente tarefas 
repetitivas mas não conseguem tomar decisões por si só, por isso precisam sempre seguir um roteito. 

Um resumo do modelo de funcionamento lógico do computador. 

.. image:: ../../_static/pergunta_resposta.png

Além do modelo lógico de "pergunta -> resposta" os computadores possuem uma plataforma física para interação com o mundo externo.

A seguir apresente os conceitos de **arquitetura** de computadores nestes 5 grupos macros (para mais detalhes clique nos links na tabela):

+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+
|  Item                                                                                         |  Nome em inglês                                            |  Exemplos                                |
+===============================================================================================+============================================================+==========================================+
|  `CPU <http://pt.wikipedia.org/wiki/Unidade_central_de_processamento>`__                      |  *Central Processing Unit*                                 |  Intel Core i3                           | 
+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+
|  `Memória Principal <http://pt.wikipedia.org/wiki/Mem%C3%B3ria_prim%C3%A1ria#Tipologia>`__    |  *Main Memory*                                             |  Memória RAM                             |
+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+
|  `Memória Secundária <http://pt.wikipedia.org/wiki/Mem%C3%B3ria_secund%C3%A1ria#Tipologia>`__ |  *Secondary Memory*                                        |  HD, Disco rígido                        |
+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+
|  `Disp. Entrada/Saída <http://pt.wikipedia.org/wiki/Entrada/sa%C3%ADda>`__                    |  *Input/Output devices*                                    |  Teclado, mouse                          |
+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+
|  `Rede <http://pt.wikipedia.org/wiki/Rede_de_computadores>`__                                 |  *Network*                                                 |  Modem Wi-fi                             |
+-----------------------------------------------------------------------------------------------+------------------------------------------------------------+------------------------------------------+

.. image:: ../../_static/arquitetura.png

Exemplos de dispositivos de Entrada/Saida 

.. image:: ../../_static/interface.png

Descrição (para detalhes clique nos links)

1. `HDMI <http://pt.wikipedia.org/wiki/High-Definition_Multimedia_Interface>`__ — Saída
2. `RJ45 <http://pt.wikipedia.org/wiki/RJ-45>`__ (rede) — Entrada/Saída
3. `VGA <http://pt.wikipedia.org/wiki/Video_Graphics_Array>`__ — Saída
4. `USB <http://pt.wikipedia.org/wiki/Universal_Serial_Bus>`__ — Entrada/Saída

Demonstre que o papel do programador é orquestrar todos estes recursos, sempre dando instruções para a CPU que, se necessário, vai requisitar aos outros “blocos” para atender o seu pedido. Tais instruções podem ser dadas diretamente, mas seria um trabalho repetitivo e lento, por isso estas instruções devem ser armazenadas em um programa. 

**Python**

Explique o que é a linguagem Python para os alunos focando no contexto do grupo de alunos. 

Algumas sugestões:

- Python é uma das linguagens de programação mais populares.
- Empresas que utilizam Python: Walt Disney, Google, Intagram, IBM, Globo.com (foque nas possibilidades de trabalho)
- Gratuíto e sem limitações. 

Liste algumas palavras reservadas do vocabulário Python, como: ``and``, ``del``, ``for``, ``is``, ``raise``, ``assert``, ``elif``, ``from``, ``lambda``, ``return``, ``break``, ``else``, ``global``, ``not``, ``try``, ``class``, ``exec``, ``if``, ``or``, ``while``, ``continue``, ``exec``, ``import``, ``pass``, ``yeld``, ``def``, ``print``.  

Não se preocupe neste momento em descrever cada uma, o importante é destacar como começar a falar, para isso vamos utilizar o comando ``print`` da linguagem. É importante neste momento mostrar como o computador recebe as instruções, interpreta e executa uma ação. 

.. activecode:: idade

	print("Ei mundo!")

**Atividades**

- Preencha o cartão **Interface** da `aula 2 <../Apoio/cartoes.html#aula-2>`__
- Trabalhe com os alunos do IDLE
- Anuncie o cartão IDLE básico ao custo de ``3$>`` (opcional)
- Para adquirir o cartão print eles precisam escrever no IDLE o nome dos três integrantes do grupo e mostrar ao professor. 

.. sourcecode:: python

   >>> print("Nome A")
   Nome A
   >>> print("Nome B")
   Nome B
   >>> print("Nome C")
   Nome C
   
.. admonition:: Instalação

  Se tiver algum problema com o laboratório verifique com o técnico ou contacte alguém do Programaê!
 
Reflexão
+++++++++

Além destas `reflexões gerais <../Apoio/feedback.html>`__ note como alunos estão lidando com a idéia dos cartões. Há interesse da sala? 

Boa aula!!!