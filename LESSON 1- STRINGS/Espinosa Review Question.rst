Review Question 1:\|
====================

.. code:: ipython3

    my_string = "Hello Revz"
    print(len(my_string))

.. code:: ipython3

    my_string = 'helloRevz'+ 'hello'
    print(my_string)

.. code:: ipython3

    my_string = 'HiRevz ' + 'HelloRevz'
    print(my_string)

.. code:: ipython3

    my_string = "The quick brown fox jumped over the lazy dog. #1234567890!"
    print(my_string[15:19])

REVIEW QUESTION 2:
==================

.. code:: ipython3

    words = ["Animals", "Badger", "Honey Bee", "Honeybadger"]
    for word in words:
        print(word.lower())

.. code:: ipython3

    words = ["Animals", "Badger", "Honey Bee", "Honeybadger"]
    for word in words:
        print(word.upper())

.. code:: ipython3

    string1 = "         Fillet Mignon"
    string2 = "Brisket  "
    print(string1.lstrip())
    print(string2.rstrip())

.. code:: ipython3

    string1 = "Becomes"
    string2 = "becomes"
    print(string1.startswith("be"))
    print(string2.startswith("be"))

.. code:: ipython3

    string1 = "Becomes"
    string2 = "becomes"
    print(string1.startswith("Be"))
    print(string2.startswith("be"))

Review Question 3:
==================

.. code:: ipython3

    user_input = input("Enter something: ")
    
    print("You entered:", user_input)
    

.. code:: ipython3

    user_input = input("Enter something: ")
    
    print("Turn into numbers:", len(user_input))

Review QUestion 4:
==================

.. code:: ipython3

    name = input("Tell me your name: ")
    first_letter = name[0].upper()
    print("The first letter of your name is:", first_letter)
    

Review Question 5:
==================

.. code:: ipython3

    num_str = "100"
    num_int = int(num_str)
    print(num_int * 5)
    

.. code:: ipython3

    num_str = "10.0"
    num_float = float(num_str)
    print(num_float * 5)

.. code:: ipython3

    text = "Age:"
    Age = "21"
    
    print(text + " " + str(Age))

.. code:: ipython3

    num1 = input("Enter first number: ")
    num2 = input("Enter second number: ")
    new_num1=int(num1)
    new_num2=int(num2)
    print("Result", new_num1 * new_num2)
    


.. parsed-literal::

    Enter first number:  5
    Enter second number:  6
    

.. parsed-literal::

    Result 30
    

Review Question 6:
==================

.. code:: ipython3

    print("AAA".find("a"))
    


.. parsed-literal::

    -1
    

.. code:: ipython3

    text = "Somebody said something to Samantha."
    print(text.replace("s", "y"))
    


.. parsed-literal::

    Somebody yaid yomething to Samantha.
    

.. code:: ipython3

    user_text = input("Enter some text: ")
    letter = input("Enter a letter to search for: ")
    position = user_text.find(letter)
    
    print("Position:", position)
    


.. parsed-literal::

    Enter some text:  revz
    Enter a letter to search for:  r
    

.. parsed-literal::

    Position: 0
    

Review Question 7:
==================

.. code:: ipython3

    text = input("Enter some text: ")
    leet = text.lower()
    leet = leet.replace("a", "4")
    leet = leet.replace("b", "8")
    leet = leet.replace("e", "3")
    leet = leet.replace("l", "1")
    leet = leet.replace("o", "0")
    leet = leet.replace("s", "5")
    leet = leet.replace("t", "7")
    
    # Display the result
    print(leet)
    


.. parsed-literal::

    Enter some text:   I like to eat eggs and spam
    

.. parsed-literal::

     i 1ik3 70 347 3gg5 4nd 5p4m
    

