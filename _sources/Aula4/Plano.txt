..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 4: Acesso & Controle
=========================

Objetivos
+++++++++

- Utilizar o comando ``import``
- Argumentos para funções
- O conceito e acesso a módulos
- Condicionais 
- Blocos
- Operações de comparações
- Sentenças com ``if``
- Sentenças com ``while``
- A diferença entre ``=`` e ``==``
- A função ``random.randint()``

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
++++++++++

**Conceitos computacionais**

1. Defina o conceito de função, faça analogia com um mini-programa, quando *chamamos* a função ele executa o código definido no mini-programa.
2. Reforce o conceito de parâmetros nas funções previamente utilizadas ``print()`` e ``input()`` onde *passamos* parametros, no primeiro caso o refere-se conteúdo a ser impresso e no último uma descrição (opcional) para o valor a ser imputado. 
3. Apresente o comando ``import`` na qual iremos importar uma "caixa" de funções (esta "caixa" dá-se o nome de módulo). 
4. Após carregar o módulo ``random.randint()`` apresente algumas funcionalidades. 

.. admonition:: Acesso a funções

	Tente invocar uma função sem fazer um ``import``. Faça os alunos pensarem porquê? 


.. activecode:: random

	import random # nossa "caixa" de funcionalidades
	numero = random.randint(1,10)
	print(numero)
	numero = random.randint(1,10)
	print(numero)

5. Os blocos de código são instruções que respeitam a mesma indentação. Reforce a necessidade deles nas instruções a seguir.

6. *Como instruimos o computador a fazer decisões?* Apresente a função ``if`` (*se*).

7. Repetição (*loops*) utilizando o ``while``

8. Comparações matemáticas: ``>`` (*maior que*) ``<`` (*menor que*) ``==`` (*igual que*) e ``!=`` (*diferente de*)

Podemos resumir estes conceitos num jogo de adivinhar o número entre 1 e 20. 

.. sourcecode:: python

	import random
	
	tentativas = 0
	
	print(u"Olá, qual é o seu nome?")
	nome = input()
	
	numero = random.randint(1,20)
	print(u"Olá! " + nome + u"eu estou pensando num número entre 1 e 20")
	print(u"Você consegue adivinhar com apenas 6 tentativas?")
	
	while tentativas < 6:
		print(u"Escreva um valor")
		chute = input()
		chute = int(chute) # converte para o tipo 'int' 

		tentativas = tentativas + 1
		if chute < numero:
			print(u"Você chutou um valor baixo... tente novamente")
			
		if chute > numero:
			print(u"Você digitou um valor muito alto! Tente novamente")
			
		if chute == numero:
			break
		
	if chute == numero:
		tentativas = str(tentativas) # converte para o tipo string
		print(u"Parabéns " + nome + u"!")
		print(u"Você acertou em " + tentativas + u" tentativas.")
	
	if chute != numero:
		numero = str(numero)
		print(u"Que pena... o número que eu estava pensando era " + numero + u".")
		

Explique passo a passo este programa, atentanto para:

- blocos de indentação, o que é código do ``while`` e do ``if``
- condições de execução do ``while``
- condições de execução do ``if``
- as funções de conversão ``int()`` e ``str()`` 
- o comando ``break`` para interromper automaticamente a execução do laço while.

**Proposta** 

- Construir um número para sortear os números da Mega Sena. 

Comandos permitidos:

* ``print()``
* ``input()`` (o grupo que pensar em que podemos fazer jogos com mais de 6 números, utilizando estruturas de controle (``if``), ganhará bônus em progmoney)
* lista ``[]`` e a função ``.append()``
* ``randint()``
	

Reflexão
++++++++

- Como organizar o código fonte com funções?
- Os módulos como "caixas" de funcionalidades.





