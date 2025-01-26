# Dynamic Memory

strings need std::

std::string

use double quotes ""

std::string word = "Beef";

---

## comparing strings

if (word == some_other_word){}

COmparison is case sensitive

---

string can be read in just like its or other types

cin, getline, ifstream

cin only grabs up until first space

next word stays i buffer and calling cin gets the next word

---

an array is a homogeneous, **fixed size** sequence of data

they are store contiguously int memory, a single block of memeory


if you want to add another element, you need to make a new bigger array and copy the current data over

declare the array and run a for loop to copy the indices of array 1 to the second array, one by 1 with a loop

---

Stupid trick:

use a pointer to point to current bigger copied array

update by every time you copt the array to point tot he new array

```
int my_array[3] {12,8,3}
p= my_array; \\ points to base address



```
The pointer can be used like the array

`cout p[3]; \\ shift over 3 mempory spaces from base address stored in p`

but old arrays stick around in memory... :-(

---

Memeory address = 64bits = 8 bytes

---

## Accessing elements 

my_array[0] is base address + 0

cout << my_array; prints the base address of the first element of the array

cout << \*my_array; prints the first element of the array

`*(my_array[2] + 3)`

---

agretgate initialization

`my_array[3] {12,8,3};`


---

Variables lifetime is determined by scope.

leftover pointers fallen out of scope are dangline pointers

this causes use after free errors

if p point to my_array2, when we exit the function that was in, p points to deallocated memory

this is from automatic storage duration

---

## Dynamic storage duration

You decided when memory gets deallocated

`new` keyword

`int* my_array2 = new int[4]; \\ signals that you want to control when memeory is deallocated`

new = gets stored in the heap,

rregular, non dynamic arrays get stored on the stack

---

When you create dynamic memory but dont free it, it creates a memory leak

use delete while in the same scope

my_array2 exists on the stack and has auto management



`delete [] p ` not `delete [] my_array2`

this delets the memory that the pointer points to

you must set that pointer to null `p=nullptr;`

you can check if p is null  with an if statement

If you were ot have the original array on the heap, you must delete that too



---

### random tips

vectors resize exponentially

square brackets p[0] works automatically aas a dereference operator

---









