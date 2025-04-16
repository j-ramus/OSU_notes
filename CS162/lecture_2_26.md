# Lectures

resize(new size) curretn elemetns stay in place but adds uninitialized objects at the end (default constructor) 

if `new size` is less that the rogional size of vector, numbers get truncated

- reserve

words.push_back("word")

Vectors make the new dynamic array the size of the old array multipled by x, instead of being one bigger in dynamic arrary copying

- push back puts the new element in the first garbage value in the array's expansion (extra slots)

- calling size would display only the length of non-garbage elements

- while there are enough free spaces, vector only has to add the element and incrament the size

- $log_2(n)$ is the number of times the vector needs to do the expensive re-size and copy operations

- actual size in memory is called capacity (including the garbage slots)

- pushback always increses size by 1

- when deleteing elements, the capcity doesnt shrink

- directly modifiying capacity can be done with `reserve`

- `reserve` is a "polite request" to shrink

- `shrink to fit` can reduce to meat size

- `reserve` can be called on creation to avoid having to resize

---

# Templates

`std::vector<primitive>` is a class which has a parameter for that primitive

`std::vector` is a class template which uses pointers to whatever type is between the angle bracket.

- to make a template:

before class definiition: `template< >`

put the placeholders in between langle and rangle

`template<typename SOMETHING>`

then when instatiated, it throws whatever is put in the angle brackets




