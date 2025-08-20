REVIEW QUESTION 1
=================

.. code:: ipython3

    num1 = 25000000      
    num2 = 25_000_000  
    print(num1)
    print(num2)


.. parsed-literal::

    25000000
    25000000
    

.. code:: ipython3

    num = 1.75e5   # 175000.0
    print(num)
    


.. parsed-literal::

    175000.0
    

.. code:: ipython3

    print(2e308)


.. parsed-literal::

    inf
    

REVIEW QUESTION 2
=================

.. code:: ipython3

    base = float(input("Enter the base number: "))
    exponent = float(input("Enter the exponent: "))
    
    result = base ** exponent
    
    print(f"{base} raised to the power of {exponent} is {result}")
    


.. parsed-literal::

    Enter the base number:  1.2
    Enter the exponent:  3
    

.. parsed-literal::

    1.2 raised to the power of 3.0 is 1.7279999999999998
    

REVIEW QUESTION 3
=================

.. code:: ipython3

    num = float(input("Enter a number: "))
    print("Rounded to two decimal places:", round(num, 2))
    


.. parsed-literal::

    Enter a number:  4.432
    

.. parsed-literal::

    Rounded to two decimal places: 4.43
    

.. code:: ipython3

    num = float(input("Enter a number: "))
    print("The absolute value of", abs(num))


.. parsed-literal::

    Enter a number:  -10
    

.. parsed-literal::

    The absolute value of 10.0
    

REVIEW QUESTION 4
=================

.. code:: ipython3

    
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    
    
    difference = num1 - num2
    if difference.is_integer():
        print("The difference is an integer. True!")
    else:
        print("The difference is not an integer. Flase!")
    


.. parsed-literal::

    Enter the first number:  1.5
    Enter the second number:  .5
    

.. parsed-literal::

    The difference is an integer. True!
    

REVIEW QUESTION 5
=================

.. code:: ipython3

    result = 3 ** .125
    print(f"{result:.3f}")
    


.. parsed-literal::

    1.147
    

.. code:: ipython3

    num = 150000
    print(f"{num:.2f}")


.. parsed-literal::

    150000.00
    

.. code:: ipython3

    result = 2 / 10
    print(f"{result:.0%}")
    


.. parsed-literal::

    20%
    

