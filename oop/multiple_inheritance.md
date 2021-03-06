# Multiple Inheritance

Sometimes we want to inherit from two or more classes.
This works in Pike (and in C++, but not in Java).
You just write several inherits.

Lets say we have a class `friend`,
that represents a friend:

```pike
class friend
{
  void cuddle()
  {
    write("Cuddle, cuddle, cuddle!\n");
  }
}
```

A hamster,
as we all know,
is both an animal and a friend,
and it can also dance:

```pike
class hamster
{
  inherit animal;
  inherit friend;

  void dance()
  {
    write(name + " dances.\n");
  }
}
```

So, try it out:

```pike
hamster h = hamster("Blue Lightning", 0.12);
h->cuddle();      // Cuddle as a friend
h->eat("grain");  // Eat as an animal
h->dance();       // Dance as a hamster
```
