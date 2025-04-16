# STL
 standard template library: stuff that got incorporated into c++ back in the 90s

 Vector is basically a dynamic array. resizable with performance boost

 vecotrs are contiguous and support random access

 they are positional AKA sequential: the container represents a sewuence of elements such that each element has a position decided by the programmer

 `std::array` a wrapper around an automatic (regular) array, non dynamic

 `std::array<int, 10> = object`

### set

 `std::set<type>` a bag of unique data, they elements added to the set must be unique

 `std::set<int>::iterator find_result = my_set.find(100)`

finding matching elements with set is fast and they use hash tables

adding and removing elements is slower than vectors

### multiset

set than can have duplicates

sets are **associative** containers: and container that is not sequential

they *associate* keys with values

### maps

`std::map` is a class template with two template parameters:

`std:map<string, int>` asscoicates a string with an integer

equivilent to dictonary in python

`std::<std::string, int> names_to_ages;`

`names_to_ages.insert("alex", 25);`
`names_to_ages.find("alex", 25):`

sets associate keys with themselves (is it in the set or not)

___

TODO read about vector, set and map

---

# Linked Lists

because vectors are implemented as arrays, they are contiguous

linked lists can have elements in arbitrary places

nodes are objects oor structures 

each node has two things in it: a value and a pointer called "next" which points to another node

last node is called tail

each node is created on the heap

use a pointer to the head to access

first node: `std::cout << head->value;`
next node: `std::cout << head.next->value;`










