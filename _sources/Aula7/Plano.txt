..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 7: Textos
=======================

Objetivos
+++++++++

- Experimentar possibilidades de uso do comando ``print()``
- Verificar o tamanho da string com a instrução ``len()``
- Concatenação de strings
- Fatiamento de strings
- Métodos *comuns* para strings

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.

Atividades
++++++++++

**Conceitos computacionais** 

1. Comece por definir uma string simples, entre aspas.

.. admonition:: Aspas duplas ou simples?

	Desde que exista um padrão, tanto faz. Você pode usar ``print('texto')`` ou ``print("texto")``


2. Armazene e imprima o conteúdo de variável 
3. Mostre como contar o número de caracteres com a função ``len()`` 

.. activecode:: strings1

	 texto = u"programar é muito bom"
	 print(texto)
	 print(len(texto))

4. Reforce a questão de índices dentro do tipo string, demonstrando as formas de acesso. Você pode fazer isso de maneira fácil no `console <../Apoio/idle.html#console-iterativo>`__. 

.. sourcecode:: python

  >>> "Programaê"[0]
  'P'
  >>> "Programaê"[8]
  'ê'
  >>> "Programaê"[9]
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  IndexError: string index out of range


A palavra "Programaê" tem 9 caracteres. O primeiro ``[0]`` e o último ``[8]``, ao tentarmos acessar um índice acima, ex ``[10]`` obtemos 
um erro indicando que o índice esta fora da faixa permitida. 

5. Fatiamento de strings.

.. activecode:: strings2

	 texto = u"programar É muito bom"
	 print(texto[0]) # primeiro caractere
	 print(texto[:9]) # do ínicio (índice zero) até o índice 8
	 print(texto[10:11]) # apenas o índice 10
	 print(texto[12:17]) # do índice 12 até o 16
	 print(texto[18:]) # do índice 18 até o final
	 
Pontos importantes: 

- O índice da string sempre começa em "0" (o primeiro item é a posição zero)
- Não se esqueça que espaços em branco ``" "`` também são considerados. 

- Para acessar um único caracter utilizamos: ``texto[índice]``
- Para um fatiamento pode ser completo utilizamos **posição de início** ``:`` **posição final** (mas em incluí-la).

6. Trabalhe funções comuns para manipular strings

.. activecode:: s3

	texto = u"programar É muito bom"
	print( texto ) # texto original
	print( texto.upper() ) # todo o texto em letras maiúsculas
	print( texto.lower() ) # todo o texto em letras minúsculas
	print( texto.capitalize() ) # texto com a primeira letra maiúscula
	print( texto.count('a') ) # quantas vezes a letra 'a' aparece
	
	
.. admonition:: Funções mais avançadas: encontrar & substituir

  As funções ``find`` e ``replace`` são sugestões para demonstrar o processo de encontrar e substituir textos.
  
  .. sourcecode:: python
  
    # retorna o índice da primeira ocorrência da letra 'a'
    print( u"programar É muito bom".find('a') ) 
    
    # substitui todos os espaços em branco por '_'
    print( u"programar É muito bom".replace(' ','_') ) 
	

É possível deixar o texto mais amigável introduzindo quebras de linha ou caracteres especiais. Por exemplo, 
como adicionar uma aspas se ela é o delimitador do tipo string? A linguagem Python oferece um caractere de *escape*, 
ou seja, tudo que estiver em seguida ao ``\`` irá ser ignorado pelo interprador. Alguns exemplos:

.. admonition:: Caracteres de escape (``\``)

	- barra invertida ``\\`` 
	- aspas simples ``\'`` 
	- aspas duplas ``\"`` 
	- quebra de linha ``\n``
	- seção tabular ``\t``

Um erro comum acontece ao definirmos uma *string*. Ao utilizarmos um caractere de escape para introduzir uma aspa e esquecermos 
fechá-la obteremos um erro de sintaxe, descrito no exemplo abaixo: 
	
.. sourcecode:: python
   
  >>> print("programaê\")
  File "<stdin>", line 1
    print("programaê\")
                       ^
  SyntaxError: EOL while scanning string literal

**Percorrendo strings** 

Na `aula anterior <../Aula6/Plano.html>`__ aprendemos um uso do ``for`` para percorrer uma faixa de números. Incentive os alunos a pensar 
como utilizar os tópicos aprendidos na aula de hoje pare ensinar percorrer uma string. 

Utilize este pequeno programa para mostrar a execução no modo passo a passo. 

.. codelens:: s5

  texto = "meu texto"  
  tamanho = len(texto)
  for pos in range(tamanho): 
    caractere = texto[pos]
    print(caractere)


Mas se pensarmos uma string como uma lista de caracteres? 
Podemos aplicar a mesma idéia ara percorrer uma *string*.

.. activecode:: s6

  for caractere in "meu texto":
    print(caractere)
  

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

