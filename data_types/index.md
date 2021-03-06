# An Introduction to Data Types

## What is a data type?

Pike works with **data items**,
also called **values**,
such as the integers **17** and **-4717**,
or the string of characters `"Hello world!"`.
Each data item has, or "is", a certain type:
**17** and **-4717** both have the type **integer**,
and `"Hello world!"` has the type **string**.
If we want to refer to the data type **integer**
in a Pike program,
we write `int`.
For the type **string**,
we write `string`.

Each variable, method, and method parameter also has a type.
The types of these determines which data items
you can put in the variable,
return from the method,
or use as arguments to the method.
An integer variable, created with

```pike
int i;
```

can only contain integer values.
If we try to put something else,
such as a string,
in this variable,
Pike will try to discover the discrepancy and complain about it.
This is called **type checking**.

`string` and `int` are **built-in types** in Pike.
You can also create your own data types, or **classes**.
We have already seen some examples of this,
for example the class `Query`,
which is part of the module `Protocols.HTTP`,
and which is used to contain the data we get
when we retrieve a page from the World Wide Web.

We will examine each individual data type in some detail in a later chapter,
but this chapter will give an introduction to data types in general.

## Different Kinds of Types

The data types in Pike can be divided into three categories:
the **basic types** (`int`, `float`, and `string`),
the **container types** (`array`, `mapping`, `multiset`),
and then the three types `program`, `object` and `function`.
We will start by looking at the basic types.
