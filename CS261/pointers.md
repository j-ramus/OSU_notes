#C Pointers

The dereference operator `*` is applied to pointers, and returns the
value addressed by that pointer.

`char *p` declares a pointer to a
char because after applying the operator, the result would be a
char.

`char c = 'a';`
`char *p = &c;`
In this example, we use the dereference operator to specify that
the value that the pointer p points to is a char. 

When applied toa pointer, the dereference operator returns the value pointed to by
that pointer. 

Similarly, when creating a pointer variable, we use
the dereference operator to specify the data type pointed to by
that pointer.

---

### Pointer Artihmetic

`char c = 'a';`
`char *p = &c;`
`printf("p = %p\n", p);`
`printf("p+1 = %p\n", p+1);`
`printf("p+2 = %p\n", p+2);`

It is perhaps not too surprising that when we add 1 to the pointer,
the result is the next hexadecimal number:

`p = 0x7ffeecb27a9b`
`p+1 = 0x7ffeecb27a9c`
`p+2 = 0x7ffeecb27a9d`

When working with other data types, however, the situation is a
little different, and that adding 1 to a pointer doesn’t always
increment the hex string by 1. When adding to a pointer, the
result is incremented by the value returned by the `sizeof()`
function. Let’s see an example using an int variable:

`int i = 1;`
`int *p = &i;`
`printf("p = %p\n", p);`
`printf("p+1 = %p\n", p+1);`
`printf("p+2 = %p\n", p+2);`

In this example, the code is the same as the previous char
example, but because the original variable `i` was defined as an `int`,
adding 1 increments the pointer value by 4, which corresponds to
the int having a size of 4 bytes.

`p = 0x7ffee915ba98`
`p+1 = 0x7ffee915ba9c`

