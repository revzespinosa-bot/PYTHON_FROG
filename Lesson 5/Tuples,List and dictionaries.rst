Review Exercise 1
=================

.. code:: ipython3

    CARDINAL_NUMBERS = ("FIRST", "SECOND", "THIRD")
    
    print (CARDINAL_NUMBERS[1])


.. parsed-literal::

    SECOND
    

.. code:: ipython3

    POSITION1, POSITION2, POSITION3 = CARDINAL_NUMBERS
    print(POSITION1)
    print(POSITION2)
    print(POSITION3)
    


.. parsed-literal::

    FIRST
    SECOND
    THIRD
    

.. code:: ipython3

    MY_NAME = tuple("REVZESPINOSA")  
    print(MY_NAME)
    


.. parsed-literal::

    ('R', 'E', 'V', 'Z', 'E', 'S', 'P', 'I', 'N', 'O', 'S', 'A')
    

.. code:: ipython3

    print("X" in MY_NAME)
    


.. parsed-literal::

    False
    

.. code:: ipython3

    MY_NAME_NO_FIRST = MY_NAME[1:]
    print(MY_NAME_NO_FIRST)
    


.. parsed-literal::

    ('E', 'V', 'Z', 'E', 'S', 'P', 'I', 'N', 'O', 'S', 'A')
    

Review Exercise 2
=================

.. code:: ipython3

    FOOD = ["RICE", "BEANS"]
    FOOD.append("BROCCOLI")
    print(FOOD)


.. parsed-literal::

    ['RICE', 'BEANS', 'BROCCOLI']
    

.. code:: ipython3

    FOOD = ["RICE", "BEANS"]
    FOOD.append("BROCCOLI")
    FOOD.extend(["BREAD","PIZZA"])
    print(FOOD)


.. parsed-literal::

    ['RICE', 'BEANS', 'BROCCOLI', 'BREAD', 'PIZZA']
    

.. code:: ipython3

    FOOD = ["RICE", "BEANS"]
    FOOD.append("BROCCOLI")
    FOOD.extend(["BREAD","PIZZA"])
    print(FOOD[:2])


.. parsed-literal::

    ['RICE', 'BEANS']
    

.. code:: ipython3

    FOOD = ["RICE", "BEANS"]
    FOOD.append("BROCCOLI")
    FOOD.extend(["BREAD","PIZZA"])
    print(FOOD[-1])


.. parsed-literal::

    PIZZA
    

.. code:: ipython3

    BREAKFAST = "EGGS, FRUIT, ORANGE JUICE".split(", ")
    print(len(BREAKFAST))
    


.. parsed-literal::

    3
    

.. code:: ipython3

    BREAKFAST = "EGGS, FRUIT, ORANGE JUICE".split(", ")
    LENGTHS = [len(item) for item in BREAKFAST]
    print (LENGTHS)


.. parsed-literal::

    [4, 5, 12]
    

Review Exercise 3
=================

.. code:: ipython3

    DATA = ((1, 2), (3, 4))
    print(DATA[0])
    print(DATA[1])
    


.. parsed-literal::

    (1, 2)
    (3, 4)
    

.. code:: ipython3

    DATA = ((1, 2), (3, 4))
    
    for i, nested_tuple in enumerate(DATA, start=1):
        total = sum(nested_tuple)
        print(f"row {i} is {total}")
    


.. parsed-literal::

    row 1 is 3
    row 2 is 7
    

.. code:: ipython3

    
    numbers = [12, 5, 9, 1, 20, 3]
    
    
    numbers_copy = numbers[:]
    print("Copy of numbers:", numbers_copy)
    
    numbers.sort()
    print("Sorted numbers:", numbers)
    


.. parsed-literal::

    Copy of numbers: [12, 5, 9, 1, 20, 3]
    Sorted numbers: [1, 3, 5, 9, 12, 20]
    

Challenge question
==================

