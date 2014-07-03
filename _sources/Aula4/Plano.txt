..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 4
---------

Objetivos
+++++++++

- Argumentos para funções
- Utilizar o comando ``import``
- O conceito e acesso a módulos
- Condicionais ``if``
- Comparações

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
++++++++++

**Conceitos computacionais**

1. Defina o conceito de função, faça analogia com um mini-programa, quando *chamamos*
a função ele executa o código definido no mini-programa.
2. Reforce o conceito de parâmetros nas funções previamente utilizadas 
``print()`` e ``input()`` onde *passamos* parametros. 
3. Apresente o comando ``import`` na qual iremos importar uma "caixa" de funções 
(esta "caixa" dá-se o nome de módulo). 
4. Após carregar o módulo ``random`` apresente algumas funcionalidades. 

.. activecode:: random

	import random # nossa caixa de funcionalidades
	numero = random.randint(1,10)
	print(numero)
	numero = random.randint(1,10)
	print(numero)

5. *Como instruimos o computador a fazer decisões?* Apresente a função ``if`` (se).

.. activecode:: intro_jogo_texto

	print("<<NOME DO JOGO>>>")
	nome = input("qual seu nome?")
	print("Ola' %s vamos inicar! " % nome)
	idade = input("qual sua idade?")
	if idade > 15:
		print("Escolha as opcoes:")
		print("1. Carro")
		print("2. Moto")
		print("3. Bicicleta")
	else:
		print("Voce nao tem idade para jogar")

**Proposta** 

- Construir um número para sortear os números da Megasena. 
	
	
Reflexão
++++++++




