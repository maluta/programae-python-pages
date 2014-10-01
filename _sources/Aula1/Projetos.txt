..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Projetos
========

A primeira aula não prevê projetos para os alunos, contudo é interessante apresentar alguns códigos para motivá-los para nas próximas aulas.

**Sorteio de equipe**

Execute estes códigos com o alunos, no console do IDLE. Primeiro carregue a biblioteca responsável por lidar com números aleatórios (``import random``) e depois execute quantas vezes for necessário ``random.randint(1,12)`` para sortear os números. Lembre-se que são dois parâmetros: o valor inicial e final, no exemplo abaixo iremos sortear um número entre 1 e 12, lembre-se ajustar o exemplo para o número de alunos da sala.

Dificuldade (★)

.. sourcecode:: python

  >>> import random
  >>> print(random.randint(1,12))

Dependendo do andamento (participação, dúvidas, ...) da sala, você pode propôr algumas **especificações**, como executar mais de uma vez o mesmo comando:

Dificuldade (★★)

.. sourcecode:: python

  >>> import random
  >>> for i in range(12):
        print(randon.randint(1,12))

Por fim, podemos mostrar um exemplo completo, que sorteia equipes de três numa sala com 12 alunos.

Dificuldade (★★★)

.. sourcecode:: python

    #!/usr/bin/python3
    import random

    lista = [] # números que já sairam

    while len(lista) != 12:
        sorteado = random.randint(1,12)
        if sorteado not in lista:
            lista.append(sorteado)

    print("Equipe A", lista[0:3])
    print("Equipe B", lista[3:6])
    print("Equipe C", lista[6:9])
    print("Equipe D", lista[9:12])