.. code:: ipython3

    # Challenge: List of Lists
    
    universities = [
        ['California Institute of Technology', 2175, 37704],
        ['Harvard', 19627, 39849],
        ['Massachusetts Institute of Technology', 10566, 40732],
        ['Princeton', 7802, 37000],
        ['Rice', 5879, 35551],
        ['Stanford', 19535, 40569],
        ['Yale', 11701, 40500]
    ]
    
    # Print all universities
    print("List of Universities:")
    for uni in universities:
        print(uni)
    
    # Example: Print just the names
    print("\nUniversity Names:")
    for uni in universities:
        print(uni[0])
    
    # Example: Print name and tuition
    print("\nUniversity Name and Tuition:")
    for uni in universities:
        print(f"{uni[0]} - Tuition: ${uni[2]}")
    


.. parsed-literal::

    List of Universities:
    ['California Institute of Technology', 2175, 37704]
    ['Harvard', 19627, 39849]
    ['Massachusetts Institute of Technology', 10566, 40732]
    ['Princeton', 7802, 37000]
    ['Rice', 5879, 35551]
    ['Stanford', 19535, 40569]
    ['Yale', 11701, 40500]
    
    University Names:
    California Institute of Technology
    Harvard
    Massachusetts Institute of Technology
    Princeton
    Rice
    Stanford
    Yale
    
    University Name and Tuition:
    California Institute of Technology - Tuition: $37704
    Harvard - Tuition: $39849
    Massachusetts Institute of Technology - Tuition: $40732
    Princeton - Tuition: $37000
    Rice - Tuition: $35551
    Stanford - Tuition: $40569
    Yale - Tuition: $40500
    

.. code:: ipython3

    # List of nouns
    nouns = ["FOSSIL", "HORSE", "AARDVARK", "JUDGE", "CHEF", "MANGO", "EXTROVERT", "GORILLA"]
    
    # List of verbs
    verbs = ["KICKS", "JINGLES", "BOUNCES", "SLURPS", "MEOWS", "EXPLODES", "CURDLES"]
    
    # List of adjectives
    adjectives = ["FURRY", "BALDING", "INCREDULOUS", "FRAGRANT", "EXUBERANT", "GLISTENING"]
    
    # List of prepositions
    prepositions = ["AGAINST", "AFTER", "INTO", "BENEATH", "UPON", "FOR", "IN", "LIKE", "OVER", "WITHIN"]
    
    # List of adverbs
    adverbs = ["CURIOUSLY", "FURIOUSLY", "SENSUOUSLY", "EXTRAVAGANTLY", "TANTALIZINGLY"]
    
    # Print all lists
    print("Nouns:", nouns)
    print("Verbs:", verbs)
    print("Adjectives:", adjectives)
    print("Prepositions:", prepositions)
    print("Adverbs:", adverbs)
    


.. parsed-literal::

    Nouns: ['FOSSIL', 'HORSE', 'AARDVARK', 'JUDGE', 'CHEF', 'MANGO', 'EXTROVERT', 'GORILLA']
    Verbs: ['KICKS', 'JINGLES', 'BOUNCES', 'SLURPS', 'MEOWS', 'EXPLODES', 'CURDLES']
    Adjectives: ['FURRY', 'BALDING', 'INCREDULOUS', 'FRAGRANT', 'EXUBERANT', 'GLISTENING']
    Prepositions: ['AGAINST', 'AFTER', 'INTO', 'BENEATH', 'UPON', 'FOR', 'IN', 'LIKE', 'OVER', 'WITHIN']
    Adverbs: ['CURIOUSLY', 'FURIOUSLY', 'SENSUOUSLY', 'EXTRAVAGANTLY', 'TANTALIZINGLY']
    

Review Execise 4
================

.. code:: ipython3

    # Create an empty dictionary named captains
    captains = {'Enterprices': 'Picard','Voyager':'Janeway','Defiant': 'Sisko'}
    
    print(captains)  # Output: {}
    


.. parsed-literal::

    {'Enterprices': 'Picard', 'Voyager': 'Janeway', 'Defiant': 'Sisko'}
    

