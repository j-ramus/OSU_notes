# Pointer and references

Pointers are a layer of indirection

If you create variable (int x;) it creates a 4byte chunk of memory (in  ram)

Uninitialized variables contain whatever value was there before

When assigned it rewrites the memory

If you do something with x like cout, it grabs the value from x's address

To get the address of a variable: std::cout << &x; prints the address

To store address of one variable in another variable:

`int *y=&x;`

&x is not an integer 

`int *y` store the address of an int

pointers are always 8-bytes

y is the address of x and points to x

### dereferencing

Us an asterisk: deref operator aka indirection operator

`std::cout << *y;` prints the VALUE of x

`std::cout << &y;` prints the ADDRESS of x

silly stuff: `*(&y)` print address

$y\equiv \ \&x$

$*y \equiv x$

## but why?

```
void changeMe(double* pi) //function is passed a pointer
  *pi =3.14; //variable that it points to by derefernce
}

main(){

changeme(&pi) // passes address to pointer
}
```
parameters are copies of arguments


## refernces

references are basically pointers with a simpler syntax

stick to refernces whenever possible

when declaring: `(double& pi)` <- reference
in body, it does not have to be derefernced, it does it by default without a * 
pi=3.14

this means the function modifies the referenced variable instead og a copy

when calling, no & needed: `change_me(pi);`

#### what is the difference
1. syntax
`double* pi_pointer = &pi;`
`double& pi_reference = pi;`

`pi_reference =12; // changes pi to 12`
`*pi_pointer = 12; //changes pi to 12`
`pi_pointer = &gravity; // changes pi_pointer to the address of gravity`
`std::cout << *pi_pointer; //prrints 9.81`

`pi_pointer = 12; //illegal, tries to set address to 12`

2. when you create a reference, at the moment you declare it you must initialize. the refence will always refer to where it was origionally assigned

`pi_reference = gravity; //changes pi to the VALUE of gravity`

3. pointers can be set temporaraly to no vallue
`pi_pointer = nullptr;`

the is no such thing as a null refernce, because references cannot be changed

nullptr can be used as a ternary statement

`if (pi_pointer != nullptr)`
`if (pi_ptr); // true if poinmter points to anything but null`

"segamtion core dumped" from runtime is maybe a nullptr error, but not always

4. dangling pointer

when i pointer is passed the address of a variable the falls out of scope or gets deleted.
this is a "use after free" error

5. if you create a pointer to the first element of array:
`char* char_pointer = &(my_chars[0]);`
it can be used to point to the array itself



## From Lab 3

from the declaration: void foo(int* iptr)
and the call fooA(&x)

```
*iptr //Dereferencing iptr gives the value of the integer being pointed to (the value of x).
iptr //This holds the address of the integer x.
&iptr //This is the address of the pointer variable iptr itself.
```

##### Passing arguments

`int foo(int* a, int& b, int c);`

```
int* a //This expects a pointer to an integer. You must pass the address of an integer variable (using the & operator).

int& b //This expects a reference to an integer. You must pass an integer variable directly (not a pointer or address).

int c //This expects a copy of an integer value. You can pass an integer literal or variable.


int result = foo(&x, y, z);
```
