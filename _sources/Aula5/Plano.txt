..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 5: Funções
============================

Objetivos
+++++++++

- Aprender a construir e utilizar funções
- Inicio dos projetos das empresas

Preparação
++++++++++

- Se ainda não possui o IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__
- Conferir se as funcionalidades `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE estã funcionando corretamente.


Atividades
++++++++++

**Conceitos computacionais necessários**

Faça os `exercícios de funções <http://www.codecademy.com/pt-BR/courses/python-beginner-pt-BR-30pxi/0/1>`_ do Codecademy.

.. admonition:: Reuso

  É importante trabalhar com os alunos a importância das funções com uma ferramenta para re-aproveitamento do código.

Alguns sinônimos para funções:

- mini-programa
- código reutilizável


**Na sala de aula**

1. Abra o Editor de Texto do IDLE e mostre como declarar uma função.


Exemplo:

.. activecode:: aula8_ex1

  def minha_funcao():
    print(u"código")
    print(u"da")
    print(u"função")


Execute o código e proponha as seguintes perguntas:

- Qual a saída deste trecho de código?
- O que é necessário para vermos a execução do ``print``


É importante destacar:
  - `indentação <../Apoio/boaspraticas.html#indentacao>`__ do bloco: 4 espaços ou *tab*.
  - a definição de função segue o seguinte formato:

  ``def`` **nome** ``(`` **parametros** ``)`` ``:``

     # seu código aqui

     **return** valor

Da mesma forma que passamos parâmetros para as funções ``print()``, ``len()``, ``input()``, ``range()`` nas aulas anteriores, podemos criar nossas
próprias funções com inúmeros parâmetros bem como retornar valores das funções. Um exemplo de função para somar dois números x e y:

.. activecode:: aula8_ex2

  def soma(x,y):
    return x + y

  print(soma(5,4))

**A escolha do nome de um função segue as mesmas regras das variáveis.**



**Prosposta**

- Construir funções simples para operações aritméticas.
- Como colocar dentro de funções o quê aprendemos nas ultimas aulas?

**Exercícios**

1. Fazer uma função que imprima o nome de cada um dos membros das equipe.

.. reveal:: ex1
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. sourcecode:: python

        def imprime_nomes():
          print("Nome 1")
          print("Nome 1")
          print("Nome 1")

        imprime_nomes()


2. Fazer uma função que retorne a soma das idades de cada um dos membros da equipe (lembre de converter para inteiro, é um erro que os alunos comentem com frequência)

.. reveal:: ex2
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. sourcecode:: python

        def retorna_soma():
          idade1 = input("Qual a idade da pessoa #1? ")
          idade2 = input("Qual a idade da pessoa #2? ")
          idade3 = input("Qual a idade da pessoa #3? ")
          soma = int(idade1) + int(idade2) + int(idade3)
          return soma

        print(retorna_soma())

**Gamification: atividades para o jogo**

Proponha uma reflexão de como eles irão utilizar funções na construção dos seus
programas e jogos. Proponha a atividade para fazer um **validador de idade** para o jogo e
o **about** (ou seja, a função que imprime os autores do programa)


1. Validador de Idade

.. sourcecode:: python

  def valida_idade():
    idade = input("Qual sua idade? ")
    if int(idade) >= 15:
      print("Bem-vindo ao jogo")
      return True
    else:
      print("Você não pode jogar!")
      return False

  # precisamos invocar (chamar) a função
  valida_idade()

Se eles tiverem dúvidas no `if` fale que ele será abordado com mais detalhes na próxima aula.

2. Sobre (About)

.. sourcecode:: python

  def sobre():
    print("Este programa foi desenvolvido por:")
    print("1. Fulano")
    print("2. Ciclano")
    print("3. Beltrano")

  sobre() # chama a função

Peça para que eles salvem o arquivo no editor e enviem para seu e-mail.

Caso sobre um tempo, mostre o `Gist <https://gist.github.com/>`_ para armazenar trechos de código.


Reflexão
++++++++

Nesta aula é importante que todos tenham compreendido a estrutura básica de funções e sua necessidade.
A partir de agora o uso de funções será utilizado amplamente e é preciso que os alunos explorem bastante seu uso.

- O que fizemos e que funcionou?
- O que fizemos e que não funcionou?
- Quais as dúvidas mais comuns que apareceram durante a aula?
- Qual as maiores dificuldades na execução das atividades?
