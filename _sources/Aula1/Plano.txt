..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 1: Regras & Conceitos
==========================

Objetivos
++++++++++

Nesta aula, os alunos deverão:

- Desenvolver o raciocíno lógico dentro da arquitetura dos computadores. 
- Compreender a importância de aprender uma linguagem de programação.
- Entender a diferença entre um programa e uma linguagem de programação.
- Entender o conceito da *Fábrica de Jogos* deste curso.

Preparação
++++++++++

**Materiais**

- Utilizaremos um ambiente de desenvolvimento integrável, o IDLE  (veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__)

.. admonition:: Lembre-se

  O ambiente deve ser instalado localmente nas máquinas, contudo em caso de problema utilize nosso espaço de `experimentação <../Apoio/console.html>`__.

Atividades
++++++++++

**Conceitos computacionais**

Comece por instigar os alunos com a pergunta: *Porquê alguém deveria aprender a fazer programas de computador?*

Orientando-os a buscar referências no dia-a-dia, onde a computação é aplicada. Contextualize com exemplos tais como serviços na internet: e-mail, Facebook, Twitter. 
Nesta parte é importante destacar que a computação (*software*) não está presente apenas nos computadores pessoais (*desktop*) mas em celulares, carros, 
televisores, etc; e que isso não é um futuro distante mas sim o presente.

Destaque as respostas mais populares e siga com a proposta de apresentar como o computador “pensa”, ou seja, como o método de execução de um programa funciona. 
Faça uma lista de atividades listando as tarefas que são mais comuns a humanos e as tarefas que são mais comuns aos computadores.

.. admonition:: Dica

  Os computadores trabalham com repetição e os seres humanos com instrospecção (pensamentos) Um exemplo é contar o número de 
  palavras de um texto (computador) e interpretar o conteúdo do mesmo texto (humano).

Apresente o conceito de computador como um dispositivo assistente pessoal que constantemente nos pergunta:

*“O que [devo fazer] agora?”*

Trabalhe os conceitos de **arquitetura** de computadores nestes 5 grupos macros (para mais detalhes clique nos links na tabela):

+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+
|  Item                                                                                         |  Nome em inglês             |  Exemplos            |
+===============================================================================================+=============================+======================+
|  `CPU <http://pt.wikipedia.org/wiki/Unidade_central_de_processamento>`__                      |  *Central Processing Unit*  |  Intel Core i3       | 
+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+
|  `Memória Principal <http://pt.wikipedia.org/wiki/Mem%C3%B3ria_prim%C3%A1ria#Tipologia>`__    |  *Main Memory*              |  Memória RAM         |
+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+
|  `Memória Secundária <http://pt.wikipedia.org/wiki/Mem%C3%B3ria_secund%C3%A1ria#Tipologia>`__ |  *Secondary Memory*         |  HD, Disco rígido    |
+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+
|  `Disp. Entrada/Saída <http://pt.wikipedia.org/wiki/Entrada/sa%C3%ADda>`__                    |  *Input/Output devices*     |  Teclado, mouse      |
+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+
|  `Rede <http://pt.wikipedia.org/wiki/Rede_de_computadores>`__                                 |  *Network*                  |  Modem Wi-fi         |
+-----------------------------------------------------------------------------------------------+-----------------------------+----------------------+

Demonstre que o papel do programador é orquestrar todos estes recursos, sempre dando instruções para a CPU que, se necessário, vai requisitar aos outros “blocos” para atender o seu pedido. Tais instruções podem ser dadas diretamente, mas seria um trabalho repetitivo e lento, por isso estas instruções devem ser armazenadas em um programa. 

Siga com a questão: **O que é necessário saber para me tornar um programador?**

Sugestões para discussão:

1. **Aprender uma linguagem de programação**, faça analogias como aprender outro idioma, conhecendo o vocabulário e a gramática.
2. **Aprender a se comunicar** de forma clara (da mesma forma que contamos uma história e melhoramos a medida que nos exercitamos). O programa é a “história” e o problema a ser resolvido é a "idéia". 

Comece por diferenciar uma linguagem humana como Português, Inglês ou Espanhol de uma linguagem de programação como o Python, apresentando as diferenças entre elas, especialmente ao tamanho do vocabulário que nas linguagens de programação são chamadas de palavras reservadas. 

Podemos pensar num treinador de cachorros que usa palavras especiais para algumas ações: “senta!”, “parado!” e “pega!”. Se utilizarmos outras palavras que o cachorro não reconhece ele não irá compreender. 

Liste algumas palavras reservadas do vocabulário Python, como: ``and``, ``del``, ``for``, ``is``, ``raise``, ``assert``, ``elif``, ``from``, ``lambda``, ``return``, ``break``, ``else``, ``global``, ``not``, ``try``, ``class``, ``exec``, ``if``, ``or``, ``while``, ``continue``, ``exec``, ``import``, ``pass``, ``yeld``, ``def``, ``print``.  

Não se preocupe neste momento em descrever cada uma, o importante é destacar como começar a falar, para isso vamos utilizar o comando ``print`` da linguagem. É importante neste momento mostrar como o computador recebe as instruções, interpreta e executa uma ação. 

.. activecode:: idade

	print("Ei mundo!")


Por fim, demonstre que programar é resolver problemas (construir soluções). Podemos instruir o computador a automatizar este processo. 

**Experimentação**

1. Uma boa sugestão é escrever um programa, no terminal interativo, para imprimir o nome de cada aluno na tela. 
2. Agrupe ``print()`` para demonstrar a execução linear do código. 


Termine apresentando as regras da **Fábrica de Jogos**:

.. admonition:: Regras 

	- Grupos de até 3 alunos. 
	- Nas próximas aulas, os alunos receberão o desafios de construir um jogo. 
	- O professor (na figura de investidor) irá distribuir 7 `progmoney <../Apoio/progmoney.html>`__  (sigla ``$>``) para cada grupo começar a empresa.
	- Em cada aula os alunos **deverão** adquirir `cartões de funcionalidades <../Apoio/cartoes.html>`__ para utilizar na construção dos jogos. 
	- A construção de código tem um *custo* em *progmoney*
	- Cada linha de código custa ``1 $>``.
	- Uso de instruções não permitidas custam ``30 $>``
	- Ao aprender funcionalidade novas os grupos adquirem mais *progmoney*.
	- Os preços por instrução/comando estão em uma `tabela <../Apoio/progmoney.html>`__.

**Atividades para a empresa**

- Organizar a sala em grupos.
- Dar um nome a empresa. 
- Cada equipe deverá escrever uma carta de apresentação dos componentes.
- Preencher a `Ficha de Inscrição <../Apoio/ficha.html>`__
- Adquirir o primeiro cartão de funcionalidade para imprimir comandos na tela. 

	
	
Reflexão
+++++++++

Nesta aula vimos como o computador pode automatizar nossas vidas, mas é importante destacar que a **criatividade** é ferramenta para construção. 
Nesta etapa avalie a participação e interesse dos alunos. Como a proposta das aulas seguintes é orientar os alunos em projetos, pense nas possibilidades da 
linguagem e mostre como eles poderiam criar algo, categorize os tópicos mais populares.

**Referências**

`Site oficial do Python <http://python.org>`__

`Porque Aprender a Programar <http://ramalho.pro.br/aprendaprog/cap0.html>`__
