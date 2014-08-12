:orphan:

.. role:: raw-math(raw)
    :format: latex html

Exercícios para Aula
======================

Aula `referente <../Aula2/Plano.html>`__

**Perguntas Gerais**


Escreva um programa que utilize as 7 funções matemáticas.

.. reveal:: ex1
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. activecode:: ac11

        print(5 + 5)
        print(5 * 5)
        print(22 / 7)
        print(22 //  7)
        print(22 % 7)
        print(3 ** 4)
        print(9 - 4)


**Grupo 1 - Frações**

Calcule no console do Python o valor das expressões

a) 

.. math::

  (\frac{1}{2} - \frac{1}{3}) - (\frac{1}{6} - \frac{1}{10})

.. reveal:: ex2
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. sourcecode:: python

        >>> (1/2 - 1/2) - (1/6 - 1/10)
          
  
b) 

.. math::

  \frac{1}{3} + \frac{1}{3} + \frac{1}{3}

.. reveal:: ex3
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. sourcecode:: python

        >>> 1/3 + 1/3 + 1/3 
        
    ou
    
    .. sourcecode:: python

        >>> 1/3 * 3
        
           
  
Dado o número decimal, diga a que fração corresponde:

a) 0,55

b) 0,13

c) 0,00098

.. reveal:: ex4
    :showtitle: Ver resposta
    :hidetitle: Ocultar

    .. sourcecode:: python

      from fractions import Fraction
      
      Fraction('0.55')
      Fraction('0.13')
      Fraction('0.00098')
      

      