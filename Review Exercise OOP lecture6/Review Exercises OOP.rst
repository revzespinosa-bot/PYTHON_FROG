Review Exercise 1
=================

.. code:: ipython3

    #1
    class Dog:
        def __init__(self, name, age, coat_color):
            self.name = name
            self.age = age
            self.coat_color = coat_color
    
    philo = Dog("Philo", 5, "brown")
    print(f"{philo.name}'s coat is {philo.coat_color}.")


.. parsed-literal::

    Philo's coat is brown.
    

.. code:: ipython3

    #2
    class Car:
        def __init__(self, color, mileage):
            self.color = color
            self.mileage = mileage
    
    blue_car = Car("blue", 20000)
    red_car = Car("red", 30000)
    
    print(f"{blue_car.color} car has {blue_car.mileage:,} miles.")
    print(f"{red_car.color} car has {red_car.mileage:,} miles.")


.. parsed-literal::

    blue car has 20,000 miles.
    red car has 30,000 miles.
    

.. code:: ipython3

    #3
    class Car:
        def __init__(self, color, mileage):
            self.color = color
            self.mileage = mileage
    
        def drive(self, miles):
            self.mileage += miles
    
    my_car = Car("black", 0)
    my_car.drive(100)
    print(my_car.mileage)


.. parsed-literal::

    100
    

Review Exercise 2
=================

.. code:: ipython3

    class Dog:
        species = "Canis familiaris"
        def __init__(self, name, age):
            self.name = name
            self.age = age
            
        def __str__(self):
            return f"{self.name} is {self.age} years old"
            
        def speak(self, sound):
            return f"{self.name} says {sound}"
            
    class GoldenRetriever(Dog):
        def speak(self, sound="Bark"):
            return f"{self.name} says {sound}"
    
    dog = GoldenRetriever("Philo", 3)
    print(dog.speak())
    print(dog.speak("Woof"))
    


.. parsed-literal::

    Philo says Bark
    Philo says Woof
    

.. code:: ipython3

    class Rectangle:
        def __init__(self, length, width):
            self.length = length
            self.width = width
    
        def area(self):
            return self.length * self.width
    
    class Square(Rectangle):
        def __init__(self, side_length):
            super().__init__(side_length, side_length)
    
    square = Square(4)
    print(square.area())


.. parsed-literal::

    16
    

CHALLENGE: MODEL A FARM
=======================

.. code:: ipython3

    class Animal:
        def __init__(self, name, age, species):
            self.name = name
            self.age = age
            self.species = species
    
        def eat(self):
            return f"{self.name} {self.species} is eating."
    
        def sleep(self):
            return f"{self.name} {self.species} is sleeping."
    
        def __str__(self):
            return f"{self.name} is a {self.species} that is {self.age} years old."
    
    class Dog(Animal):
        def __init__(self, name, age):
            super().__init__(name, age, "Dog")
    
        def bark(self):
            return f"{self.name} Dog is barking loudly!"
    
        def run(self):
            return f"{self.name} is running in the park."
    
    class Cat(Animal):
        def __init__(self, name, age):
            super().__init__(name, age, "Cat")
    
        def meow(self):
            return f"{self.name} is meowing softly."
    
        def climb(self):
            return f"{self.name} is climbing a tree."
    
    class Bird(Animal):
        def __init__(self, name, age):
            super().__init__(name, age, "Bird")
    
        def chirp(self):
            return f"{self.name} is chirping happily."
    
        def fly(self):
            return f"{self.name} is flying high in the sky."
            
    dog = Dog("Philo", 1)  
    print(dog.sleep()) 
    print(dog.bark()) 
    print(dog.run())  
    print()
    
    cat = Cat("Garfield", 3)  
    print(cat.eat())  
    print(cat.meow())  
    print(cat.climb())  
    print()
    
    bird = Bird("Rio", 5)
    print(bird.eat())  
    print(bird.chirp())  
    print(bird.fly())  
    print()


.. parsed-literal::

    Philo Dog is sleeping.
    Philo Dog is barking loudly!
    Philo is running in the park.
    
    Garfield Cat is eating.
    Garfield is meowing softly.
    Garfield is climbing a tree.
    
    Rio Bird is eating.
    Rio is chirping happily.
    Rio is flying high in the sky.
    
    

