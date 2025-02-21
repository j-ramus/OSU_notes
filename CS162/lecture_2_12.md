# The Big 3


anytime a class has dynamic memory, you need the big 3

1. Copy constructor

redefines "="

`this->variable = other.variable;`


when a copy is made by passing the object by value, it uses the copy constructor

2. Copy AOO

for when an already created object gets another object copied to it

Synatx: has a return type. Can be a reference

`taxpayer& operator=(const taxpayer& other)` defines what = does between 2 existing objects

the main difference in the logic is that you need to delete the dynamic memory that exists in the object that is being copied to

`if(this-> defpendents != nullptr){delete [] this->dependents}`

`ben = ben` deletes the memory that is going to be copied before the copy happens though

`if(this == & other){return *this;}` end function 


```

return *this;
```

th return types `(ben=alex).print()` copies then prints ben

3. destructor

when class is freed from memory, make internal allocated memory, like dynamic arrays need to be deleted

The destructor is called automatically

it is safe to delete a null pointer



Double free: when data on heap is allocated and freed twice. gives segmentation fault


