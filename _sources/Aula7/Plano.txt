..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 7: Aventuras no texto (II)
===============================

Objetivos
+++++++++

- Aprender o conceito de dicionários 
- Aprender o conceito de tuplas
- Construir o enrredo da história (transições)


Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 

Atividades
++++++++++

**Conceitos computacionais**

1. Tuplas 

São semelhantes as listas, exceto que eles não permitem alterações. Um Exemplo prático para demonstrar são os meses do ano.

.. activecode:: tuple

  meses = ("Janeiro","Fevereiro", u"Março","Abril",
           "Maio","Junho","Julho","Agosto","Setembro",
           "Outubro","Novembro","Dezembro")
  print(meses)
           
.. admonition:: Tuplas com um único elemento

  Uma tupla unitária precisa ser definida como ``( valor, )`` caso contrário será definido com o *tipo* do valor. 

2. Dicionários.

Dicionários sao similiares a outros tipos compostos exceto por eles poderem user qualquer tipo imutavel de dados como indice. Como exemplo, nos criaremos um dicionário para traduzir palavras em Inglês para Espanhol. Para esse dicionário, os indices serão strings.

.. activecode:: dict

  dicionario = {
                  'car':u"carro",
                  'bus':u"ônibus"
               }
               
  print( dicionario['car'] )
  print( dicionario['bus'] )
  print( dicionario.keys() )
  
**Enrredo**

1. Na construção da história os lugares são tuplas
2. Na construção da história as transições são dicionários

.. activecode:: transictions

  sala = ( "sala", u"Você está na sala principal da mansão")
  quarto = ( "quarto", u"Você esta no quarto")
  cozinha = ( "cozinha", u"Você esta na cozinha" ) 
  
  transicoes = { # da ____ : você pode ir para ( ____ , ____ , ...)
                  sala: (quarto, cozinha),
                  quarto: (sala, cozinha),
                  cozinha: (quarto, sala)
               } 

**Prosposta**

- Proponha a continuação da aula passada com os alunos construindo as ações. 

Reflexão
++++++++

- Você já conhece alguma texto-aventura?
- Faça uma pesquisa nas histórias existentes.
- Jogos de RPG podem ser automatizados?



