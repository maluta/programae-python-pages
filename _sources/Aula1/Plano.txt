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

- Entender o conceito da *Fábrica de Jogos* deste curso.
- Introduzir os alunos o conceito de arquitetura de computadores.
- Demonstrar a importância de aprender uma linguagem de programação.
- Entender a diferença entre um programa e uma linguagem de programação.

Preparação
++++++++++

**Materiais**

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
++++++++++

**Conceitos computacionais**

Comece por instigar os alunos com a pergunta: *Porquê alguém deveria aprender a fazer programas de computador?*

Orientando-os a buscar referências no dia-a-dia, onde a computação é aplicada. Contextualize com exemplos tais como serviços na internet, exemplos: e-mail, Facebook, Twitter. Nesta parte é importante destacar que a computação (*software*) não esta presente apenas nos computadores pessoais (*desktop*) mas em celulares, carros, televisores, etc; e que isso não é um futuro distante mas sim o presente.

Destaque as respostas mais populares e siga com a proposta de apresentar como o computador “pensa” ou seja, com o método de execução de um programa funciona. Faça uma lista de atividades listando as tarefas que são mais comuns a humanos e as tarefas que são mais comuns aos computadores. Um exemplo é contar o número de palavras de um texto (habilidade melhor executada por um computador) e interpretar o conteúdo do mesmo texto (habilidade melhor executada por um ser humano).

Apresente o conceito de computador como um dispositivo assistente pessoal que constantemente nos pergunta:

*“O que [devo fazer] agora?”*

Trabalhe os conceitos de **arquitetura** de computadores nestes 5 grupos macros:

- **CPU** (*Central Processing Unit*)
- **Memória Principal** (*Main Memory*)
- **Memória Secundária** (*Secondary Memory*)
- **Dispositivos de Entrada/Saída** (*Output Devices*)
- **Rede**

Mostre como estes grupos e faça analogias. Uma dica é Recortar quadrados de papel e indifique cada uma das partes, pergunte como elas podem ser associadas? 

Demonstre que o papel do programador é orquestrar todos estes recursos, sempre dando instruções para a CPU que, se necessário, vai requisitar aos outros “blocos” para atender o seu pedido. Tais instruções podem ser dadas diretamente, mas seria um trabalho repetitivo e lento, por isso estas instruções devem ser armazenadas em um programa. 

Siga com a questão: **O que é necessário saber para me tornar um programador?

Sugestões para discussão:

1. **Aprender uma linguagem de programação**, faça analogias como aprender outro idioma, conhecendo o vocabulário e a gramática.
2. **Aprender a se comunicar** de forma clara (da mesma forma que contamos uma história e melhoramos a medida que nos exercitamos). O programa é a “história” e o problema a ser resolvido é a "idéia". 

Comece por diferenciar uma linguagem humana como Português, Inglês ou Espanhol de uma linguagem de programação como o Python, apresentando as diferenças entre elas, especialmente ao tamanho do vocabulário que nas linguagens de programação são chamadas de palavras reservadas. 

Podemos pensar num treinador de cachorros que usa palavras especiais para algumas ações: “senta!”, “parado!” e “pega!”. Se utilizarmos outras palavras que o cachorro não reconhece ele não irá compreender. 

Liste algumas palavras reservadas do vocabulário Python, como: ``and``, ``del``, ``for``, ``is``, ``raise``, ``assert``, ``elif``, ``from``, ``lambda``, ``return``, ``break``, ``else``, ``global``, ``not``, ``try``, ``class``, ``exec``, ``if``, ``or``, ``while``, ``continue``, ``exec``, ``import``, ``pass``, ``yeld``, ``def``, ``print``.  

Não se preocupe neste momento em descrever cada uma, o importante é destacar como começar a falar, para isso vamos utilizar o comando ``print`` da linguagem. É importante neste momento mostrar como o computador recebe as instruções, interpreta e executa uma ação. 

.. activecode:: idade

	idade = 15
	print("Minha idade:",idade)


Por fim, demonstre que programa é construir soluções. Podemos instruir o computador a automatizar este processo. 

Termine apresentando a **Fábrica de Jogos** e suas regras:

.. admonition:: Regras 

	- Separe a turma em grupos de até 3 alunos. 
	- Nas próximas aulas, os alunos receberão o desafios de construir um jogo. 
	- O professor (na figura de investidor) irá dar 100 `progmoney <../Apoio/progmoney.html>`__  (sigla ``$>>>``) para cada grupo começar a empresa de jogos. 
	- Em cada aula os alunos receberão uma lista de comandos permitidos para construção do jogos. 
	- A construção de código tem um *custo* de progmoney
	- Cada linha de código custa ``1 $>>>``.
	- Uso de instruções não permitidas custam ``30 $>>>``
	- Ao aprender funcionalidade novas os grupos recebem mais progmoney.
	- Existe uma tabela de preços por instrução.

Reflexão
+++++++++

Nesta aula vimos com o computador pode automatizar nossas vidas, mas é importante destacar que a **criatividade** é ferramenta para construção. 
Nesta etapa avalie a participação e interesse dos alunos. Como a proposta das aulas seguintes é orientar os alunos em projetos, pense nas possibilidades da linguagem e mostre como eles poderiam criar algo, categorize os tópicos mais populares.

**Referências**

`Site oficial do Python <http://python.org>`__

`Porque Aprender a Programar <http://ramalho.pro.br/aprendaprog/cap0.html>`__
