Review Exercise
===============

.. code:: ipython3

    1 <= 1




.. parsed-literal::

    True



.. code:: ipython3

    1 != 1




.. parsed-literal::

    False



.. code:: ipython3

    1 != 2




.. parsed-literal::

    True



.. code:: ipython3

    "good" != "bad"




.. parsed-literal::

    True



.. code:: ipython3

    "good" != "Good"




.. parsed-literal::

    True



.. code:: ipython3

    123 == "123"




.. parsed-literal::

    False



2
=

.. code:: ipython3

    3 < 4 




.. parsed-literal::

    True



.. code:: ipython3

    10 > 5




.. parsed-literal::

    True



.. code:: ipython3

    "jack" != "jill"




.. parsed-literal::

    True



.. code:: ipython3

    42 == "42"




.. parsed-literal::

    False



Review Exercise 2
=================

.. code:: ipython3

    (1 <= 1) and (1 != 1)
    not (1 != 2)




.. parsed-literal::

    False



.. code:: ipython3

    ("good" != "bad" ) or false




.. parsed-literal::

    True



.. code:: ipython3

    ("good" != "Good") and not (1 == 1)




.. parsed-literal::

    False



2
=

.. code:: ipython3

    False == (not True)
    




.. parsed-literal::

    True



.. code:: ipython3

    (True and False) == (True and False) 




.. parsed-literal::

    True



.. code:: ipython3

    not (True and "A" == "B")




.. parsed-literal::

    True



Review Exercise 3
=================

.. code:: ipython3

    word = input("Enter a word:")
    
    if len(word) < 5:
        print("The len of word is less than 5 characters.")
    elif len(word) > 5:
        print("The len of word is greater than 5 characters.")
    else:
        print("The len of word is Exactly 5 characters.")


.. parsed-literal::

    Enter a word: zekoylovecagas
    

.. parsed-literal::

    The len of word is greater than 5 characters.
    

Review Exercise 4
=================

.. code:: ipython3

    while True:
        user_input = input("Enter something (or 'Q' to quit): ")
        if user_input == 'Q' or user_input == 'q':
            print("Quitting the program...")
            break
        else:
            print(f"You entered: {user_input}")
    


.. parsed-literal::

    Enter something (or 'Q' to quit):  s
    

.. parsed-literal::

    You entered: s
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  d
    

.. parsed-literal::

    You entered: d
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  f
    

.. parsed-literal::

    You entered: f
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  a
    

.. parsed-literal::

    You entered: a
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  s
    

.. parsed-literal::

    You entered: s
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  d
    

.. parsed-literal::

    You entered: d
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  f
    

.. parsed-literal::

    You entered: f
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  g
    

.. parsed-literal::

    You entered: g
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  h
    

.. parsed-literal::

    You entered: h
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  
    

.. parsed-literal::

    You entered: 
    

.. parsed-literal::

    Enter something (or 'Q' to quit):  q
    

.. parsed-literal::

    Quitting the program...
    

.. code:: ipython3

    for number in range(2, 67):
        if number % 3 == 0:
            continue  # Skip multiples of 3
        print(number)
    


.. parsed-literal::

    2
    4
    5
    7
    8
    10
    11
    13
    14
    16
    17
    19
    20
    22
    23
    25
    26
    28
    29
    31
    32
    34
    35
    37
    38
    40
    41
    43
    44
    46
    47
    49
    50
    52
    53
    55
    56
    58
    59
    61
    62
    64
    65
    

