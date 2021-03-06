# Object Orientation in Pike

## Programs Within Programs: Object-Oriented Pike

As we have said before,
a **class** is a description of a type of thing.
You can **clone** the class to create **objects**.
Each object is a **clone**
(sometimes called **instance**)
of the class.

A class contains some variables,
which are sometimes called **member variables**.
The variables are attributes or characteristics of the objects,
and each object will have
its own set of the member variables.
For example,
if the class `animal` has the member variables `name` and `weight`,
then each animal will have those two variables,
so each animal can have a name and a weight.

A class also contains some methods.
(C++ programmers would call them "member functions".)
The methods describe things that the objects can do.

For example,
if the class "animal" has the method `eat`,
then you can call that method in any animal,
to make it eat.
Well, of course it won't really eat,
since it's just some data in the computer
and not a real animal.
But the method can change the member variables,
for example by increasing the value of `weight` for that animal.
