# Searching


Searching array L: \[1, -2,3,7,12\] V: 6

Determine if V is in L

main two algos

1.  Linear Search

- time: n

- Start at index 0 to end of array witha for loop

```

for (int i = 0; i \< size; i++){
  if (L[i] == V) {
    return true;
  }
  return false;
}
```

Operrates in linear time

For linked list, traverse pointer by checking value until reading the tail

In most cases, linear search is the best you can do

2. Binary search 

- time $log_2(n)$ where n is length of list

imposing restrictions
if list is sorted:
go to middle of list and check if value is greater or less than target

`['A', 'L', 'M', 'Y', 'Z']`
If checking for J, it must be on the left side of the inital cahracter, M

Binary search is slow for linked lists because you have to find the middle first

---


# Sorting

1. Selection sort

- find smallest value
- put it where is belongs
- repeat n-1 times (last element will end up where it needs to be by the time you get to it)


2. Insertion sort

- find element immediately to the right of the liine
- left part is sorted, right is unsorted

steps:  1. take first unsorted value
        2. insert it where it goes on sorted side
        
insertion is hard with singly linked lists

can work with doubly linked lists

3. Merge Sort

`[12, 7, 8 ,3]`

Sort in ascending order

Divide and conquer recursive sorting algorithim

Split list in half and sort both sides

base case: list with 1 element = do nothing

#### merging two sorted lists

`[2, 4, 6]&[1,3,5]`

For arrays: **Not done in place**, copy to new array

For *linked lists*: It should be done in place

- compare first element of both arrays

- move smaller of 2 into new array

- compare larger of 2 to second element of other array

- i=0 index of first element first array
- j=0 second array
- k=0 first (garbage) index of new array.

- increment k and i or j depending on where the smaller element came from

- for assignment 5, insert nodes without changing the adresses and order of pointers

- list can be split into two lists with two heads

- insert/ 


