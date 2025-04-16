### Extra polymorphism

`monster* m = new zombie;`

`m->do_turn();` calls dynamically bound zombie `do_turn()`

|function| pointer |
 ----    | ----
|do turn | pointer |

Each derived object has a vpointer to the object types vtable

---

# Vectors

Are objects that contains a dynamic array of some type of object (homogeneous)

automates the copying and deleting involved with dynamic arrays.

automatically implements big 3

syntax: `std::vector<object_type> vector_of_objects;`

`std::vector<>` is a class. when instatiated, it calls constructors etc.

`vector_of_objects.push_back()` push back is a member of all vector classes `push_back(object_to_add)`

can use square brackets: `std::cout << vector_of_objects[0]`

or with `.at(0)`

if using a `.at()` it does not cause overflow, but throws exception where square brackets cause undefined behavior

crashes are better tahn undefined behavior

at function returns a reference

square brackets are faster than `.at()`, but use `at` whenevr possible.

`at` returns a reference to the element of the array, not a copy

iterate through vector:

to get size use `.size()` which is a getter for an int store in the vector representing size

### iterators

object that represent the location of an element within a data structure

`objects_vector.begin()` returns first element iterator
`objects_vector.begin() +1 ` return second element iterator


to remove elements use `erase()`
`vecotr_objects.erase(vector_objects.begin())`

`std::vector<double>::iterator itr = vector_objects.begin()`
or use `auto itr = vector_objects.begin()`

iterator is a generic object for many types

some vector member functions use iterators, some use indicies

---

non-default constructor for vectors:

accepts initial size: `std::vector stuff list_of_stuff(10);`

another non default

`std::vector<things> stuff(size, exalple thing)`


--

`std::vector<std::vector<room> cave`

`cave.at(2).at(6)` gives 3rd row 7th column
