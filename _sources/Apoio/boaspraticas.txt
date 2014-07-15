:orphan:

Boas práticas 
==========================

Indentação
----------

**Definição**

.. image:: ../../_static/indentacao_dicionario.png

(Fonte: dicionário `Priberam <http://www.priberam.pt/dlpo/indenta%C3%A7%C3%A3o>`__)

Temos que ter sempre em mente que a indentação faz toda a diferença na execução do programa, 
podendo ocorrer, em geral, dois tipo de erros:

- na **execução**: o código-fonte simplesmente não executa a ação proposta. 
- de **lógica**: o programa executa mas a lógica apresenta falhas.

Uma maneira de visualmente entender o conceito de indentação é organizar os blocos em execícios como descrito abaixo:

.. parsonsprob:: q1_ind

   Coloque os cada funcionalidade dentro do seu bloco indentado:
   -----
   def maior(a,b):
   =====
      if a &gt; b:
   =====
          return a
   =====
      else:
   =====
          return b

**Exemplos** 

.. image:: ../../_static/i3.png
  

  
  

