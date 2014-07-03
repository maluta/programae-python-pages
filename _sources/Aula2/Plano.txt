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

- Primeiro contato com o ambiente: IDLE.
- Criar um programa simples. Rode pelo *console* e através de um **arquivo**.
- Entender a diferença entre um programa e uma linguagem de programação.
- Interpretar erros básicos.
- Primeiros trabalhos da fábrica.

Preparação
++++++++++

**Materiais**

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
+++++++++++

**Conceitos computacionais**

1. Inicialize o console do IDLE e explique o papel do console para execução de códigos rápidos.
2. Demonstre a execução de um programa simples.

Instigue os alunos a experimentarem o console, introduza as instruções para uma calculadora simples. 

=================	=============	
Operação			Exemplo
=================	=============	
Adição (+)			``4 + 3``
Subtração (-)		``10 - 6``
Multiplicação (*)	``7 * 6``
Divisão	(/)			``9 / 3``
Resto	(%)			``9 % 3``
=================	=============

Para imprimir o resultado dentro de um programa (arquivo), não se esqueça do ``print``

.. activecode:: Operações Básicas

	print(4 + 3)
	print(10 - 6)
	print(7 * 6)
	print(9 / 3)
	print(10 % 6)

Demonstre a prioridade dos operadores matemáticos. 

É importante neste momento:

- Contruir sentenças
- Observar a precedências dos operadores.
- Gerar erros de sintaxe.
- Escrever palavras reservadas e não reservadas.
- Armazenar valores em variáveis (lembre-se do operador de atribuição ``=``)
- Lembre-se que podemos usar quantas variáveis quisermos 
- Sobrescrever variáveis.

.. admonition:: Discussão

		Qual o propósito de uma variável? Porquê um programa precisa de uma variável? 


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

.. admonition:: Comentários 

	No Python um comentários de uma linha são definidos pelo símbolo ``#`` e comentários de múltiplas linhas pelos blocos ``""" """``


**Desafio**

- Como fazer um programa para saber se um número é par ou impar?


Reflexão
+++++++++

Avalie a participação e curiosidade dos alunos, experimentar nesta parte irá faciliar a construção nas aulas seguintes.