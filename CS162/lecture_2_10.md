# The Big 3

1. constructors

default constructor takes no arguments, bvut can have initializer list

non default takes arguments

If no constuctors are supplied, compiler generates default constructor that does nothing

if non-default constructor created, no default constructor is auto generated. Now the default constructor must be explicitly defined


```
pokemon array[10];
pokemon* heap_pokemon = new pokemon[12];
```

placement new

explicit constructor call

for my contenders array
`array[0] = Pokemon(argument);`

deault constructor for strings sets up an empty string

default values can be added to declarions in hpp

`int attack = 1`

default can be declared as `pokemon() = default;` and does not need to be defined in cpp file

### nest object constructors  

inner objects are constructed before the outer object

2. Destructors

needs access to private memeber variables



