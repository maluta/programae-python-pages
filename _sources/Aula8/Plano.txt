..  Copyright (C)  Fundação Lemann

    Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Aula 3: Funções 
============================

Objetivos
+++++++++

- Aprender a declarar funções

Preparação
++++++++++

- IDLE - Veja na seção de ajuda `Como instalar o Python <../Apoio/comoinstalar.html>`__ 
- `Editar <../Apoio/idle.html#sugestao-de-layout>`__ e `executar <../Apoio/idle.html#executando-um-codigo>`__ códigos no IDLE.


Atividades 
++++++++++

**Conceitos computacionais**

Funções são uma espécie de "*mini*-programa" dentro do código que permite executá-lo facilmente.
Além de utilizar demonstre que podemos construir as nossas próprias funções, a linguagem Python possui uma palavra reservada para tal: ``def``.

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


A escolha do nome de um função segue as mesmas regras das variáveis.
  
  
**Prosposta**

- Construir funções simples para operações aritméticas. 
- Como colocar dentro de funções o quê aprendemos nas ultimas aulas?

Reflexão
++++++++

Nesta aula é importante que todos tenham compreendido a estrutura básica de funções e sua necessidade.
A partir de agora o uso de funções será utilizado amplamente e é preciso que os alunos explorem bastante seu uso. 

- O que fizemos e que funcionou?
- O que fizemos e que não funcionou?
- Quais as dúvidas mais comuns que apareceram durante a aula? 
- Qual as maiores dificuldades na execução das atividades? 



