..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 5: Mais com textos
=======================

Objetivos
+++++++++

- Experimentar possibilidades com o comando ``print()``
- Verificar o tamanho da string com a instrução ``len()``
- Concatenação de strings
- Fatiamento de strings
- Métodos *comuns* para strings

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 


Atividades
++++++++++

**Conceitos computacionais** 

1. Começe por definir uma string simple, entre aspas (*lembre-se do ``u""`` apresentado na aula aterior se for utilizar acentuação*)

.. admonition:: "" ou ''?

	Tanto faz. Você pode usar ``print('texto')`` ou ``print("texto")``


2. Armazene e imprima numa variável 
3. Mostre como contar o número de caracteres com a função ``len()`` 

.. activecode:: strings1

	 texto = u"programar é muito bom"
	 print(texto)
	 print(len(texto))

4. Reforce a questão de indice da string, demonstrando a forma de acessar.
5. Fatiamento de strings.

.. activecode:: strings2

	 texto = u"programar É muito bom"
	 print(texto[0]) # primeiro caractere
	 print(texto[:9]) # do ínicio (índice zero) até o índice 8
	 print(texto[10:11]) # apenas o índice 10
	 print(texto[12:17]) # do índice 12 até o 16
	 print(texto[18:]) # do índice 18 até o final
	 
Pontos importantes: 

- O índice da string começa em "0"
- Não se esqueça que o espaço em branco ``" "`` também está no índice. 
- Para acessar um único caracter utilizamos: ``texto[índice]``
- Para um fatiamento pode ser completo utilizamos **posição de início** ``:`` **posição final** (mas em incluí-la).

6. Trabalhe funções comuns para manipular strings

.. activecode:: strings3

	texto = u"programar É muito bom"
	print( texto ) # texto original
	print( texto.upper() ) # todo o texto em letras maiúsculas
	print( texto.lower() ) # todo o texto em letras minúsculas
	print( texto.capitalize() ) # texto com a primeira letra maiúscula
	print( texto.count('a') ) # quantas vezes a letra 'a' aparece
	print( texto.find('a') ) # retorna o índice da primeira ocorrência da letra 'a'
	print( texto.replace(' ','_') ) # substitui todos os espaços em branco por '_'
	
.. admonition:: Caracteres de escape (``\``)

	- barra invertida ``\\`` 
	- aspas simples ``\'`` 
	- aspas duplas ``\"`` 
	- quebra de linha ``\n``
	- seção tabular ``\t``

**Proposta** 

- Impressão de poesias (haikais) com ``print()`` e o delimitador ``\t``

.. activecode:: strings4

	texto="Pra que cara feia?\n\tNa vida,\nNinguém paga meia.\n\n(Paulo Leminski)"
	print(texto)

- Construir um validador de *twitts*. Como saber se meu texto "cabe" dentro de uma mensagem no **Twitter** (limite de 140 caracteres)
- Construir um buscador de palavras no textual 


Reflexão
++++++++

- Onde este tipo de manipulação pode ser utilizado nas aulas de literatura/português?