.. code:: ipython3

    captains = {'Enterprices': 'Picard', 'Voyager': 'Janeway', 'Defiant': 'Sisko'}
    
    # Check if "ENTERPRISE" exists
    if "ENTERPRISE" not in captains:
        captains["ENTERPRISE"] = "UNKNOWN"
    
    # Check if "DISCOVERY" exists
    if "DISCOVERY" not in captains:
        captains["DISCOVERY"] = "UNKNOWN"
    
    print(captains)
    


.. parsed-literal::

    {'Enterprices': 'Picard', 'Voyager': 'Janeway', 'Defiant': 'Sisko', 'ENTERPRISE': 'UNKNOWN', 'DISCOVERY': 'UNKNOWN'}
    

.. code:: ipython3

    captains = {
        'Enterprise': 'Picard',
        'Voyager': 'Janeway',
        'Defiant': 'Sisko',
        'Discovery': 'Lorca'
    }
    
    # For loop to display ships and captains
    for ship, captain in captains.items():
        print(f"The {ship} is captained by {captain}.")
    


.. parsed-literal::

    The Enterprise is captained by Picard.
    The Voyager is captained by Janeway.
    The Defiant is captained by Sisko.
    The Discovery is captained by Lorca.
    

Review Exercise 5
=================

.. code:: ipython3

    captains = {
        'Enterprise': 'Picard',
        'Voyager': 'Janeway',
        'Defiant': 'Sisko',
        'Discovery': 'Lorca'
    }
    
    # Delete "Discovery"
    del captains["Discovery"]
    
    print(captains)
    


.. parsed-literal::

    {'Enterprise': 'Picard', 'Voyager': 'Janeway', 'Defiant': 'Sisko'}
    

.. code:: ipython3

    captains = dict(
        Enterprise="Picard",
        Voyager="Janeway",
        Defiant="Sisko",
        Discovery="Lorca"
    )
    
    print(captains)
    


.. parsed-literal::

    {'Enterprise': 'Picard', 'Voyager': 'Janeway', 'Defiant': 'Sisko', 'Discovery': 'Lorca'}
    

Challenge Exercise
==================

.. code:: ipython3

    capitals_dict = {
        'Alabama': 'Montgomery',
        'Alaska': 'Juneau',
        'Arizona': 'Phoenix',
        'Arkansas': 'Little Rock',
        'California': 'Sacramento',
        'Colorado': 'Denver',
        'Connecticut': 'Hartford',
        'Delaware': 'Dover',
        'Florida': 'Tallahassee',
        'Georgia': 'Atlanta'
    }
    
    # Loop through dictionary and display state with capital
    for state, capital in capitals_dict.items():
        print(f"The capital of {state} is {capital}.")
    


.. parsed-literal::

    The capital of Alabama is Montgomery.
    The capital of Alaska is Juneau.
    The capital of Arizona is Phoenix.
    The capital of Arkansas is Little Rock.
    The capital of California is Sacramento.
    The capital of Colorado is Denver.
    The capital of Connecticut is Hartford.
    The capital of Delaware is Dover.
    The capital of Florida is Tallahassee.
    The capital of Georgia is Atlanta.
    

.. code:: ipython3

    capitals_dict = {
        'Alabama': 'Montgomery',
        'Alaska': 'Juneau',
        'Arizona': 'Phoenix',
        'Arkansas': 'Little Rock',
        'California': 'Sacramento',
        'Colorado': 'Denver',
        'Connecticut': 'Hartford',
        'Delaware': 'Dover',
        'Florida': 'Tallahassee',
        'Georgia': 'Atlanta'
    }
    
    # Loop through dictionary in alphabetical order by state
    for state in sorted(capitals_dict.keys()):
        print(f"The capital of {state} is {capitals_dict[state]}.")
    


.. parsed-literal::

    The capital of Alabama is Montgomery.
    The capital of Alaska is Juneau.
    The capital of Arizona is Phoenix.
    The capital of Arkansas is Little Rock.
    The capital of California is Sacramento.
    The capital of Colorado is Denver.
    The capital of Connecticut is Hartford.
    The capital of Delaware is Dover.
    The capital of Florida is Tallahassee.
    The capital of Georgia is Atlanta.
    

