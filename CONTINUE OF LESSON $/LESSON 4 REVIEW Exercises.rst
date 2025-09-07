.. code:: ipython3

    # REVIEW QUESTION 5

.. code:: ipython3

    while True:
        try:
            number = int(input("Enter an integer: "))
            print(f"You entered: {number}")
            break  # stop loop once valid integer is entered
        except ValueError:
            print("Try again! That was not an integer.")
    


.. parsed-literal::

    Enter an integer:  
    

.. parsed-literal::

    Try again! That was not an integer.
    

.. parsed-literal::

    Enter an integer:  2
    

.. parsed-literal::

    You entered: 2
    

.. code:: ipython3

    text = input("Enter a string: ")
    
    try:
        n = int(input("Enter an index number: "))
        print(f"The character at index {n} is: {text[n]}")
    except ValueError:
        print("Invalid input. Please enter a valid integer for the index.")
    except IndexError:
        print("Index out of range. The number is too large for the given string.")
    


.. parsed-literal::

    Enter a string:  Revo
    Enter an index number:  2
    

.. parsed-literal::

    The character at index 2 is: v
    

REVIEW QUESTION 6
=================

.. code:: ipython3

    import random
    
    def roll():
        return random.randint(1, 6)
    
    print("You rolled:", roll())
    
    


.. parsed-literal::

    You rolled: 2
    

.. code:: ipython3

    
    total_rolls = 10000
    sum_of_rolls = 0
    
    for _ in range(total_rolls):
        sum_of_rolls += roll()
    
    average = sum_of_rolls / total_rolls
    
    print(f"After {total_rolls} rolls, the average number rolled is: {average}")
    


.. parsed-literal::

    After 10000 rolls, the average number rolled is: 3.4882
    

.. code:: ipython3

    import random
    
    # Probabilities of Candidate A winning each region
    p_region1 = 0.87
    p_region2 = 0.65
    p_region3 = 0.17
    
    def simulate_election(trials=100000):
        wins_for_A = 0
        
        for _ in range(trials):
            # Simulate each region
            r1 = random.random() < p_region1  # True if A wins
            r2 = random.random() < p_region2
            r3 = random.random() < p_region3
            
            # Count how many regions A won
            regions_won = sum([r1, r2, r3])
            
            # Candidate A becomes mayor if 2 or more regions won
            if regions_won >= 2:
                wins_for_A += 1
        
        return wins_for_A / trials  # probability
    
    # Run the simulation
    probability_A_wins = simulate_election()
    print(f"Estimated probability Candidate A wins the election: {probability_A_wins:.4f}")
    


.. parsed-literal::

    Estimated probability Candidate A wins the election: 0.6349
    

