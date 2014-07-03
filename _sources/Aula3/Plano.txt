..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 3
---------

Objetivos
+++++++++


- Salvar e executar programas no IDLE
- Entender alguns tipos de dados
- Utilizar as funções ``print()`` e ``input()``
- Ententer o propósito de listas (``list``)


Preparação
++++++++++

**Materiais**

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 


Atividades
++++++++++


**Conceitos computacionais**

1. Relembre as funcionalidades do IDLE como abrir e salvar programas.
2. Crie um programa para armazenar um número em uma variável.
3. Quais os outros tipos de informação podemos armazenas numa variável? 

Relembre como armazenar uma *string* numa variável e algumas operações.

.. sourcecode:: python
	
	>>> nome = "Pedro " # atribuição
	>>> sobrenome = "Silva"
	>>> nome_completo = nome + " " + sobrenome # concatenação

4. Introduza listas.
5. Tipos de dados.

Faça uma diferenciação nos tipos de dados utilizados.


+------------------------+-------------------------------------------------------+---------+
|       Tipo             |   Exemplos                                            | Tipo    +
+========================+=======================================================+=========+
| Números inteiros       | ``1``, ``2``, ``3``, ``4``, ``5``, ..., ``99``, ...   | 'int'   |
+------------------------+-------------------------------------------------------+---------+
| Números fracionários   | ``0.0001``, ``0.5``, ``3.14159``, ``12.5``, ...       | 'float' |
+------------------------+-------------------------------------------------------+---------+
| Texto                  | ``"10"``, ``"3.14159"``, ``"nome"``                   | 'string'|
+------------------------+-------------------------------------------------------+---------+
| Lista                  |``[]``, ``"['a','b','c']"``, ``[1,2,3]``               | 'list'  |
+------------------------+-------------------------------------------------------+---------+


6. Armazene alguns valores em listas simples (nomes de times de futebol, por exemplo). Remova um item de uma lista e também de uma *string*.
7. Apresente formalmente a função ``print()``
8. Apresente formalmente a função ``input()``

Para intruduzir o conceito de procedimento, mostre a execução do programa passo a passo, uma idéia:

.. activecode:: aula3

	alunos = []
	nome = input("Diga um nome?")
	alunos.append(nome)
	nome = input("Diga outro nome?")
	alunos.append(nome)
	print(alunos)
	
	
**Proposta** 
	
- Inserir os nomes dos alunos da turma numa lista


Reflexão
++++++++


