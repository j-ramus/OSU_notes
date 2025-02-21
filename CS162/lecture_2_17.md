# inheritance

Purpose of inheritance: creating an "is a" relationship: "every zombie is a monster"

everything from parent gets inherited by child that is public

protected allows child classes to access the private members of the parent class

`zombie z;`
`monster m= z;` is legal because all zombie are monsters

this calls the monster copy constructor

this is type of casting called "upcasting"

casting zombie "up" to parent class

when this happens, m loses the zombie only members:

`z.eat_brains()` works, but `m.eat_brains()` doesnt.

z and m both have HP, that stays

- object slicing is when upcasting discards child objects memebers

monster is only x bytes, so it can only take what fits in the memory allocated for a monster

overriding is when you are overloading a function in a child class which has the same parameters

compiler by default call lowest function with that name in family tree

to call function from parent/grandparent that has been overriden, use scope resolution operator
`z.monster::do_turn()`

---

# Polymorphism





