#Primitive datatypes
Data structures in C can be described as built from five
fundamental “elements” or building blocks that are combined to
form larger structures.

1. char
- 1 byte, signed or unsigned

2. void
- no size

3. int
- 2 or 4 bytes depending on system architexture

4. float
- 4 bytes
- double is 8 bytes

5. pointer
- 4 bytes on 32-bit systems
- 8 bytes on 64-bit systems

---

###sizeof()

The sizeof() function returns the size in bytes for any input
variable or data type. For a variable x, the value returned by
sizeof(x) quantifies the size of the variable

---

#printf()

At minimum, printf()
takes in a quoted string, as in printf("hello, world!").

If a properly formatted, %-labeled placeholder is in the quoted string
to specify the data type of each variable.



-    %d %i     Decimal signed integer.
-    %o	      Octal integer.
-    %x %X     Hex integer.
-    %u	      Unsigned integer.
-    %c	      Character.
-    %s	      String. See below.
-    %f	      double
-    %e %E     double.
-    %g %G     double.
-    %p        pointer.
-    %n	      Number of characters written by this printf.
-              No argument expected.
-    %%	      %. No argument expected.

---


