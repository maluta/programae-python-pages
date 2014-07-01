..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Objetivos
----------

- Compreender como uma variável armazena uma informção. 
- Compreender a diferença entre um número e uma *string*
- Ententer o propósito de listas (*list*) e tuplas (*tuple*)


Materiais
----------

- IDLE

Atividades
----------

1. Relembre as primeiras lições abrindo o console e executando um programa
2. Crie um programa para armazenar um número em uma variável 

.. admonition:: Discussão

		Qual o propósito de uma variável? Porquê um programa precisa de uma variável? 

3. Quais os outros tipos de informação podemos armazenas numa variável? Introduza listas. 

4. Tipos de dados.

Faça uma diferenciação nos tipos de dados utilizados, faça uma analogia aos conjuntos.


* Números inteiros
	Exemplos: ``1``, ``2``, ``3``, ``4``, ``5``, ..., ``99``, ...


* Números fracionários
	Exemplos: ``0.0001``, ``0.5``, ``3.14159`` , ``12.5``, ...

* Tipo Texto
	Exemplos: ``"10"``, ``"3.14159", ``"nome"``

* Tipo Lista
	Exemploa: ``[]``, ``"['a','b','c']", ``[1,2,3]``


.. activecode:: Tipos

	print(type(42))
	print(type(3.14))
	print(type("texto"))
	print(type(['a','b','c']))


4. Armazene alguns valores em listas simples (nomes de times de futebol, por exemplo). Remova um item de uma lista e também de uma *string*.

Para intruduzir o conceito de procedimento, mostre a execução do programa passo a passo, uma idéia:

.. codelens:: ex

	alunos = ["Pedro","Maria","Jose"]
	alunos.remove("Jose")
	nome = "pedro"
	nome = nome.replace("p","")

5. Defina uma tupla. Tente remover um elemento. Discuta a utilidade das tuplas. 

6. Utilize marcadores como ``%s`` para colocar   

.. sourcecode:: python
	
	nome = "Pedro"
	idade = 16
	print("%s tem %d" % (nome,idade))

7. Introduza o conceito de jogo-texto de aventura e oriente os alunos a utilizar o que eles sabem até então para começar a construir as sentenças.

.. activecode:: intro_jogo_texto

	print("NOME DO JOGO")
	nome = input("qual seu nome?")
	print("Ola' %s vamos inicar! " % nome)
	idade = input("qual sua idade?")
	if idade > 15:
		print("Escolha as opcoes:")
		# adicione opções aqui
	else:
		print("Você não tem idade para jogar")
	

Avaliação
----------

