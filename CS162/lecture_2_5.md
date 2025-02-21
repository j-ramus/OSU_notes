# classes

if a class object is passed to another object of the same class, it can access the private members

Public member functions can call internal private member functions

Getters and setters undo encapsulation, but still better than public member variables

---

### Object

An object is a variable whose type is a class

---

### OOP

Programming that is centered around objects

---

```
fighter f1;
fighter f2;

//structured programming (old)
f2.health -= f1.power;

//OOP
f1.attack(f2);

```

---

### Class invariants

Invariant: something that is always the same no matter how it is transformed

Class invariant: Property about an object that is always true no matter what you do to the object

If member variable are private, acna only be modified by class' functions

---

quiz
1: a
2: t
3: c
4: f
5: f

---

memeber function to initialize members:

### Constructors

Automatically called on the object when it is declared, and sets up the object

###### Default constuctors

No parameters

###### Non-default constructors

Has parameters

COnstructors dont have return types, skip it

Ex: 
```
Circle::Cirlce() {
    this->center.x = 0;
    this->center.y = 0;
    this->radius = 1;
}
```

If you add parameters it becomes non defalut.

### overloading

Can have same fucntion as long as parameters are different

Default call: `circle c;`

Non default call: `circle c(center, radius);`

---

`circle::circle(point center, double radius) : center(center), radius(radius){}`

do it this way with memeber initializer list


