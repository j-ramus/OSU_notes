# dynamic meme

any time yu create regular variables like int x; double* p...
they go on the stack

last in $\longrightarrow$ first out

this is because of scope

---

If you want variables to stick around, you cant use the stack (automatic memory)

If you use automatic memory, you cant decided when it is deleted

with pointer to new (dynamic array): pointer is on the stack, poinmt to something in the heap

the stack pointer gets deleted, but the array says around in the heap

the new keyword create an unnamed array that the corrspoining named pointer points to

stack is much smaller than the heap

dyanmic memoryis only accesable through pointers

use after free: dref point that no longer point to allocated memeory

---

# Structures

A struct is a user defined datatype

represents a container of other datatypes

function of a struct type returns a struct object

declaring new object frim struct: `baseball_player joe;`

use dot operator for initalization/calls:

`joe.name = "steve"`

passing:

```

void printBaseballPlayer(baseBallPlayer player) {
    std:cout << player.name << std::endl;
}

```

---

### initialization

```
baseball_player joe {
    "steve",
    37,
    0.6
}
```
you can use a colon (name: "steve"), but must be in same order

---

by default structs are passed by value

pass by reference,

or const reference if no modifcations

cant use dot operator if memeber variable was declared const in the struct declaration. you must then use the format in the initialiation example above.

yu can put structs inside of structs: called composition





