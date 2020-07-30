# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Something that can take many different forms, it has several different is-a's.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

Different objects can be accessed through a common interface. Ex. ArrayList<IFly> could be an ArrayList of Bird, Plane or Superman objects since they all implement the IFly interface, they can all fly.

3. What can we use to implement polymorphism in Java?

Interfaces, they will define a behaviour that all objects that implements the interface will have (how each object does something might differ but they will all have the method/-s defined in the interface).

4. How many 'forms' can an object take when using polymorphism?

No. of forms = x + 1

x = no. of interfaces the object implements
1 = the objects original form

5. Give an example of when you could use polymorphism.

A fridge could have an ArrayList of food items, each with a separate class. Each class could implement the iConsumable interface meaning that the fridge's ArrayList would store <iConsumable> items.


# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

A class that HAS-A(n) object of another class.

7. When would you use composition? Provide a simple example in Java.

Whenever an object has something that in itself is an object with separate properties and methods. Ex. A Flat object could have a Door object. The door has it's own properties (height/width, colour, etc.) and methods (open, close, lock etc) but none of that needs to be put in the flat class, the flat only need to know that it has a door, the door class handles all door things.

8. What is/are the advantage(s) of using composition?

Keeps the code dry and easy to read, all behaviour related to the class is handled in the class (see flat/door above). Having separate objects allows them to be re-used in other places as well, a house could also have a door object and you wouldn't need to write all the door code in both flat and house.

9. When an object is destroyed, what happens to all the objects it is composed of?

They're destroyed as well.