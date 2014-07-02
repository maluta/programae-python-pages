..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 2
======

Objetivos
+++++++++

- Instalar o Python
- Primeiro contato com o ambiente: IDLE
- Criar um programa simples. Rode pelo *console* e através de um **arquivo**
- Entender a diferença entre um programa e uma linguagem de programação.
- Interpretar erros básicos

Preparação
++++++++++

**Materiais**

- IDLE

Atividades
++++++++++

1. Inicialize o console do IDLE e explique o papel do console para execução de códigos rápidos
2. Demonstre a execução de um programa simples

.. activecode:: idade

	nascimento = input("Em que ano voce nasceu?")
	idade = 2014 - int(nascimento)
	print("Voce ja tem", idade, "anos!")

Instigue os alunos a experimentarem o console, introduza as instruções para uma calculadora simples. 

=================	=============	
Operação			Exemplo
=================	=============	
Adição (+)			``4 + 3``
Subtração (-)		``10 - 6``
Multiplicação (*)	``7 * 6``
Divisão	(/)			``9 / 3``
=================	=============

Para imprimir o resultado dentro de um programa (arquivo), não se esqueça do ``print``

.. activecode:: Operações Básicas

	print(4 + 3)
	print(10 - 6)
	print(7 * 6)
	print(9 / 3)

Demonstre a prioridade dos operadores matemáticos. 

".. admonition:: Lidando com números fracionários no Python 2

		Ao fazer ``3/2`` teremos ``1`` e não ``1.5``. Esta versão do Python trata os números como inteiros, portanto se quisermos obter o valor correto é preciso escrever a sentença com um ``.`` tal como ``3/2.`` ou ``3./2``

É importante neste momento:

- Gerar erros de sintaxe.
- Escrever palavras reservadas e não reservadas.
- Como armazenar uma variável (uma idéia é salvar a idade dos alunos).
- Liberdade para explorar. 

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

A primeira parte ``SyntaxError`` é o tipo do erro, e após o sinal de ``:`` vem a descrição: erro de sintaxe inválida.
Geralmente os erros mais comuns são relacionados a sintaxe, falta de definição e tipos errados.


Reflexão
++++++++

Avalie a participação e curiosidade dos alunos.