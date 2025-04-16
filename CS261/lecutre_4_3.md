quiz prep:

how many bits are needed to represent 1000 items?

$2^{10}=1024$
$\therefore$ we need 10-bits

$log_2(2^n)=n$

2. whaty is the minimum length of a hex string needed to index 1GB

$2^{30}\rightarrow$ 30-bits

relate to power of 16: $16^L$ 

$16 = (2^4)^L = 2^{4L}$
$4L$ must be greater than or equal to 30. 
$L\geq\frac{30}{4}


---

$\frac{log(1000)}{log(2)}=9.97$

a character is 1 byte/8-bit

$2^{10}=1024 \quad 2^9=512$

---

3. how many configurations of 1s and 0s can be stored in 16-bytes

$2^{128}$

8-bits time 16-bytes = 128

$2^{128}\approx10^{38}$

Representing a float with binary digits, the number must start with a non-zero integer

---

### Pointer Arithmetic

`char c = 'a';`
`char *p = &c;`
adding 1 to char pointer moves the address by 4 because a char is 4 bytes.
`0xdeadbeef0008`
+1 = `0xdeadbeef000c`

Adding one to a dereferenced int would not change its address

---

`malloc` memory allocation

user defined variable work best with a pointer to the struct


---

question: does a struct take additional memory?

answer: NO!

---

include string.h for strings


you cant use == to comaprare strings, must sue stringcompare

---

pointers point to data "nodes"

---

self referential data types


