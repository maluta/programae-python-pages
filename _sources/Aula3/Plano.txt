..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 3: Variáveis
======================

Objetivos
+++++++++


- Aprender como salvar e executar programas no IDLE.
- Entender o conceito de variável.
- Entender quais tipos de dados podem ser armazenados. 
- Melhorar a legibilidade.


Preparação
++++++++++

**Materiais**

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#sugestao-de-layout>`__ códigos no IDLE.

Atividades
++++++++++


**Conceitos computacionais**

1. Relembre as funcionalidades do IDLE utilizando o console.
2. Ainda no console, crie um programa para armazenar um número em uma variável.
3. Transfira este conceito para o `editor de texto <../Apoio/idle.html#novo-codigo>`__.

.. activecode:: var

  ano = 2014


4. Defina um tipo texto (chamado *string*) 

.. sourcecode:: python
	
	>>> nome = "Pedro " # atribuição
	>>> sobrenome = "Silva"
	
5. Lembre que os conceitos aritméticos aplicam-se em variáveis.

.. activecode:: concat

  nome = "nome"
  sobrenome = "sobrenome"
  nome_completo = nome + sobrenome
  print(nome_completo)

6. Quais as regras para definir um nome de variável? 

.. admonition:: Definição.

  O nome de uma variável preciasa respeitar algumas regras como:
  
  - não pode começar com números. (ex. ``1a``)
  - não pode possuir caracteres especiais, como símbolos matemáticos (ex. ``1-``)
  - o caracte ``_`` pode ser utilizado para agrupar nomes grandes (ex. ``nome_completo`` é OK)
  
4. Quais os outros *tipos* de informação podemos armazenas numa variável? 

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

.. admonition:: Nota sobre acentuação

		Na Python3 (utilizado na IDLE) podemos utilizar caracteres especiais sem problemas, contudo devido a uma limitação da plataforma, utlizamos a notação ``u" "`` quando nos referimos a trechos de texto (*strings*) com caracteres especiais. 

Para intruduzir o conceito de procedimento, mostre a execução do programa passo a passo, uma idéia:

.. activecode:: nomes_lista

	alunos = []
	nome = input(u"Qual é o seu nome?")
	alunos.append(nome)
	nome = input("Diga outro nome?")
	alunos.append(nome)
	print(alunos)
	

**Proposta** 
	
- Criar uma lista de instruções. 
- Inserir os nomes dos alunos da turma numa lista.


Reflexão
++++++++

- Há problemas para serem automatizados nas aulas de matemática?
- Como podemos organizar nosso cotidiano com estuturas de dados computacionais? 


