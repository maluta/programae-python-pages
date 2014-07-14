..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 6: Aventuras no texto (I)
==============================

Objetivos
+++++++++

- Definir uma função própria com ``def``
- Introdução da aventuras em modo texto
- A palavra reservada ``pass``
- Tipos Lógicos (Booleanos)
- Começar a construir um enrredo 


Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
++++++++++

O objetivo das **texto-aventuras** é criar um jogo ficcional e interativo na qual o personagem é levado, de acordo com a opção do jogador, a uma determinada parte do jogo. Iremos utilizar os conceitos aprendidos até então para construir este tipo de narrativa!

Um exemplo: 

.. sourcecode:: python

	Você esta em um mundo cheio de dragões. Na sua frente,
	você vê duas cavernas. Em uma delas, o dragão é seu amigo
	e vai compartilhar o tesouro com você. Na outra o dragão
	é hostil e violento e irá destruí-lo num piscar de olhos. 
	
	Qual das cavernas você deseja entrar (1 ou 2)?
	1

	Você se aproxima da caverna 
	Esta escuro e assustador.
	
	Um dragão enorme salta na sua frente. Ele abre a mandíbula e...
	Te devora em uma mordida.
	
	Você quer jogar de novo? 
	

**Conceitos computacionais**

1. Apresente a estrutura para construção de uma função utilizando a palavra reservada ``def``

.. activecode:: intro

  def intro():
    print(u"Introdução ao jogo")

  def regras():
    print(u"1. regra a")
    print(u"2. regra b")
    print(u"3. regra c")

  intro()
  regras()

É importante destacar:
  - indentação do bloco: espaço ou tab (mas não misture os dois)
  - a definição de função segue o seguinte formato:
  
	``def`` **nome** ``(`` **parametros** ``)`` ``:``
	
  - a função **precisa** executar uma ação, imprimir algo, retornar um valor, etc
  
.. admonition:: Definição

  Se quisermos definir uma função mas ainda não implementar a lógica podemos utilizar a palavra reservada ``pass``


2. Mostre que as fuções podem receber parâmetros e retornar valores. 

.. activecode:: intro1

  def verifica_idade(idade):
    if idade > 15:
	return True
    else:
	return False

  print( verifica_idade(15) )
  print( verifica_idade(16) )

3. ``True`` e ``False`` são palavras reservadas da linguagem. 

4. Apresente alguns conceitos dos operadores Booleanos: ``and``, ``or`` e ``not``.

.. activecode:: intro2

    print( False and False ) # falso
    print( False or False )  # falso
    print()
    print( True and False )  # falso
    print( True or False )   # verdadeiro
    print()
    print( True and True )   # verdadeiro
    print( True or True )    # verdadeiro
    print()
    print ( not False )      # inverte
    print ( not True)
	
**Prosposta**
	
- Reserve um tempo para o grupo discutir e apresentar o enredo da história.
- Fale com os alunos quais poderiam ser as frases do jogo, quais ambientes, quais tipos de perguntas
- Peça uma rápida apresentação (3 min) do enredo 
- Submeta uma votação na classe, o grupo com mais votos irá ganhar 50 progmoney. 
	
Reflexão
++++++++

- Você já conhece alguma texto-aventura?
- Faça uma pesquisa nas histórias existentes.
- Jogos de RPG podem ser automatizados?


