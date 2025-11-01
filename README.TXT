Project: zuul-bad
Authors: Michael Kölling and David J. Barnes

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

This project is a simple framework for an adventure game. In this version,
it has a few rooms and the ability for a player to walk between these rooms.
That's all.

To start this application, create an instance of class "Game" and call its
"play" method.

This version of the game contains some very bad class design. It should NOT
be used as a basis for extending the project without fixing these design
problems. It serves as an example to discuss good and bad design (chapter 8
of the book).

Chapter 8 of the book contains a detailed description of the problems in this
project, and how to fix them.

The project 'zuul-better' contains a version of this project with better
designed class structure. It includes the fixes discussed in the book.



1)
	a)the application is a game that allows you to move around a bit
	b)go,help,quit
	c) the go command followed by the dirrection allows yoiu to go to that direction
	d)4 rooms
9)Returns a Set view of the keys contained in this map. The set is backed by the map, so changes to the map are reflected in the set, and vice-versa. If the map is modified while an iteration over the set is in progress.
13) the go command changes the player location so the only change it brings in the object diagram is that when you use it to go the next room it will now point to the new room you are in instead of the room it was pointing to before.
17) no because now since we are calling parser.getcommands().showAll() the show all methode reads and prints all the commands stored in the CommandWords object.
18)pros-it simplifies the parse and game classes because they would not need to creat and store commandwords object, which reduces the complexity.
cons-static methods make code less flexible if we ever decide to change the code in the future.