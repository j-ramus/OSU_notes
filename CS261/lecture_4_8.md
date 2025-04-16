# Abstract data types ADT

### Lists

- sequences of elements
$L=e_1,\dots,e_n$ assuming $n>0$

- build/create(x) reset a list's memory to empty

---

### stdlib

- malloc() : Memory allocation `p=malloc(size)`
Returns a pointer to a `void`
that pointer can be cast to a specified type
`p = (type*) malloc(size);`

ex: `p = (int*) malloc(length * sizeof(int));`

- calloc(): initializes memory with zeros

`c= (int*)calloc(length * sizeof(int));`

- `realloc();` if realloc can fit, it will find a new block on the heap.

- `free();` allocated memory must be freed

---

### public and private:

- public: function is declared in `.h` file
- private: function is in `.c` file, but not in `.h`
