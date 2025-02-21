# File separation

### rules

1. In each .cpp file, every function that is called in that cpp file must be **declared** at least once before it is called.

2. Across all of your .cpp files every function that is used anywhere must be **defined** exactly once.

3. In each .cpp file, every structure type that is used in that cpp file must be **defined exactly once** before it is used.

- 1 and 3 throw compiler errors, 2 throws a linker error


---


- function prototype: declaration without definition

- Pre-process -> compile -> assemble -> link

- in prototype you only need to supply the types of parameters, not the names of the parameters (not a great idea)

---

To compile : list cpp file one by one in g++

---

- include is a preprocessor directive that pastes that file into that line of code

---

##### In main.cpp

include all hppp

`#include "name of header.hpp"`

use quotes instead of langle rangle, which point to the path

---

#### header guards

wierd behavior if header included twice, redefinition error

Header guards prevent this 

in **every** header you shoulld use

```
#ifndef HELLO_HPP //arbitray constant for ifndef 
#define HELLO_HPP

body

#endif

```



`ifndef` or `pragma once`


overloading: two functions with same name and different parrams = two different functions

---

suppose you have header a.hpp which include b.hpp, which include c.hpp, which includes a.cpp

this is called circular includes which breaks everything

solutoion, take what c.hpp needs from a.cpp and move it to a new d.hpp

"incomplete type" error



