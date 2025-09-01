REVIEW QUESTION 1
=================

.. code:: ipython3

    
    def cube(number):
        return number ** 3  
    
    print("cube(2) =", cube(2))   
    print("cube(3) =", cube(3))    
    


.. parsed-literal::

    cube(2) = 8
    cube(3) = 27
    

.. code:: ipython3

    def greet(name):
        return("Hi" + " " + name + "!")
    print(greet("zekoy"))


.. parsed-literal::

    Hi zekoy!
    

Challenge Question
==================

.. code:: ipython3

    def convert_cel_to_far(celsius: float) -> float:
        return (celsius * 9/5) + 32
    
    def convert_far_to_cel(fahrenheit: float) -> float:
        return (fahrenheit - 32) * 5/9
    
    fahrenheit = float(input("Enter a temperature in degrees F: "))
    celsius = convert_far_to_cel(fahrenheit)
    print(f"{fahrenheit} degrees F = {celsius:.2f} degrees C")
    
    
    
    celsius = float(input("\nEnter a temperature in degrees C: "))
    fahrenheit = convert_cel_to_far(celsius)
    print(f"{celsius} degrees C = {fahrenheit:.2f} degrees F")
    


.. parsed-literal::

    Enter a temperature in degrees F:  72
    

.. parsed-literal::

    72.0 degrees F = 22.22 degrees C
    

.. parsed-literal::

    
    Enter a temperature in degrees C:  72
    

.. parsed-literal::

    72.0 degrees C = 161.60 degrees F
    

REVIEW QUESTION 2
=================

.. code:: ipython3

    for i in range(2, 11):
        print(i)
    


.. parsed-literal::

    2
    3
    4
    5
    6
    7
    8
    9
    10
    

.. code:: ipython3

    num = 2
    while num <= 10:
        print(num)
        num += 1  
        
    


.. parsed-literal::

    2
    3
    4
    5
    6
    7
    8
    9
    10
    

.. code:: ipython3

    def doubles(number):
        return number * 2
    value = int(input("Enter a number to double: "))
    for i in range(3):
        value = doubles(value)
        print(value)
    


.. parsed-literal::

    Enter a number to double:  2
    

.. parsed-literal::

    4
    8
    16
    

