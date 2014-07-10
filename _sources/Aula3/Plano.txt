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
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.

Atividades
++++++++++


**Conceitos computacionais**

1. Relembre as funcionalidades do IDLE utilizando o console.
2. Ainda no console, crie um programa para armazenar um número em uma variável.

.. activecode:: var

  ano = 2014

3. Transfira este conceito para o `editor de texto <../Apoio/idle.html#novo-codigo>`__.
4. Defina um tipo (*string*) para armazar textos.

.. sourcecode:: python
	
	>>> nome = "Pedro " 
	>>> sobrenome = "Silva"
	

Repare que o *tipo* da variável é definido no momento que associamos um valor a ela. 
	
5. Verifique quais conceitos aritméticos aplicam-se em variáveis que armazenam números. 

.. activecode:: idade

  ano = 2014
  nascimento = 1998
  idade = ano - nascimento
  print(idade)

Destaque que cada *tipo* de dado permite operações diferentes, por exemplo, se armazenarmos um tipo **string** podemos concatenar (``+``) ou repetir (``*``) mas não subtrair ou dividir. 

.. activecode:: string

  nome = "nome"
  sobrenome = "sobrenome"
  nome_completo = nome + sobrenome
  print(nome_completo)
  print(nome * 5)

  
  
6. Quais as regras para definir um nome de variável? 

.. admonition:: Definição.

  O nome de uma variável preciasa respeitar algumas regras como:
  
  - não pode começar com números. (ex. ``1a``)
  - não pode possuir caracteres especiais, como símbolos matemáticos (ex. ``1-``)
  - o caracte ``_`` pode ser utilizado para agrupar nomes grandes (ex. ``nome_completo`` é OK)
  
7. Quais os outros *tipos* de informação podemos armazenas numa variável? 

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

		Dentro da IDLE podemos utilizar acentuação, contudo devido a uma limitação desta plataforma, utlizamos a notação ``u" "`` quando nos referimos a trechos de texto (*strings*) com acentos.


Ao concatenar uma variável, podemos notar que não existe o espaço em branco entra elas, para tal, podemos definir uma terceira variável que irá armazenar um *espaço em branco*. 

.. activecode:: concat2

	print(u"Qual é o seu primeiro nome?")
	nome = input()
	print(u"Qual é seu sobrenome?")
	sobrenome = input()
	espaco = " "
	print(nome + espaco + sobrenome)
	
.. admonition:: Captura de dados

  A função ``input()`` captura o valor digitado pelo usuário depois que ele aperta a tecla ⏎ (*Enter* ou *return*). No exemplo acima atribuimos este valor 
  a uma variável. 
	
	
**Comentários**

As vezes faz-se necessário explicar com mais detalhes trechos de código, por exemplo, qual motivo de estarmos declarando uma variável chamada ``ano``?
É uma `boa pratica <../Apoio/boaspraticas.html>`__ de programação definir nomes de variáveis capazes de contextualizar seu conteúdo, contudo nem sempre isso é possível e definir nomes
de variáveis exageradamente grandes pode criar problemas de legibilidade do código.  Para tal a linguagem Python permite escrever comentários, 
ou seja, blocos de códigos que serão ignorados pelo computador na hora de transformas o código em linguagem de máquina, existem dois tipo:

- Para comentários de uma **única** linha, utilizamos o caractere ``#``

.. sourcecode:: python

  # define a idade do jogador 
  idade = 10

- Para comentários de **múltiplas** linhas, utilizamos ``"""`` ou ``'''``

.. sourcecode:: python

  """
  Este é um exemplo de comentário
  em várias linhas, e o que esta dentro deste bloco
  não será executado, a variável abaixo não será definida.
  idade = 10
  """
  
.. admonition:: Bônus

  Como declarar diversas variáveis com uma única linha de código?
    Apenas separe cada uma com ``,`` e depois do ``=`` atribua o conteúdo respectivo.
  
.. activecode:: bonus

     # multiplas definições com uma linha de código
     nome, sobrenome, idade = u"José", u"Silva", 20
     print(nome,sobrenome,idade)


	
**Proposta** 
	
1. Combine com os alunos um padrão paro os arquivos, que tipo de conteúdo seria interessante acrescentar na forma de comentários?

Algumas dicas:

- `Meta <http://pt.wikipedia.org/wiki/Metadados>`__-informações: nome do arquivo, data, autores, descrição, contato, quais outros campos poderiam ser utilizados? 
- Permissões de uso, apresente como opção as licenças `Creative Commons <http://creativecommons.org/choose/?lang=pt_BR>`__. 

Um exemplo de cabeçalho:

.. sourcecode:: python

  """
  idade.py - programa que calcula a idade
  
  Licença: CC BY-SA
  
  Autores: Lucas <lucas@programae.org.br>
	   Tiago <tiago@programae.org.br>
	    
  Data: 18/08/2014
  
  Versão: 1.0
  
  """

2. Defina uma variável chama ``__autor__`` que deverá ser sempre preenchiada com o nome da empresa escolhida por cada grupo.

.. sourcecode:: python

  __autor__ = 'empresa' 
  


Reflexão
++++++++



