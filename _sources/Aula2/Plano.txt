..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Motivação
----------

Objetivos
----------

- Instalar o Python
- Se familiarizar com o IDLE
- Criar um programa simples. Rode pela shell e pela linha de comando
- Entender a diferença entre um programa e uma linguagem de programação.

Materiais
----------

- IDLE

Atividades
----------

Instique os alunos a experimentarem o console, introduza os conceitos de uma calculadora simples. 

=================	=============	
Operação			Exemplo
=================	=============	
Adição (+)			``4 + 3``
Subtração (-)		``10 - 6``
Multiplicação (*)	``7 * 6``
Divisão	(/)			``9 / 3``
=================	=============

Para imprimir o resultado dentro de um programa, não se esqueça do ``print``

.. activecode:: Operações Básicas

	print 4 + 3
	print 10 - 6
	print 7 * 6
	print 9 / 3

Demonstre a prioridade dos operadores matemáticos. 

.. admonition:: Lidando com números fracionados no Python 2.7.x

		Experimente fazer ``3/2`` teremos ``1`` e não ``1.5``. A versão do Python (2.7) que utilizamos para este curso trata os números como inteiros, portamo se quisermos obter o valor correto é preciso escrever a sentença com um ``.`` tal como ``3/2.`` ou ``3./2``

**Interpretando os erros** 

Ensine os alunos a decifrar as mensagens de erros. 

.. sourcecode:: python

	>>>algumcomando
	Traceback (most recent call last):
  	  File "<stdin>", line 1, in <module>
	NameError: name 'algumcomando' is not defined

	>>> 4 1 +
  	  File "<stdin>", line 1
          4 1 +
          ^
	SyntaxError: invalid syntax

Normalmente os erros são relacionados a comandos **não definidos** e **sintaxe**. Oriente aos alunos a *ler* sempre estas mensagens. 

	
Avaliação
----------
