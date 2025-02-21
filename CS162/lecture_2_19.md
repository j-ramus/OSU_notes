# Polymorphism

`monster[i]= z;` implicit upcasting

slices zombie object

trick: mosnsters are smaller than zombies, so zombies wont fit

zombie pointers are the same size as monster pointer: 8-bytes


create array of monster pointers, upcast zombie and vampire pointers to monster pointers, store in moster array

`monster** monsters = new monster*[15];` <- store the first address of an array of monster pointers

create zombie on heap `zombie* z = new zombie`

---

#### 2nd problem

`monster[i]->do_turn()`
compiler will default to monster virtual functions instead of the scope local to the child objects

this is called **static binding** <- in this context means before runtime, or at compile time

every vatiable has a static type and a dynamic type. Static stype of variable: declared type. Dynamic type: its "actual type" 

static type is `monsters[i]` =mosnter*
dynamic type is iether zombie* or vampire*

dynamic info not available at compile time

Solve thr peoblem with dynamic binding:

in base class, put the word virtual in front of overrideable functions


